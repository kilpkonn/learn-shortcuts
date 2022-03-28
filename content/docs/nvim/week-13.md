---
weight: 1
bookFlatSection: false
title: "Week 13"
---

# Buffers
Vim buffers are something you can think of as opened files.
Some of them are readonly and do not correspond to actual files (eg. Nvimtree),
but it still is something that makes thinking of them easier.

A buffer can be opened in multiple windows in which case if you edit it in one window, the changes also appear in the other.

## Basic commands
You can view the contents of buffers with `:buffers` or `:ls`.
The ouput of the command is:
```vim
:ls
<nr> <mark><info> <unsaved> <name> line <line nr>
```

## Switching buffers
Here are some commands to move between buffers
```vim
:bp - go to previous buffer
:bn - go to next buffer
:b<nr> - jump to buffer by number
<C-6> - jump between current and alternate buffer
```

## Closing buffers
```vim
:bd - Delete buffer
:bw - Wipe buffer, deletes everything related to it 
```

