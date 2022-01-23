---
weight: 1
bookFlatSection: false
title: "Week 3"
---

# Working on long lines
Sometimes lines are so long that they do not fit onto screen.
It is inportant to know how to split line to multiple or sometimes merge into single in these cases.


## Movement
This is how to move on wrapped lines as if they were multiple lines
```vim
gj - down
gk - up
g$ - end of a visual line
g0 - beginning of a visual line
```

## Split to multiple lines
To split single line (or any other text object) to multiple lines `gq` followed by a motion can be used.
For example splitting current lines can be done with `gqq`.

## Merge lines
The opposite of split would be merge lines and it can be done with `J` command.
To avoid adding space in between `gJ` can be used.

## Capitalization
You can also performa capitalization on the whole line (or any other text object) at once.
```vim
gu - uncapitalize
gU - capitalize
g~ - flip capitalization
```
For exaple `gu$` uncapitalizes till end of the line.

## Reselect last selection
To reselect last selection `gv` can be used.
