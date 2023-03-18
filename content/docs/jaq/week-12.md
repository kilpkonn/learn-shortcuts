---
weight: 1
bookFlatSection: false
title: "Week 12"
---

# Function `length`
The `length` function is one of the basic functions in `jq`.
It works pretty much as expected, but there are some points to bring out just to be sure.
- Length of string is amount of characters
- Length of array is amount of elements
- Length of object is amount of key-value pairs
- Length of `null` is 0


## Examples
Input
```json
[[1,2], "string", {"a":2}, null]
```
Query
```jq
jq '.[] | length'  -> 2, 6, 1, 0
```
