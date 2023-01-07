---
weight: 1
bookFlatSection: false
title: "Week 54"
---

# Filtering command output
Vim has built in command `:filter` to filter command output so you wouldn't have to use `grep` etc. for it.

# Basic usage
The basic usage is `:filter /pattern/ <cmd>`

## Example
Here is an example to show only buffers that have "content" in them.
```vim
:filter /content/ buffers
```
