---
weight: 1
bookFlatSection: false
title: "Week 14"
---

# QuickFix lists
Whilst the name seems new, some of QuickFix lists usecases are quite common.
r example it is used when vimgrepping a pattern and then jumping between entries found.
Local QuickFix lists can be used for code errors and warnings.

## Viewving and navigating QuickFix list
QuickFix list can be viewed with `:copen` or `:lopen` command depending on if you want global or local list.
Navigation can be done with `:cnext` and `:cprev` or `:lnext` and `:lprev` respectively.


## Run command on all entries
Commands `:cdo` and `:ldo` allow running commands on all entries of the list.
An example to transform `TODO:` into `TODO(foo):`
```vim
:vimgrep TODO: %
:cdo s/TODO:/TODO(foo):/g
```

## Populating QuickFix list with Telescope
One way to populate quickfix list is to use `Telescope` plugin.
```vim
<C-q> - Send all not filtered items to QuickFix list
<M-q> - Send all items to QuickFix list
```

