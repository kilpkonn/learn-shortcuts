---
weight: 1
bookFlatSection: false
title: "Week 15"
---

# Makeprg
A big part of programming is compiling files and running them.
Whilst editing parts of code usually it is a good idea to sometimes build the project to see if everything works fine.
This can be done also in vim without exiting it.

## Make and makeprg
To build a program you can run `:make`.
As You might have guessed the default build system is GNU Make.
However you can use different build systems via `:set makeprg`.
Example to build current file with gcc _(`\` is to escape space)_.
```vim
:set makeprg=gcc\ %
```
{{< hint info >}}
**Note:** You can also run it instantly by chaining run command
{{< /hint >}}

## Local make
Running `:make` polulates QuickFix list with errors.
To use local list instead `:lmake` command can be used instead.
Otherwise it acts as `:make`.

## Error format
One benefit of using `:make` rather than shelling out is that you can automatically jump between build errors.
For that you need to `:set errorformat`
An example for rust would be
```vim
let &efm=''
let &efm .= '%Eerror%m,'
let &efm .= '%Wwarning: %m,'
let &efm .= '%-Z%*\s--> %f:%l:%c,'
```
Note that this can become quite complex for some compilers so it might be a good idea to set it in `ftplugin` automatically
rather than typing it in every time.

