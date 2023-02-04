---
weight: 1
bookFlatSection: false
title: "Week 58"
---

# Autocommand groups
Autocommand groups are something like a namespaces for autocommands.
If you don't specify group, the autocommand is added automatically to default autocommand group without a name.
But there are several reasons why it can be useful to specify custom autocommand groups.

## Basic syntax
The basic syntax is following:
```vim
:augroup <name>
:au <event> <pattern> <cmd>
...
:augroup END
```
{{< hint error >}}
**Note:** You can add same autocommand to group multiple times so watch out for it :p
Common fix to the problem is to delete all the commands in group with `:au! <name>` (or `:au!` if inside group) and then readding them.
{{< /hint >}}

## Viewing autocommands
To view the autocommand groups use
```vim
:augroup
```

## Deleting autocommands
To delete autocommand group `<name>` use
```vim
:augroup! <name>
```

