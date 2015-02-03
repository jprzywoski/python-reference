===
int
===

Description
===========
Returns an expression converted into an integer number.

Syntax
======
**int** *([number, [base]])*

*number*
	Optional. Can be of string, int, float or long type.
*base*
	Optional. If used number must be a string.

Return Value
============
**int**

Time Complexity
===============
#TODO

Remarks
=======
If number is floating point, the conversion truncates towards zero. If the argument is outside the integer range, the function returns a long object instead.

If number is not a number or if base is given, then number must be a string or Unicode object representing an integer literal in radix base. Optionally, the literal can be preceded by + or - (with no space in between) and surrounded by whitespace. A base-n literal consists of the digits 0 to n-1, with a to z (or A to Z) having values 10 to 35. The default base is 10. The allowed values are 0 and 2-36. Base-2, -8, and -16 literals can be optionally prefixed with 0b/0B, 0o/0O/0, or 0x/0X, as with integer literals in code. Base 0 means to interpret the string exactly as an integer literal, so that the actual base is 2, 8, 10, or 16.

Example 1
=========
>>> # this example converts octal, hex and binary integers into a decimal integer
>>> int(0o10)
8
>>> int(0x10)
16
>>> int(0b10)
2

Example 2
=========
>>> # this example uses base argument
>>> int('0101', 2)
5
>>> int('0101', 8)
65
>>> int('0101', 16)
257
>>> int('0101', 10)
101

Example 3
=========
>>> int(3.14)
3
>>> int(3.14e10)
31400000000L
>>> int(-3.14)
-3

Example 4
=========
>>> int('-100')
-100
>>> int('+100')
100
>>> int('100')
100

See Also
========
#TODO

