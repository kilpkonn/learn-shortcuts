---
weight: 1
bookFlatSection: false
title: "Week 48"
---

# Copying in command line mode
Sometimes we want to paste something from current buffer to the command line mode (accessed with `:`)
The boring way to do it is go back to normal mode, yank it and then paste it with `C-r<reg>`.
However there are some handy shortcuts for it.

# Most useful shortcuts
- `C-r C-f` Copy the `f`ilename under buffer cursor
- `C-r C-w` Copy the `w`ord under buffer cursor
- `C-r C-a` Copy the `a`round word under buffer cursor
- `C-r C-l` Copy the `l`ine under buffer cursor
