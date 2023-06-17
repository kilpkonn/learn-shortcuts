---
weight: 1
bookFlatSection: false
title: "Week 22"
---

# Function `add`
The filter `add` takes as input an array, and produces as output the elements of the array added together.
This might mean summed, concatenated or merged depending on the types of the elements of the input array - the rules are the same as those for the `+` operator.

If the input is an empty array, add returns `null`.

## Examples
Input
```json
["a", "b", "c"]
```
Query
```jq
jq 'add'   # --> "abc" 
```
