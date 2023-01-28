---
weight: 1
bookFlatSection: false
title: "Week 57"
---

# Autocommands
Autocommands are definitely something you have heard of, but maybe not tried yourself yet.
Here's how they work :D

## Basic syntax
The basic syntax is following:
```vim
:au[tocmd] <event> <pattern> <cmd>
```
- `<event>` is event you wish to hook into (such as `BufRead`)
- `<pattern>` is regex pattern to filter files where to append the autocommand (use * for everywhere)
- `<cnd>` is the command to execute

{{< hint info >}}
**Note:** You can specify multiple events or patterns by separating them with commas.
For example `:au BufRead,BufWrite *.md,*.txt <cmd>`.
{{< /hint >}}

## Viewing autocommands
To view the autocommands created for `<event>` use
```vim
:au[tocmd] <event>
```

## Deleting autocommands
To delete all atocommands for `<event>` use
```vim
:au[tocmd]! <event>
```

