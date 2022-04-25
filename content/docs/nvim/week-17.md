---
weight: 1
bookFlatSection: false
title: "Week 17"
---

# Set and let
Since day one, everybody know vim has `:set` command to set options.
There also seems to be a `:let` command which in a way is similar, but it's also quite different.

## Set command
Set is command for setting vim options.
Here are some things you can do with it.

```vim
:verbose set "show all options
:set tw=40 "set option (text width to 40)
:set wrap& "set default option (to wrap)
:set nowrap "unset option
:set wrap! "toggle option
:set wrap? "show current value
```

## Let command
Let works similarly to set.
It allows setting options, but it is more powerful as it also allows setting registers etc.
However, it is generally harder to use than `:set`.

```vim
let &tw = 40 "set tw option to 40
let vi = 'vim' "set variable
let @a = $HOME . '/git' "set register value
let $ENVVAR = 'some_var' "set environment variable
```

## Misc
You can set multiple options at once with:
```vim
:set et sw=4 sts=4 
```
There is also way to set multiple items at once with let:
```vim
:let [&et, &sw, &sts] = [0, 4, 4]
```

{{< hint warning >}}
**Note:** Right side of `:let` is expression, but right side of `:set` is value.
In other words: `:let &tw = 40 + 60` is legit, but `:set tw=40+60` is not.
{{< /hint >}}

{{< hint info >}}
**Note:** Note that tab comletion works with both
{{< /hint >}}
