---
weight: 1
bookFlatSection: false
title: "Week 10"
---

# Registers 3
We finish with registers by looking at:
1. Black hole register
2. Last selection register
3. Last search register


## The black hole register
- `"_` <- the name
- When writing to it, nothing happens
- Can be used to delete text without affecting other registers
- Reading it returns nothing
- Can be used for clearing other registers

## Last selection registers
Keys: `"+` and `"*`
Useful for operating with system clipboard.
In case you do not like it you can use the clipboard for all operations
```vim
set clipboard+=unnamedplus
```

## The last search register
Key: `"/`
In inser/search mode int can be accessed with `<C-r>/`  
Mostly useful for correcting searces and later using previous search for replace etc.

