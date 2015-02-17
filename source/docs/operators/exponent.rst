===========
** power
===========

Description
===========
Returns the value of a numeric expression raised to a specified power.

Syntax
======
**A ** B**

*A*
    Any expression evaluating to a numeric type.
*B*
    Any expression evaluating to a numeric type.

Return Value
============
According to coercion rules.

Time Complexity
============
#TODO

Remarks
=======
Python defines pow(0, 0) and 0 ** 0 to be 1, as is common for programming languages.

Example 1
=========
>>> 2**2
4
>>> 2**2.0
4.0
>>> 2.0**2
4.0

Example 2
=========
>>> 4**0.5
2.0
>>> 4**-2
0.0625

See also
========
#TODO