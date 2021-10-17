# Syntax Coloring for Snowflake Stored Procedures

This is a simple Syntax Coloring Extension for Snowflake Stored Procedures and now also for python scripts. 

This extension is more useful if you are using the SnowConvert tool to move code from Teradata, Oracle or SQL Server to Snowflake.


## Release Notes


### 1.0.0

Initial release of syntax coloring for SnowScript

### 1.0.1

Some minor reviews

### 1.0.2

Added support for doing SQL Syntax highlight. 
This is currently being done only inside EXEC(`sql`) 
or snowconvert_helpers.execute_sql_statement("""
sql
""")

### 1.0.3

Fixed issue that required a new line character for hightlight on `EXEC` or `CURSOR` calls.
Added support to hightlight the `snowflake.execute` and `snowflake.createStatement` calls as well.

### 1.0.4

Fixed issue with `EXEC` helper delimiter in both JS and Python scripts.
Thanks to Jonathan!!!

### 1.0.5

Added support to highlight `SELECT` calls.

### 1.0.6

Added support to highlight `INSERT_TEMP` calls.
Also integrating commands for quick selection.


# Examples

## General JS Highlight

![sample](./sample_procedure.png)

## SQL Highlight inside the procedures
![sample1](./sample_procedure2.png)

## SQL Highlight in python 
![sample2](./sample_python.png)


## Keyword shorkcuts extensions

I copied this excellent extensions from https://github.com/dbankier/vscode-quick-select/

They are very handy :) specially to select all the SQL or all the parameters
## Usage

Here some examples - and it supports multiple selections.

In the examples below use <kbd>CTRL</kbd> instead of <kbd>⌘</kbd> for Windows.

<kbd>⌘</kbd><kbd>k</kbd> <kbd>"</kbd>

![doublequotes](https://github.com/orellabac/snowflake-sp-syntax-coloring/raw/master/images/doublequotes.gif)

<kbd>⌘</kbd><kbd>k</kbd> <kbd>'</kbd>

![singlequotes](https://github.com/orellabac/snowflake-sp-syntax-coloring/raw/master/images/singlequotes.gif)

**NEW:** You can also use this following shortcut to select either single, double quotes or backticks

<kbd>⌘</kbd><kbd>k</kbd> <kbd>;</kbd>

**NEW:** You can also use this following shortcut to toggle quotes, e.g. `"word"` to `'word'`

<kbd>⌘</kbd><kbd>k</kbd> <kbd>:</kbd>

**NOTE:** the extensions can be configured to exclude backticks from selection or switching

<kbd>⌘</kbd><kbd>k</kbd> <kbd>`</kbd>

![singlequotes](https://github.com/orellabac/snowflake-sp-syntax-coloring/raw/master/images/backticks.gif)

<kbd>⌘</kbd><kbd>k</kbd> <kbd>(</kbd> and
<kbd>⌘</kbd><kbd>k</kbd> <kbd>[</kbd> and
<kbd>⌘</kbd><kbd>k</kbd> <kbd>{</kbd>

Using the following performs and outer selection:

<kbd>⌘</kbd><kbd>k</kbd> <kbd>)</kbd> and
<kbd>⌘</kbd><kbd>k</kbd> <kbd>]</kbd> and
<kbd>⌘</kbd><kbd>k</kbd> <kbd>}</kbd>

Or if you have already made in inner selection, use the same key combination again to expand to an outer selection.

![brackets](https://github.com/orellabac/snowflake-sp-syntax-coloring/raw/master/images/brackets.gif)


<kbd>⌘</kbd><kbd>k</kbd> <kbd><</kbd>

This also selects the matching tag.

<kbd>⌘</kbd><kbd>k</kbd> <kbd>></kbd>

This matches the tag value.

![brackets](https://github.com/orellabac/snowflake-sp-syntax-coloring/raw/master/images/tags.gif)

