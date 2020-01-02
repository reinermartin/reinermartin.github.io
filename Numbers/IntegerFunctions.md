---
title: "Integers and its Functions"
date: 2019-09-25T14:17:17+02:00
author: "Reiner Martin"
tags: ["Julia", "Number Theory"]
weight: 10
---

### Types

Integer types are

~~~julia
Int8, Int16, Int32, Int64, Int128      # Signed
UInt8, UInt16, UInt32, UInt64, UInt128 # Unsigned
BigInt                                 # Arbitrary precision
~~~

### Literal constants

~~~julia
17 0x11                    # 17 in decimal, hexadecimal,
0o21 0b10001               # 17 in octal, binary
~~~

### Number-theoretic (integer) functions

~~~julia
isodd(n)                 # is n odd?
iseven(n)                # is n even?

div(x, y), x ÷ y         # division with remainder
fld(x, y)                # floor of x/y
fld1(x, y)
cld(x, y)                # ceiling of x/y
divrem(x, y) (x/y, x%y)
fldmod(x, y)
fld1
mod(n, m)                # n modulo m, in range 0:m-1 (or m+1:0 if m is negativee)
mod1(n, m)               # n modulo m, in range 1:m (or m:-1 if m is negativee)
fldmod1

nextpow(a, n)            # smallest a^n ≥ x (a>1, n>0)
prevpow(a, n)            # largest a^n ≤ x (a>1, n>0)
ispow2(n)                # test whether n is a power of two
nextprod([a,b,..], n)    # next integer ≥ n which is product of numbers from [a,b,...] with repetition

gcd(a,b,c), gcd([a,b,c]) # greatest common divisor
lcm(a,b,c), lcm([a,b,c]) # least common multiple

powermod(a, k, p)        # a^k modulo p
invmod
factorial(n)             # factorial n! = 1*2*...*n
binomial(n, k)           # binomial coefficient n!/(k!(n-k)!)

widemul
~~~

### Decimal, binary and other representation

These three functions accept keywords 'base' and 'pad'.

~~~julia
digits(123)      # ⟶ [3, 2, 1], 
ndigits(n)       # number of digits in integer n
string(n)
~~~
