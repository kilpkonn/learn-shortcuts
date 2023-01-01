---
weight: 1
bookFlatSection: false
title: "Week 53"
---

# Redirections
What if you want to save the output of Vim commands in a file or in a register? The command `:redir` is here to fulfill your desires.

# Basic usage
- `:redir > <file>` - Write commands output to a file. Use `>>` to append and `:redir!` to overwrite.
- `:redir @<reg>` - Write every commands output to  the register.
- `:redir @<reg>>>` - Append every commands output to register. (Caps append as well)
- `:redir => <var>` - Write every commands output to a variable.
- `:redir END` - End redirections

## Example
Here is an example to save `sessionoptions` to `.vimrc`.
```vim
:redir >> $VIMCONFIG/.vimrc
:set sessionoptions?
:redir END
```

