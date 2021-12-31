
---
weight: 1
bookFlatSection: false
title: "Week 1"
---

# Replace in range
Sometimes we wish to replace strings only in some range, not at file at a time.
Here are some tims to accomplish that.

## Replace in visually seleceted range
1) Select range in visual mode
2) Press `<:>` to start range action, you should see something like this:
```vim
:'<,'>
```
3) Type in replace command as usual eg. for foo -> bar
```vim
:'<,'>s/foo/bar/g
```

## Replace last visually selected range in normal mode
1) Select range in visual mode
2) Exit to normal mode
3) Start command with `<:>` as usual
4) Use `\%V` to restrict selection to previously selected visual range.
5) Replace usual eg. for foo -> bar
```vim
:%s/\%Vfoo/bar/g
```

## Replace multiple ranges
You can also select range in command mode with `:start,end` and run command on it.
You can then also chain renaming in multiple ranges like so
```vim
:18,20s/foo/bar/g | 28,30&&
```

