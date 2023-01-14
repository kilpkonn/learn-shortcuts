---
weight: 1
bookFlatSection: false
title: "Week 55"
---

# Verbose commands
Vim has `:verbose` command to give more precise information about
- Abbreviations
- Options
- Mappings
- User commands

# Basic usage
The basic usage is `:filter /pattern/ <cmd>`

## Example
Here is an example to see where `mouse` option was set from.
```vim
:verbose set mouse?
```
