---
weight: 1
bookFlatSection: false
title: "Week 15"
---

# Function `path(path_expression)`
Outputs array representations of the given path expression in `..`.
The outputs are arrays of strings (object keys) and/or numbers (array indices).

Path expressions are `jq` expressions like `.a`, but also `.[]`.
There are two types of path expressions: ones that can match exactly, and ones that cannot. 
For example, `.a.b.c` is an exact match path expression, while `.a[].b` is not.

`path(exact_path_expression)` will produce the array representation of the path expression even if it does not exist in `.`, if `.` is null or an array or an object.

`path(pattern)` will produce array representations of the paths matching pattern if the paths exist in `..`.

Note that the path expressions are not different from normal expressions.
The expression `path(..|select(type=="boolean"))` outputs all the paths to boolean values in `.`, and only those paths.

## Examples
Input
```json
null
```
Query
```jq
jq 'path(.a[0].b)'  ->   ["a", 0, "b"] 
```

Input
```json
{ "a": [{ "b": 1 }] }
```
Query
```jq
jq '[path(..)]'  ->  [[], ["a"], ["a",0], ["a",0,"b"]] 
```
