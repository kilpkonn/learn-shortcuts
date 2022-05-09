---
weight: 1
bookFlatSection: false
title: "Week 19"
---

# More on inserting and deleting
How to insert and delete text are some of the first things you have to learn in vim, but there
are also more "advanced" ways to do it or just cool shortcuts for it.

## Start inserting on new line
The `o` key can be used to start inserting text to newline just below the cursor.
The capital `O` does the same, but start inserting to a line above.

## Special inserts
There are also some more special ways to insert text.
`:r [filename]` can be used to insert the contents of some file to current location.
`:r ![command]` runs shell command and pastes the output to current location.

## Deleting by sentence
To delete from current location to the end of sentence `d)` can be used.
Similarly `d}` etc. can be used to delete to end of paragraph etc.

## Replacing text
To replace single character use `r`.
To go to replace mode (instead of inserting new characters overwrite existing ones) use `R`.
