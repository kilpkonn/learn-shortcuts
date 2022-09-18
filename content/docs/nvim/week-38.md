---
weight: 1
bookFlatSection: false
title: "Week 38"
---

# Substitute magic
Vim has a regex engine that has some so-called magic features.
Here's how to use or not to use them.

## Enabling different levels of magic
```vim
\v - very magic
:sm - substitute magic
:sno - no magic
\V - very no magic
```
These all delete opening brackets:
```vim
:%s/\V(/
:%sm/(/
:%s/\(/
```
