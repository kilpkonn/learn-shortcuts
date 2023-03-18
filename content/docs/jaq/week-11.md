---
weight: 1
bookFlatSection: false
title: "Week 11"
---

# Multiplication (`*`), division (`/`), modulo (`%`) 
All these infix operators work as you'd expect with numbers.
Only thing to note is that dividing with 0 gives error.

Multiplying string works as in python (repeats string n times).

Dividing string by another string splits first string using the second string as a separator.

Multiplying objects merges them recursively, so it works similarly to addition, but if both objects contain the same key and values are objects, then they get merged.


## Examples
Input
```json
"a, b,c,d, e"
```
Query
```jq
jq '. / ", "'  -> ["a","b,c,d","e"]
```
