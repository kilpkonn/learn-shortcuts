---
weight: 1
bookFlatSection: false
title: "Week 4"
---

# Array filters
Array filter is quite basic as it works as `.[i]` where `i` is the index of the object we wish to select.
Note that also negative indexes work just as in python.

# Slice filters
Slice filters work as `.[i:j]` where `i` is the start index and `j` is the end index of the slice.
The filter works on both arrays and strings.

# Examples
```bash
echo '[1,2,3]' | jq '.[-2]' # 2
echo '["a","b","c","d","e"]' | jq '.[2:4]' # ["c", "d"] 
```

