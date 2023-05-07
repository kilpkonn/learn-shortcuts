---
weight: 1
bookFlatSection: false
title: "Week 19"
---

# Function `select(boolean_expression)`
The function `select(foo)` produces its input unchanged if `foo` returns `true` for that input, and produces no output otherwise.

It's useful for filtering lists: `[1,2,3] | map(select(. >= 2))` will give you `[2,3]`.

## Examples
Input
```json
[1, 5, 3, 0, 7]
```
Query
```jq
jq 'map(select(. >= 2))'   # -->[5,3,7] 
```

