---
weight: 1
bookFlatSection: false
title: "Week 42"
---

# Zero-with lookaround
Zero-with lookaround assertions allow regex to match patterns looking forward or backward without actually including them in the match.
Since they do dot have with, replacing them is actually inserting text.
Simple example are `^` and `$` characters.

# Useful examples
- `\zs` - Only match your pattern if what’s before the metacharacter `\zs` has a match
- `\ze` - Only match your pattern if what’s after the metacharacter `\ze` has a match
- `\<` - Match beginning of a word
- `\>` - Match end of a word
- `\%^` - Match beginning of a file
- `\%$` - Match end of a file
- `\%V` - Match only in last visual selection

