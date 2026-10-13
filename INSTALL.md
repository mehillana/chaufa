# Chaufa Installation Guide

This document contains instructions to set up Chaufa and the full source code for the Python interpreter (`chaufa.py`).

---

## 1. Requirements

- **Python 3.8** or higher installed on your system.

---

## 2. Interpreter Source Code (`chaufa.py`)

Create a file named `chaufa.py` in your project folder and paste the following Python code:

```python
import sys
import os

class ChaufaInterpreter:
    def __init__(self):
        self.variables = {}
        self.log_history = []
        self.temp_info = ""

    def run_file(self, filename):
        if not os.path.exists(filename):
            print(f"Error: File '{filename}' not found.")
            return

        with open(filename, 'r', encoding='utf-8') as f:
            lines = f.readlines()

        for line in lines:
            line = line.strip()
            if not line:
                continue

            if line.startswith('/'):
                text = line[1:]
                # Replace variable interpolation (:loadvar name)
                for var_name, var_val in self.variables.items():
                    text = text.replace(f"(:loadvar {var_name})", str(var_val))
                print(text)

            elif line.startswith(':'):
                cmd_parts = line[1:].strip().split(' ', 1)
                cmd = cmd_parts[0]
                arg = cmd_parts[1] if len(cmd_parts) > 1 else ""

                self.execute_command(cmd, arg)

    def execute_command(self, cmd, arg):
        if cmd == "printspace":
            print("")
        elif cmd == "inserttext":
            self.temp_info = input("> ")
        elif cmd == "saveinfo":
            pass
        elif cmd == "savevar":
            if arg:
                self.variables[arg] = self.temp_info
        elif cmd == "log":
            # Replace variable interpolation in log entry
            log_text = arg
            for var_name, var_val in self.variables.items():
                log_text = log_text.replace(f"(:loadvar {var_name})", str(var_val))
            self.log_history.append(log_text)
        elif cmd == "showlog":
            print("\n--- LOG HISTORY ---")
            for entry in self.log_history:
                print(f"- {entry}")
            print("-------------------\n")
        elif cmd == "endprogram":
            sys.exit(0)

if __name__ == "__main__":
    if len(sys.argv) < 2:
        print("Usage: python chaufa.py <file.cha>")
    else:
        interpreter = ChaufaInterpreter()
        interpreter.run_file(sys.argv[1])
