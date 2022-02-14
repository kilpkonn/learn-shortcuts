---
weight: 1
bookFlatSection: false
title: "Week 7"
---

# Registers
Sometomes you copy a thing.. and then you copy another thing.. but now you want to paste the first one.
This is what vim registers are for :D


## Different types of registers
1. Unnamed register `""`
2. 10 numbered registers `"0..9`
3. The small delete register `"-`
4. 26 named registers `"a..z`
5. Three read-only registers `".`, `"%`, `:`
6. Alternate buffer register `"#`
7. The expression register `"=`
8. The black hole register `"_`
9. The last selection registers `"*` and `"+`
10. Last search pattern register `"/`

## Viewing registers
Show all registers
```vim
:registers
# Or simply..
:reg
```
Show specific register
```vim
:reg <register>
```

## Accessing registers

**Normal mode**
```v
"<reg> <action>

"0p  # Paste from register "0
```

**Insert mode**
```vim
<C-r> <reg> <action>
```

## Unnamed register
Yank, delete, substitute and similar commands already use the unnamed register.
The unnamed register acts as a default so there is no need to specify it via `""`.
In other words `""yy` and `yy` both yank line to unnamed register.

<br>

{{< hint info >}}
**Side note**  
Make sure to check out https://www.youtube.com/watch?v=I5QGlfbuCfs for more detailed description!
{{< /hint >}}

