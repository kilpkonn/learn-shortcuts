---
weight: 1
bookFlatSection: false
title: "Week 14"
---

# Functions `has(key)` and `in`
The builtin function `has(key)` returns whether the input object has the given key, or the input array has an element at the given index.
The function has the same effect as checking whether the `key` is in array of keys returned by the function `keys`, but it works faster.

The builtin function `in` in returns whether or not the input key is in the given object, or the input index corresponds to an element in the given array. It is, essentially, an inversed version of `has(key`).

## Examples
Input
```json
[{ "foo": 42 }, {}]
```
Query
```jq
jq 'map(has("foo"))'  -> 	[true, false] 
```

Input
```json
["foo", "bar"]
```
Query
```jq
jq '.[] | in({"foo": 42})'  ->  true, false 
```
