---
weight: 1
bookFlatSection: false
title: "Week 0"
---

# Starting point

_This is a short chapter to describe starting point._  

Before starting you should have:
- basic experience with neovim (I had ~5 months as neovim as my main editor but also less is sufficient for sure)
- know basic movement, editing and similar in vim.
- know very basics of lua _(for config)_

## Some random tips
Make neovim your default editor
```bash
# .zshenv
export EDITOR="nvim"
```

Add alias to launch neovim faster
```bash
# .zshrc
alias v="nvim"
```

Edit terminal command in vim with `C-e` (`zsh` specific)
```bash
# .zshrc
autoload edit-command-line; zle -N edit-command-line
bindkey '^e' edit-command-line
```
