---
weight: 1
bookFlatSection: false
title: "Week 5"
---

# Array/Object value iterator
Array/object value iterator simply returns whole array/object instead of some of its values.
You can also postfix it with `?` to avoid yielding error if the root object isn't array nor object.

# Examples
```bash
echo '[1,2,3]' | jq '.[]' # [1, 2, 3]
```

