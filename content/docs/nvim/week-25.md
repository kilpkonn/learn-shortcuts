---
weight: 1
bookFlatSection: false
title: "Week 25"
---

# Aligning text
This week we're simply continuing with aligning text.

## Aligning left or right
Aigning text to left or right can be achieved with `:left` and `:right`.
Make sure to also set correct `textwidth` so that aligning right would make sense.

## Aligning by character
As a followup to last week I also decided to add option to align by char.
For that you can use
```vim
:% ! column -t -s= -o=
```
The example above aligns by `=` character.
