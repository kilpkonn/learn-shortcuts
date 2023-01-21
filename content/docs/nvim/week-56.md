---
weight: 1
bookFlatSection: false
title: "Week 56"
---

# Operator pending mode
Once you start deleting, yanking or changing text vim enters `OPERATOR PENDING MODE` which then waits for textobject to come in.
There is also a way to define mapping for this mode with `:omap`.

## Example
Here is an example to select everything on the line within next curly braces.
```vim
:onoremap nc :normal! f{vi{<cr>
```
