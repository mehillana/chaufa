# Chaufa

Chaufa is a minimalist programming language designed for data organization, storage, retrieval, and processing. It provides a simple syntax that eliminates unnecessary boilerplate code, making it the easiest modern language to learn and use.

Chaufa source files use the `.cha` file extension and are executed using a lightweight Python interpreter.

## Target Audience: Who is Chaufa for?

Chaufa is specifically designed for:

* **Data-focused Users:** Anyone who needs to organize, store, process, and query data quickly without setting up complex databases or bloated environments.
* **Beginners and Students:** Learners who want to master data logic and system operations without fighting against syntax errors, brackets, or strict formatting rules.
* **Terminal Developers:** Users who want a clean, text-based tool to handle simple automation, system logging, and tabular data management directly from the command line.

## Why Chaufa is the Easiest Modern Language

Chaufa replaces traditional language complexity with a clean, functional design:

1. **Zero Boilerplate:** No main functions, imports, semicolons, quotes, or parenthetical nesting required to display text or manipulate variables.
2. **Predictable Architecture:** Every line clearly signals its purpose using simple single-character prefixes (`/` for visual output, `:` for functions).
3. **Streamlined Data Pipeline:** Input capture, variable assignment, and string interpolation happen sequentially and naturally without managing data types manually.

## Architecture

The system operates line-by-line using a single-character prefix system:

* `/` represents screen output and display lines.
* `:` represents system and data manipulation functions.
* `(:function)` or `(:variable)` represents inline data interpolation within display lines.

## File Structure

* `README.md`: Overview and repository guidelines.
* `functions.md`: Complete documentation of all available Chaufa functions.
* `examples.md`: Practical examples of Chaufa code.
* `LICENSE`: License terms for the repository.

## Requirements and Execution

Execution requires Python 3.x installed on the system.

To run a `.cha` file:

```bash
py chaufa.py script.cha
