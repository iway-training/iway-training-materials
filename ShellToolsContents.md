# Shell tools

## Getting help
* man: interface to online manual (more popular than info)
* info: read Info document, but if Info document is unavailable, use man page instead.
### Compare:
| man | info |
| more popular | less popular |
| key binding like vim | keybinding like emacs |
.... (Need add more)

## sed
### Introduction
    This is a special editor for modifying automatically
### Pattern
Use regular expression
### Command
* s: substitution
* d: delete, reversing: !
* p: print, reversing: !
* q: quit
* a: append a line
* i: insert a line
* c: change a line
### Range
* By line number
    - Single line
    - Multiple lines
    - $: last line
* By pattern
    - Begin and end pattern
    - Mix with line number
### Grouping
Using { and }

## awk
### Introduction
AWK is an versatile programming language for working on files.
### Basic Structure
* pattern { action }
* Two special patterns (keyword)
    - BEGIN before any line are read.
    - END last line is read.
* Field select
    - syntax: $x
    - limit: 99 fields per line.
    - $0 is hold line.
* Quote is just a switch
### Built-in Variables
* FS: Input field separator variable
* OFS: Output field separator variable
* NF: Number of fields variable
* NR: Number of records variable
* RS: Record separator variable
* ORS: Output record separator variable
* FILENAME: Current filename variable
### Expressions
* Arithmetic
* Conditional
* Regular expressions
* Boolean
### Commands
Very few commands: if, while, for, break, continue, assignment, print, printf, next,quit
### Associative arrays
Compare to array of other languages

## Example
* Use sed || awk to filter 404 log Apache
    - Select only request's path, HTTP method and agent
    - Count total access
* Sum up an field from a csv file
* Delete line:
    - Eliminate user with no password from passwd

