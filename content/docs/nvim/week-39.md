---
weight: 1
bookFlatSection: false
title: "Week 39"
---

# Repeating substitutions
Instead of doing substitution on the whole file and reverting if it goes wrong there is a better way to
test out you substitutions.

## Repeat same substitution
To repeat the last substitution with its flags use the `:&&` command.

## Repeat the substitution with new pattern
To redo the substitution with a new pattern (same replacement) you can use
the `:-` command. 
Typical solution would be
```vim
:s/pattern/replacement/
/new
:~
```
In the sequence above the occurances of `new` get replaced with `replacement`.

## More tips
- `:&` Repeats last substitution with its falgs but without its range
- `:g&` Repeats last substitution with its flags and global range. Also replaces search pattern with latest search pattern used.
