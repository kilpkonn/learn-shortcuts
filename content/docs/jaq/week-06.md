---
weight: 1
bookFlatSection: false
title: "Week 6"
---

# Basic filter combinators
Here are some basics on how to combine filters.

## Comma filter (`,`)
If too filters are separated with comma both filters are ran and their outputs are concatenated in the order they are specified.

## Pipe filter (`|`)
If too filters are separated by a pipe operator then the first filter is rand and its output is fed into the second filter.

# Examples
```bash
echo '{"foo": 42, "bar": "something else", "baz": true}' | jq '.foo, .bar' # [42, "something else"]
echo '[{"name":"JSON", "good":true}, {"name":"XML", "good":false}]' | jq '.[] | .name' # ["JSON", "XML"]
```
{{< hint info >}}
**Note:** Parenthesis work as grouping operator just like in other programming languages.
{{< /hint >}}

