---
weight: 1
bookFlatSection: false
title: "Week 8"
---

# Registers 1
We continue with registers by looking atÖ
1. 10 numbered registers `"0..9`
2. The small delete register `"-`
3. 26 named registers `"a..z`


## Numbered registers
- `"0` has the last yank
- `"1` has the last delete (`d`, `c`, `s`, `x`)
- `"2..9` have previous deletes


{{< hint danger >}}
**Side note**  
Note that `%`, `()`, `/`, `n` and `N` (and maybe some more) dont got to delete registers.
{{< /hint >}}

## Small delete register
This register contains the deletes that delete less than one line.
This is also somewhat confusing register as some commands don't put stuff there while others do.
_Don't have any good usecase, but never know :D_

## Named registers
- Store whatever you want
- Macros are stored here automatically
- You can edit macros by editing contents of these registers
- 

Edit macro a with:
```vim
let @a='<macro>'
```
_Use `<C-r>a` to access previous macro from `"a` register in insert mode._
