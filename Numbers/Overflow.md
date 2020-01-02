---
title: "Checking for Integer Overflows"
date: 2019-09-25T12:02:55+02:00
author: "Reiner Martin"
tags: ["Julia", "Numerics", "Recreational Programming"]
---

Per default, integer overflows are not checked for, which can be dangerous and make it hard to detect certain bugs in your code. To activate checking, add

~~~Julia
+(a...) = Base.checked_add(a...)
-(a...) = Base.checked_sub(a...)
*(a...) = Base.checked_mul(a...)
~~~

at the beginning of your code.
