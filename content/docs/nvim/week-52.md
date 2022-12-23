---
weight: 1
bookFlatSection: false
title: "Week 52"
---

# Saving options to a file
Usually you have hand written config fir your vim, but it might be that sometimes you want to save your current settings to a file.
And vim has a command for that...

# Basic usage
You can save all your mappings and options to a file with `:mk[exrc] <file>`.
The options can be later loaded with `:source` command.

If you wish to save more than just options and mappings you can use `mks[ession] <file>` command that
saves current session (tabs, buffer, pwd, ..) to a file.
Option called `sessionoptions` specifies what exactly is saved.
Loading sessions is also done with `:source` command
