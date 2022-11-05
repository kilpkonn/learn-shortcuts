---
weight: 1
bookFlatSection: false
title: "Week 44"
---

# External commands
Vim has also an easy interface to run external (shell) commands from within vim.
Some of it is quite basic but it has also some small useful tips not used so often.

# Usage
`:! <cmd>` executes the shell command `<cmd>`.  
`:!!` repeats the last executed command.

To insert the output of the command into current buffer you can use `:read! <cmd>` or `:!r <cmd>` for short form.
And if you were wondering, `:r!!` also works fine.
