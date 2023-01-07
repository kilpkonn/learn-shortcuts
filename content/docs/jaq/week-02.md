---
weight: 1
bookFlatSection: false
title: "Week 2"
---

# Object identifier index
Object identifier filter is the most basic non-trivial filter there is (well, along array index).
The syntax is `.foo`, `'.foo.bar`, `."123foo"`, `."foo::bar"` or `.["foo"]`.
The filter takes object and returns value at the key specified or `null` otherwise.

# Example
```bash
echo '{ "a": 1, "b": true }' | jq '.a' # Outout: 1
echo '{ "a": 1, "b": true }' | jq '.["b"]' # Outout: true
```
