---
weight: 1
bookFlatSection: false
title: "Week 16"
---

# Function `del(path_expression)`
The builtin function `del` removes a key and its corresponding value from an object.

## Examples
Input
```json
{ "foo": 42, "bar": 9001, "baz": 42 }
```
Query
```jq
jq 'del(.foo)'   # --> {"bar": 9001, "baz": 42}
```

