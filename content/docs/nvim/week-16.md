---
weight: 1
bookFlatSection: false
title: "Week 16"
---

# Compiler plugins
Compiler plugins are something that allow automating steps described in previous week.
You can pretty much set the `:makeprg` and `:efm` based on filetype.

## Writing plugin
Compiler plugins are stored in `compiler/` subdirecotory so `~/.config/nvim/compiler/` for nvim.
You can write them both in vim and lua.

Example plugin written in vim:
```vim
if exists("current_compiler") | finish | endif " Needed to avoid running multiple times
let current_compiler = "zsh"

if exists(":CompilerSet") != 2		" older Vim always used :setlocal
  command -nargs=* CompilerSet setlocal <args>
endif

CompilerSet makeprg=zsh\ -n
CompilerSet errorformat=%f:\ line\ %l:\ %m
```
{{< hint info >}}
**Note:** You can also write compiler plugins in lua, however I didn't manage to find any good examples.
{{< /hint >}}

## Setting compiler
You can set compiler with `:compiler <name>`.
To automate it you can easily move setting it automatically to `ftplugin`.

