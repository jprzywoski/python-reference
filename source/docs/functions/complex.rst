=======
complex
=======

Description
===========
Returns an expression converted into a complex number.

Syntax
======
**complex** *([real[, imaginary]])*

*real*
	Optional. Must be a number.
*imaginary*
	Optional. Must be a number.
    
**complex** *([string])*

*string*
	Optional. If string is used it must represent a valid Python numeric type.

Return Value
============
**complex**

Time Complexity
============
#TODO

Note
====
When converting from a string, the string must not contain whitespace around the central + or - operator. For example, complex('1+2j') is fine, but complex('1 + 2j') raises *ValueError*. The complex type is described in Numeric Types — int, float, long, complex.

Remarks
=======
If the first parameter is a string, it will be interpreted as a complex number and the function must be called without a second parameter. The second parameter can never be a string. Each argument may be any numeric type (including complex). If imaginary is omitted, it defaults to zero and the function serves as a numeric conversion function like int(), long() and float(). If both arguments are omitted, returns 0j.

Example 1
=========
>>> complex()
0j
>>> complex(1)
(1+0j)
>>> complex(1, 2)
(1+2j)

Example 2
=========
>>> complex(1.12, 2.34)
(1.12+2.34j)
>>> complex(1, 2.34)
(1+2.34j)
>>> complex(1+2j)
(1+2j)
>>> complex(1+2j, 3+4j)
(-3+5j)

Example 2
=========
>>> complex('1')
(1+0j)
>>> complex('1+5j')
(1+5j)

See Also
========
#TODO

