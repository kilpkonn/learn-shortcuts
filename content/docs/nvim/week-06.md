---
weight: 1
bookFlatSection: false
title: "Week 6"
---

# Macros
It is quite often that we want to repeat some combination of actions multiple times...
And thats exactly what macros are for :D.


## Recording a macro
Recording macro is started with pressing `q` in normal mode followed by macro name _(any lowercase letter)_.
Recording macro can be stopped with pressing `q` again.
```vim
qa  # Record macro named "a"
# perform actions
q
```

## Playing macros
Macro can me played with `@{macro-name}`. It is also possible to specify how many times the macro should be run.
```vim
@a    # Run macro "a"
10@a  # Run macro "a" 10 times
```
