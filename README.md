# Chaufa

Chaufa is a minimalist programming language designed for data organization, storage, retrieval, and processing. It provides a simple syntax that eliminates unnecessary boilerplate code.

Chaufa source files use the `.cha` file extension and are executed using a lightweight Python interpreter.

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
```
