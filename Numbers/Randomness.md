---
title: "Randomness"
author: "Reiner Martin"
tags: ["Julia"]
---


## Random numbers

~~~julia
rand(), rand(n), rand(n, m)     # uniform from [0,1), either single, vector, or matrix
randn(), randn(n), randn(n, m)  # normal, either single, vector, or matrix
rand(a:b)                       # equiprobablity from range a:b
range(c)                        # c is any indexable collection (array, tuple, set, string, ...)
Random.randstring("ACGT", n)    # random string of letters n draen from the string 
~~~


### Using other distributions

~~~julia
using Distributions
my_dist = Bernoulli(0.2) # For example
rand(my_dist) 
~~~
