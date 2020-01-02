---
title: "Complex Numbers"
author: "Reiner Martin"
tags: ["Julia", "Mathematics"]
---


Julia has built-in support for complex numbers.


~~~julia
Complex{T}             # type for complex numbers where the real and imaginary parts are of type T
Complex64, Complex128  # complex number types
Complex{BigInt}        # works!!
~~~

~~~julia
im                     # imaginary unit  
z = 2 - 3im            # complex number
z = complex(2, 3)      # complex number
real(z), imag(z)       # real and imag part of z
conj(z)
~~~

