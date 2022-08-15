---
weight: 1
bookFlatSection: false
title: "Week 33"
---

# Opening links in other apps
Text files often contain links to either files or web pages.
It is also quite common that you want to open those links
with an app that you have installed for particular meme type.

## The `gx` command
Vim has a `gx` command to open links with default app configured in your system.
It can be used in a similar manner to `gf`.
Simply place your cursor on the link and press `gx`.
It can open web URLs, image files, videos etc.

{{< hint warning >}}
**Note:** You need to have `netrw` plugin enabled in vim for `gx` command to work.
{{< /hint >}}
