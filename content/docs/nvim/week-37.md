---
weight: 1
bookFlatSection: false
title: "Week 37"
---

# Ranges
Ranges are useful for performing action over a range of text.
Whether it is adding some text, deleting or performing any other action, they can still be used.
Here are some tips to use specify rangfes with the least amount of hustle.

## Basic syntax
The range in vim consists of starting position and ending position.
Quite common is to use line numbers for them so the syntax looks something like `1,30` to create range over first 30 lines.  
**Note that the indexing starts from 1!**

## Special delimiters for range
Here are some more special delimiters that can be used for specifying range.
- `.` - Represents the current line
- `$` - Represents last line of current buffer
- `%` - Represents entire file
- `*` - Represents last selection made in visual mode
- `'<` - Represents start of last visual selection
- `'>` - Represents end of last visual selection

An example to select everything from current line till end of last visual selection would be
```vim
.,'>
```
