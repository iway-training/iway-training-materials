# File management
## Copy, move
cp, mv, rm: using man page
Notice: end with or without backslash
## Setting file permission
* chmod: change mode bit(s) of file(s)
    - 2 ways to specify permission:
	+ use octal value (octal mode)
	+ use symbolic (symbolic mode)
    - setuid, setgid and sticky bit
* chgrp: change group of file(s)
* chown: change owner of file(s)
* common option:
    - -R, --recursive: recursive apply command
    - -v, --verbose: verbose
## Searching via name and contents
* find: find by name, path
    - disadvantage: slow
    - advantage: doesn't need database
* locate: find by name, path
    - advantage: faster than find
    - disadvantage: must have database, create and update using "updatedb", ussually update use cron
* grep: find by content, using regular expression
    - regular expression:
    A regular expression is a pattern that describe a set of string
    Some concept:
	+ Chracter classes, bracket expression
	+ Anchoring
	+ Backslash character and special expressions
	+ Repetition
	+ Concatenation, alternation,...
* find and locate can use regular expression using -regex
