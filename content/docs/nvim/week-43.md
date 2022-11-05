---
weight: 1
bookFlatSection: false
title: "Week 43"
---

# Regex with marks
Regular expressions can be also combined with marks in vim to have easier and more powerful expressions.

# Usage
- `\%<'m` - Match before position `'m`.
- `\%<'m` - Match after position `'m`.

For example, `/\%>'afoo\%<'b` search the pattern `foo` between the mark `'a` and `'b`.

