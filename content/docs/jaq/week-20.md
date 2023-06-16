---
weight: 1
bookFlatSection: false
title: "Week 20"
---

# Function / value `empty`
`empty` returns no results. None at all. Not even `null`.

It's useful on occasion. You'll know if you need it :)


## Examples
Input
```json
null
```
Query
```jq
jq '[1,2,empty,3]'   # --> [1,2,3] 
```

