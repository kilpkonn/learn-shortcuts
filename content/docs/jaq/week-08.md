---
weight: 1
bookFlatSection: false
title: "Week 8"
---

# Object construction
Here are some basics on how to construct objects.

## Basics
Objects are constructed with `{}`, and you can use comma separated expressions inside object similarly to arrays.
One thing to note is that you might be able to specify keys without quotes if the are "identifier-like".

## Useful tips
Since it is common that we want something like `{ foo: .foo, bar: .bar }` there is a shorter form for it: `{ foo, bar }`.
If any of the expressions produces multiple outputs then multiple objects are produces.
However you can put parenthesis around the key to make it an expression and then the values will be concatenated if the keys match.

## Examples
Here are some ways of declaring objects with items.
```txt
{foo: .bar}
{user, title: .titles[]}  # multiple objects for single user
{(.user): .titles}  # Single object for single user
```
