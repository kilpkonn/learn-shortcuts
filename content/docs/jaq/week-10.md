---
weight: 1
bookFlatSection: false
title: "Week 10"
---

# Addition (`+`) and subtraction (`-`)
Addition takes two filters and then adds results of them together.
Depending of the value type, adding has different meanings:
- **Numbers** are added arithmetically
- **Arrays** are concatenated
- **Strings** are concatenated
- **Objects** are merged. If both have same key, then the object on the right wins

{{< hint info >}}
**Note:** `null` can be added to any value resulting no change.
{{< /hint >}}

Subtraction works in a similar manner.
For arrays it means that are occurrences of element(s) are removed.



## Examples
Input
```json
{ "a":3 }
```
Query
```jq
jq '.a + 1'    -> 4
jq '4 - .a'    -> 1
```

Input 
```json
["xml", "yaml", "json"]
```
Query
```jq
jq '. - ["xml", "yaml"]'   -> ["json"]
```
