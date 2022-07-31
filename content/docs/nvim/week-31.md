---
weight: 1
bookFlatSection: false
title: "Week 31"
---

# Undo in insert mode
In inser mode we insert text and later we can undo those changes with `u` key in normal mode.
However undo to whole update is not what we always want and vim might not be always clever enough to understand what should be considere 
atomic edit. 
To solve that there is an option to tell where an atomic edit should end.

## Splitting insert to multiple atoms
To split a single edit to multiple atoms use `<C-G>u` shortcut.
Now you can undo everything you inserted after it without losing what was written before.
