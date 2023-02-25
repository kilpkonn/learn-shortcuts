---
weight: 1
bookFlatSection: false
title: "Week 9"
---

# Recursive descent `..`
Recursively descends `.`, producing every value.
For `[1, 2]` this is `[[1, 2], 1, 2]`.

## Useful tips
Note that `..a` does not work so you should use `..|.a` to get all values for key `a`.

## Examples
Input
```json
[{"a": true, "b": false}, 1]
```
Query
```jq
..|.a?    -> true
```
