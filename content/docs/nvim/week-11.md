---
weight: 1
bookFlatSection: false
title: "Week 11"
---

# Vim Marks
Marks allow storying corrent location and returning to it later.
There are generally 3 types of marks lowercase marks, uppercase marks and special marks.
Marks can be added with `m<letter>` in normal mode for example `ma`.
The mark stores both the line and column information.


## Lowercase marks
These are marks for `a-z`.
Lowercase marks are local to a file meaning multiple files can have say mark `'a`.

{{< hint warning >}}
**Note:** You can only jump to lowercase marks whilst in the same file. 
{{< /hint >}}

## Uppercase marks
These are marks from `A-Z`.
Uppercase marks are global meaning there can be only one mark `'A`.
These can be really useful for returning to some place after moving around in multiple files.

## Using marks
```vim
ma - Add mark `a`
'a - Jump to line of mark (first nonblank character)
`a - Jump to position of mark (line and column)
d'a - Delete from current line to line of mark `a`
d`a - Delete from current position to position of mark `a`
c'a - Change text from current line to line of mark `a`
:marks - List all marks
:marks aB - List marks `a` and `B` 
```

{{< hint info >}}
Commands like `d'a` operate linewise and include start and end lines but commands like
``d`a`` operate characterwise and include start but not the end character.
{{< /hint >}}


