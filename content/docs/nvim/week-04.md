---
weight: 1
bookFlatSection: false
title: "Week 4"
---

# Opening files
Here are some tips for opening files with vim.


## Open file with nvim
The most basic way is to open files when opening vim.
```bash
nvim [-o] /path/to/file.txt
```
`-o` Can be used to open each file in sepparate window or you can specify amount of windows with it as `-o 4`

## Open width :edit / :view command
To edit
```vim
:e /path/to/file.txt
```

View only mode
```vim
:v /path/to/file.txt
```

## Open path in buffer
Sometimes you have some paths in you text document and you want to open them.
For that you can simply do `gf` on the path to open it.
