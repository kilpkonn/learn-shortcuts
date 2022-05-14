---
weight: 1
bookFlatSection: false
title: "Week 20"
---

# Folds
In all kinds of IDEs folds are quite common.
You can fold all kinds of long functions or even bunch of vars to make your spagetti code easier to read.
Folds also do exist in vim, and here are some examples for it.

## Folding lines
To fold lines `zF` command can be used followed by a motion.
Folds can also be created in command mode with
```vim
:{range}fo[ld]
```

## Deleting folds
Folds can be ledeted with `zd` or with `zD` to delete folds recursively.

{{< hint info >}}
**Note:** Note that deleting folds does not delete text, but only fold markers.
{{< /hint >}}

## Opening and closing folds
Folds can be opened with `zo` and closed with `zc`, but there is also an onption `za` which will toggle fold.
To operate on folds recursively `zO`, `zC` and `zA` can be used.

## Opening and closing multiple folds
To open or close all folds in a file `zr` and `zm` commands can be used.
They also operate on one level of folds and have `zR` and `zM` as a counterparts to open or close folds recursively.
