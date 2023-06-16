---
weight: 1
bookFlatSection: false
title: "Week 21"
---

# Function `error(message)`
Produces an error, just like `.a` applied to values other than `null` and objects would, but with the given message as the error's value.
Errors can be caught with `try/catch`

# Function `halt`
Stops the `jq` program with no further outputs. `jq` will exit with exit status `0`.

{{< hint info >}}
**Note:** The function `halt_error(exit_code)` works in a similar matter but you can also specify exit code which otherwise defaults to `5`.
{{< /hint >}}
