---
weight: 1
bookFlatSection: false
title: "Week 13"
---

# Function `keys`
The builtin function `keys`, when given an object, returns its keys in an array.

The keys are sorted "alphabetically", by unicode codepoint order.
This is not an order that makes particular sense in any particular language, but you can count on it being the same for any two objects with the same set of keys, regardless of locale settings.

{{< hint info >}}
**Note:** For arrays the `keys` function returns an array of indices.
{{< /hint >}}

## Examples
Input
```json
{ "abc": 1, "abcd": 2, "Foo": 3 }
```
Query
```jq
jq 'keys'  -> ["Foo", "abc", "abcd"]
```

Input
```json
[42, 3, 35]
```
Query
```jq
jq 'keys'  -> [0,1,2] 
```
