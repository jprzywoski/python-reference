===
abs
===

Description
===========
Returns the absolute value of a number.

Syntax
======
**abs** *(number)*

*number*
	Required. Any valid numeric expression.

Return Value
============
The same as passed to the function.

Time Complexity
============
#TODO

Remarks
=======
If the number is a complex number, its magnitude is returned.

If the number is an integer with base other than 10 the abs() function will return its value as a decimal integer.

Example 1
=========
>>> abs(-1)
1
>>> abs(0)
0
>>> abs(1)
1
>>> abs(3.14)
3.14
>>> abs(3 + 2j)
3.6055512754639896

Example 2
=========
>>> abs(0x10)
16
>>> abs(0b10)
2
>>> abs(0o20)
16

See Also
========
#TODO