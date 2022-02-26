---
weight: 1
bookFlatSection: false
title: "Week 9"
---

# Registers 2
We continue with registers by looking at:
1. Three read-only registers `".`, `"%`, `:`
2. Alternate file register `"#`
3. The expression register `"=`


## Readonly registers
- `".` Last insert mode
- `"%` Current file name
- `":` Last Command

**Some tips to go with current filename:**
```vim
%:p -> Make filename full path
%:h -> Head of the filename
%:t -> Tail of the filename
%:r -> Root
%:e -> Extension
```

## Alternate file register
Register can be accessed via `"#`.
Always contains the filename of the last file you were at.
You can quicly switch to last file with `<C-^>`
Otherwise works similraly to current file reg.

## The expression register
Can be accessed via `"=`.
You can do math and system calls and then paste.

Examples:
```vim
=123 * 456
=system('ls ')
```

