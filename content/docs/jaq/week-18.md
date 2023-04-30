---
weight: 1
bookFlatSection: false
title: "Week 18"
---

# Functions ` to_entries`, `from_entries`, `with_entries`
These functions convert between an object and an array of key-value pairs.
If `to_entries` is passed an object, then for each `k: v` entry in the input, the output array includes `{"key": k, "value": v}`.

`from_entries` does the opposite conversion, and `with_entries(foo)` is a shorthand for `to_entries | map(foo) | from_entries`,
useful for doing some operation to all keys and values of an object. 
`from_entries` accepts key, Key, name, Name, value and Value as keys.

## Examples
Input
```json
{ "a": 1, "b": 2 }
```
Query
```jq
jq 'to_entries'   # --> [{"key":"a", "value":1}, {"key":"b", "value":2}] 
```

Input
```json
[{"key":"a", "value":1}, {"key":"b", "value":2}]
```
Query
```jq
jq 'from_entries'   # --> {"a": 1, "b": 2} 
```

Input
```json
{"a": 1, "b": 2}
```
Query
```jq
jq 'with_entries(.key |= "KEY_" + .)'   # --> {"KEY_a": 1, "KEY_b": 2} 
```
