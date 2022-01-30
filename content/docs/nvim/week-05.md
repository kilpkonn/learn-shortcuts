---
weight: 1
bookFlatSection: false
title: "Week 5"
---

# Opening files
More tips for opening files incoming.


## Open multiple files from inside vim
Similarly to passing wildcards to arguments when opening vim with files you can open multiple files from inside vim.
This can be acieved with `:ar[gs] <pattern>` command.

For example all `.cpp` files is src can be opened with
```vim
:args src/**/*.cpp
```

## Nvim Tree
Another very useful option is to use [kyazdani42/nvim-tree](https://github.com/kyazdani42/nvim-tree.lua) _(or something similar)_.
Some keymappings inside `nvim-tree`.
```vim
x - cut
c - copy
p - paste
y - copy name
<C-V> - open file in vertical split
H - toggle visibility of dotfiles
..and more
```

## Telescope
Telescope is also very useful when opening files with either `find_files` or `live_grep`.
Find files is fuzzy finder for files whilst live grep is for searching file by it's context _(fuzzy finder for text)_.
My mappings for them
```vim
<Leader>ff - find_files
<Leader>fw - live_grep
```
