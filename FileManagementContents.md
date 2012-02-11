# File Management Contents

## Copy, move

* cp, mv, rm: using man page.
* Notes: be careful with the slash ("/")
* Some common use cases

## Setting file permission

* chmod: change permission bit(s) of file(s)
  - 2 common ways to specify permission:
    + use octal value(s)
    + use symbolic representation
  - setuid, setgid and sticky bit

* chgrp: change group owner of file(s)
* chown: change owner of file(s)

* Common options:
  - -R, --recursive: recursive
  - -v, --verbose: verbose

## Searching via name and contents

* find: find by name, path
  - Cons: slow
  - Pros: convenient, no indexing time

* locate: find by name, path
  - Cons: faster than find
  - Pros: must have database, create and update using "updatedb" (usually run
    by a cron daemon)

* grep: find by contents, using regular expression
  - Regular expression: A regular expression is a pattern that provides a
    concise and flexible means for "matching" strings of text:
    + Character classes, bracket expression
    + Anchoring
    + Backslash character and special expressions
    + Repetition
    + Concatenation, alternation,...

* find and locate can use regular expression using `-regex`
