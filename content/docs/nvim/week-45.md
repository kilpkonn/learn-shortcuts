---
weight: 1
bookFlatSection: false
title: "Week 45"
---

# Virtual edit
While editing text normally, you cannot type characters in a random place in the window.
You need to manually add spaces or tabs to type text to the right side of the buffer.
However there is a way to tell vim to allow placing cursor everywhere and then add spaces wherever needed if something was inserted.

# Usage
`:set virtualedit=all` allows you to type everywhere on the screen.  
`:set virtualedit=onemore` allows you to type one extra character on the right.
