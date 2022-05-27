---
weight: 1
bookFlatSection: false
title: "Week 21"
---

# Incremental selection
Most ides support incremental selection of some sort.
You can start from single function argument, then select all arguments, whole line etc. and then up to whole file.
Same is possible using treesitter

## Setup
To enable incremential selection, following snippet can be used:
```lua
require'nvim-treesitter.configs'.setup {
  incremental_selection = {
    enable = true,
    keymaps = {
      init_selection = "gnn",
      node_incremental = "grn",
      scope_incremental = "grc",
      node_decremental = "grm",
    },
  },
}
```

## Usage
Now you are pretty much good to go :D
As you can see above, `gnn` can be used to init selection.
`grn` and `grm` can be used to increment and decrement the selection so they are likely the most useful commands.
`grc` selects whole scope, which I'm not quite sure what exactly is, but it seems to be whole file etc.
