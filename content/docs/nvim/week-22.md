---
weight: 1
bookFlatSection: false
title: "Week 22"
---

# Moving lines around
Moving lines can be thought of as deleting and pasting lines.
However sometimes it is easier to think of it as pushing selected part up or down.
For that vim has `:m` command.

## The move command
The move command is quite easy to use.
To move a line, first you have to place cursor at it or select it in visual mode.
After that you can do `:m <nr>` to move line to line `<nr>`.
Also relative numbers can be used to move lines around.
Simly use `:m +1<CR>` to move line down or `:m -2<CR>` to move line up.

## The copy command
Similarly to `:m[ove]` command vim has `:co[py]` command that works in a similary manner,
but instead of moving lines it copies them.
Copy also doesn't play nice with relative line numbers.
