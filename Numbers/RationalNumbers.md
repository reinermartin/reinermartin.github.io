---
title: "Rational Numbers"
author: "Reiner Martin"
tags: ["Julia"]
---



~~~julia
//                  # division as rational numbers
2//3 - 1//2         # rational numbers
denominator(2//3)   # is 3
numerator(2//3)     # is 2
rationalize(x)      # approximate x as a Rational
rationalize(T, x)   # with components of integer type 
~~~

Julia does not automatically check for numerical overflow.
