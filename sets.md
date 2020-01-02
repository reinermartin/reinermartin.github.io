---
title: "Sets"
date: 2019-09-25T15:25:06+02:00
author: "Reiner Martin"
tags: ["Julia"]
---




~~~julia
s = Set([2, 3, 5, 7])   # create set
s ∪ t, union(s, t)      # set union (can use iterators)
s ∩ t, intersect(s, t)  # set intersection
setdiff(s1, s2)         # elements in s but not in t
symdiff(s1, s2)         # elements exactly in one of s or t
push!(s, elem)          # add element to set
pop!(s, elem)           # remove element from set (error if not present)
collect(s)              # convert set to array
in(elem, s)             # is elem in set s?
~~~

Some of these function also work with iterators.

## Tests for subsets

~~~julia
s ⊆ t, t ⊇ s, issubset(s, t)   # is s1 a subset of s2?
s ⊈ t, t ⊉ s                   # is s1 not a subset of s2?
s ⊊ t, t ⊋ s                   # is s1 a proper subset of s2?
s == t, issetequal(s1, s2)      # [are these equivalent?]
~~~
