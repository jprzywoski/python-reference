==========
/ division
==========

Description
===========
Returns the quotient of numbers.

Syntax
======
A / B [/ …]

Remarks
=======
For (plain or long) integer division, the result is an integer. The result is always rounded towards minus infinity: 1/2 is 0, (-1)/2 is -1, 1/(-2) is -1, and (-1)/(-2) is 0. Note that the result is a long integer if either operand is a long integer, regardless of the numeric value.

Example
=======
>>> 2 / 1
2
>>> 2 / 1.0
2.0
>>> 2.0 / 1
2.0
>>> 2 / 0.7
2.857142857142857