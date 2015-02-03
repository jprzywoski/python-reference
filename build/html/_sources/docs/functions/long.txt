====
long
====

Description
===========
Returns an expression converted into a long integer number.

Syntax
======
**long** *([number, [base]])*

*number*
	Optional. Can be of string, int, float or long type.
*base*
	Optional. If used number must be a string.

Return Value
============
**long**

Time Complexity
===============
#TODO

Remarks
=======
If number is floating point, the conversion truncates towards zero. If the argument is outside the integer range, the function returns a long object instead.

If number is not a number or if base is given, then number must be a string or Unicode object representing an integer literal in radix base. Optionally, the literal can be preceded by + or - (with no space in between) and surrounded by whitespace. A base-n literal consists of the digits 0 to n-1, with a to z (or A to Z) having values 10 to 35. The default base is 10. The allowed values are 0 and 2-36. Base-2, -8, and -16 literals can be optionally prefixed with 0b/0B, 0o/0O/0, or 0x/0X, as with integer literals in code. Base 0 means to interpret the string exactly as an integer literal, so that the actual base is 2, 8, 10, or 16.

Example 1
=========
>>> # this example converts an octal, hex and binary integer into a proper integer
>>> long(0o10)
8
>>> long (0x10)
16
>>> long (0b10)
2

Example 2
=========
>>> # this example uses base argument
>>> long('0101', 2)
5L
>>> long('0101', 8)
65L
>>> long('0101', 16)
257L
>>> long('0101', 10)
101L

Example 3
=========
>>> long(3.14)
3L
>>> long(3.14e10)
31400000000L
>>> long(-3.14)
-3L

Example 4
=========
>>> long('-100')
-100L
>>> long('+100')
100
>>> long('100')
100L

See Also
========
#TODO

