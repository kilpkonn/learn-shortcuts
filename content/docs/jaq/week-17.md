---
weight: 1
bookFlatSection: false
title: "Week 17"
---

# Function `getpath(PATHS)`
The builtin function `getpath` outputs the values in `.` found at each path in `PATHS`.

## Examples
Input
```json
{ "a": {"b":0, "c":1} }
```
Query
```jq
jq '[getpath(["a","b"], ["a","c"])]'   # --> [0, 1]
```

# Function `setpath(PATHS; value)`
The builtin function `setpath `sets the `PATHS` in `.` to `VALUE`.
If there is no value to update, new value is inserted.

## Examples
Input
```json
{ "a": {"b":0} }
```
Query
```jq
jq 'setpath(["a","b"]; 1)'   # --> {"a": {"b": 1}} 
```
