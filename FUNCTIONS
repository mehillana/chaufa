# Chaufa Function Reference

This document provides a comprehensive reference for all functions available in Chaufa for data handling, storage, arithmetic, and system management.

## 1. Input, Output, and Screen Control

| Prefix / Function | Description | Syntax Example |
| --- | --- | --- |
| `/` | Displays text on the terminal screen | `/Display this message` |
| `:inserttext` | Prompts the user to input text | `:inserttext` |
| `:saveinfo` | Saves the last entered or evaluated value into the temporary memory buffer | `/Value: (:saveinfo)` |
| `:clearscreen` | Clears the current terminal display | `:clearscreen` |
| `:printline` | Outputs a horizontal dividing line | `:printline` |
| `:pause` | Halts execution until any key is pressed | `:pause` |
| `:asknumber` | Prompts specifically for numeric user input | `:asknumber` |
| `:askdate` | Prompts for date input | `:askdate` |
| `:confirm` | Asks the user for a Yes/No confirmation | `:confirm Are you sure?` |
| `:printspace` | Prints a single blank line | `:printspace` |

## 2. Memory and Variable Storage

| Function | Description | Syntax Example |
| --- | --- | --- |
| `:savevar` | Stores a buffer value into a named key | `:savevar variable_name` |
| `:loadvar` | Retrieves a value from a named variable | `(:loadvar variable_name)` |
| `:deletevar` | Removes a variable from memory | `:deletevar variable_name` |
| `:showallvars` | Displays all active variables and their contents | `:showallvars` |
| `:clearallvars` | Deletes all stored variables from memory | `:clearallvars` |
| `:copyvar` | Copies the value of one variable into a new key | `:copyvar target_var source_var` |
| `:renvar` | Renames an existing variable key | `:renvar new_key old_key` |
| `:checkvar` | Verifies whether a key exists in memory | `:checkvar key` |
| `:countvars` | Returns the total count of stored variables | `(:countvars)` |
| `:lockvar` | Marks a variable as read-only | `:lockvar key` |
| `:unlockvar` | Removes read-only status from a variable | `:unlockvar key` |
| `:exportvars` | Exports active variables to a formatted text file | `:exportvars` |

## 3. Lists and Sequential Data

| Function | Description | Syntax Example |
| --- | --- | --- |
| `:createlist` | Initializes an empty list structure | `:createlist list_name` |
| `:addtolist` | Appends a value to an existing list | `:addtolist list_name value` |
| `:removefromlist` | Removes an element from a list by index | `:removefromlist list_name 0` |
| `:getfromlist` | Retrieves an element from a list by index | `(:getfromlist list_name 0)` |
| `:countlist` | Returns total items in a list | `(:countlist list_name)` |
| `:showlist` | Prints all items contained in a list | `:showlist list_name` |
| `:sortlist` | Sorts list elements in ascending order | `:sortlist list_name` |
| `:clearlist` | Clears all elements from a list | `:clearlist list_name` |
| `:searchlist` | Searches for a term within a list | `:searchlist list_name term` |
| `:joinlist` | Concatenates list elements using a specified separator | `:joinlist list_name ,` |
| `:reverse` | Reverses the order of list elements | `:reverse list_name` |
| `:poplist` | Removes and returns the last element of a list | `(:poplist list_name)` |
| `:duplicatelist` | Clones a list into a new list key | `:duplicatelist target source` |

## 4. Tables and Structured Data

| Function | Description | Syntax Example |
| --- | --- | --- |
| `:createtable` | Defines table column headers | `:createtable Name,Age,Role` |
| `:insertrow` | Adds a row of comma-separated data to the active table | `:insertrow Alice,28,Admin` |
| `:deleterow` | Deletes a table row by zero-based row index | `:deleterow 0` |
| `:showtable` | Displays the formatted table in the terminal | `:showtable` |
| `:filtertable` | Displays rows matching a column comparison | `:filtertable Age > 20` |
| `:countrows` | Returns the total number of rows in the active table | `(:countrows)` |
| `:getcell` | Fetches a cell value by row index and column header | `(:getcell 0 Name)` |
| `:updatecell` | Overwrites a cell value by row index and column header | `:updatecell 0 Age 29` |
| `:cleartable` | Removes all rows and headers from the active table | `:cleartable` |
| `:exporttable` | Exports the active table data to a CSV file | `:exporttable` |

## 5. Text Processing

| Function | Description | Syntax Example |
| --- | --- | --- |
| `:uppercase` | Converts text string to uppercase | `:uppercase text` |
| `:lowercase` | Converts text string to lowercase | `:lowercase text` |
| `:len` | Returns the character length of a text string | `(:len text)` |
| `:trim` | Removes leading and trailing whitespace | `:trim text` |
| `:replace` | Replaces occurrences of a substring | `:replace target_var old new` |
| `:substring` | Extracts text given a start and length index | `(:substring text 0 5)` |
| `:concat` | Combines two text strings | `:concat str1 str2` |
| `:contains` | Checks if a string contains a specified substring | `:contains text query` |
| `:split` | Splits text into a list using a delimiter | `:split text ,` |
| `:capitalize` | Capitalizes the first letter of a text string | `:capitalize text` |
| `:repeattext` | Repeats a text string N times | `:repeattext text 3` |
| `:padleft` | Pads a string on the left to a specified length | `:padleft text 10 0` |

## 6. Arithmetic and Mathematics

| Function | Description | Syntax Example |
| --- | --- | --- |
| `:math1x1` | Runs internal system math verification check | `(:math1x1)` |
| `:add` | Adds two numeric values | `:add 10 5` |
| `:sub` | Subtracts second numeric value from first | `:sub 10 5` |
| `:mult` | Multiplies two numeric values | `:mult 4 5` |
| `:div` | Divides first numeric value by second | `:div 20 4` |
| `:mod` | Computes the modulus of two values | `:mod 10 3` |
| `:round` | Rounds a float value to the nearest integer | `:round 4.7` |
| `:max` | Evaluates and returns the highest value | `:max 12 45` |
| `:min` | Evaluates and returns the lowest value | `:min 12 45` |
| `:sumlist` | Computes total sum of numeric items in a list | `(:sumlist list_name)` |

## 7. System Date, Time, and Logging

| Function | Description | Syntax Example |
| --- | --- | --- |
| `:gettime` | Returns the current system time (HH:MM:SS) | `(:gettime)` |
| `:getdate` | Returns the current system date (DD/MM/YYYY) | `(:getdate)` |
| `:getyear` | Returns the current four-digit year | `(:getyear)` |
| `:getmonth` | Returns the current month number | `(:getmonth)` |
| `:getday` | Returns the current day of the month | `(:getday)` |
| `:log` | Appends a timestamped record to the session log | `:log System check complete` |
| `:showlog` | Outputs all session log records to screen | `:showlog` |

## 8. Control Flow and Program Execution

| Function | Description | Syntax Example |
| --- | --- | --- |
| `:if` | Evaluates a conditional block | `:if variable == value` |
| `:else` | Declares an alternative execution block | `:else` |
| `:endif` | Closes a conditional block | `:endif` |
| `:endprogram` | Explicitly terminates script execution | `:endprogram` |
