---
weight: 1
bookFlatSection: false
title: "Week 24"
---

# Aligning text
A simple, but sometimes boring and slow task is alagning text.
However it is also quite common task in programming, wheather fore readme or for printing to terminal.

## Aligning to columns
One of the most common tasks is algining text to columns.
It can be easily achieved using linux `column` command.
```vim
:'<,'>! column -t
```

## Centering text
There is also a command in vim for centering text.
```vim
:'<,'>center 30
```
