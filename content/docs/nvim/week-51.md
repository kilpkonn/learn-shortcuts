---
weight: 1
bookFlatSection: false
title: "Week 51"
---

# Abbreviations
Vim has a feature called abbreviations that can be used to either write out text without actually having to type all words or to
correct some common typing mistakes.

# Basic usage
To see all the abbreviations created use `:ab[breviate]` command.  
To see abbreviations starting with some specific string you can use `:ab <string>`.  
New abbreviations can be created with `:ab <string> <replacement>` and cleared with `:una <string>`.
To clear all abbreviations you can use `:abc[lear]`.  

To create abbreviation for only a specific mode you can prefix the command with `i` for insert mode or `c` for command line mode.
