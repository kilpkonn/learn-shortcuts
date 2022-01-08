---
weight: 1
bookFlatSection: false
title: "Week 2"
---

# The 'g' command
It is quite common to wish to run some specific command on every line containing a pattern.
This is exactly what the 'g' command is for.

## Syntax
The 'g' command is executed in command mode and the syntax is following:
```vim
:g/pattern/command
```
Also the inverse is possible (run command on lines that do not match)
```vim
:g!/pattern/command
```
or
```vim
:v/pattern/command
```

## Examples

### Delete all lines containing pattern
```vim
:g/foo/d
```

### Delete all empty lines
```vim
:g/^\s*$/d
```

### Move imports to start of file
```vim
:g/import/m0
```

### Capitalize all lines not containig bar
```vim
:v/bar/normal gUU
```
