---
weight: 1
bookFlatSection: false
title: "Week 12"
---

# More on Marks
We learned some basics of vim marks last week.
Now we can take a look at some more advanced commands.


## Movement
Here are some more options to move around marks.
```vim
]' - jump to next line with a lowercase mark
[' - jump to previous line with a lowercase mark
]` - jump to next lowercase mark
[` - jump to previous lowercase mark
```
{{< hint info >}}
**Note:** You can use count with all the commands above, for example `5['` works.
{{< /hint >}}

## Special marks
Here are some special marks from vim that can be useful.
```vim
`. - Jump to position of last change in buffer
`" - Jump to position where last exited current buffer
`0 - Jump to position in last file edited (Also other numbers)
'' - Jump back (to line before last jump)
`` - Jump back (to position before last jump)
`[ or `] Jump to beginning / end of previously yanked text
`< or `> Jump to beginning / end of last visual selection
```

## Deleting marks
Sometimes you also want to delete marks.
This can be done with `:delmarks`.
```vim
:delmarks a - deletes a
:delmarks a-d - deletes a,b,c,d
:delmarks ax - deletes a,x
:delmarks! - deletes all lowercase marks
```

