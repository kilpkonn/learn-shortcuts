---
weight: 1
bookFlatSection: false
title: "Week 50"
---

# Running multiple commands in CLI mode
Sometimes it is useful to run multiple commands one after another in CLI mode.
An example would be replacing text with `:argdo` and then following it up with write.

# Basic usage
Commands can be chained with `|` symbol.
So the example above would become
```vim
:argdo s/foo/bar/g | w
```

{{< hint danger >}}
**Note:** You cannot use it with commands that take pipe as input. `:!ls | ...` won't work.
{{< /hint >}}
