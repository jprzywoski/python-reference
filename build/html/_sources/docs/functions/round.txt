=====
round
=====

Description
===========
Returns a floating point number rounded to a specified number of decimal places.

Syntax
======
**round** *(number[, decimalplaces])*

*number*
	Required. An integer or float number.
*decimalplaces*
	Optional. An integer specifying the number of decimal places. If omitted, defaults to zero.

Return Value
============
**float**

Time Complexity
============
#TODO

Note
====
The behavior of round() for floats can be surprising: for example, round(2.675, 2) gives 2.67 instead of the expected 2.68. This is not a bug: it’s a result of the fact that most decimal fractions can’t be represented exactly as a float. 

See Floating Point Arithmetic: Issues and Limitations for more information.

See also: Decimal module.

Remarks
=======
Values are rounded to the closest multiple of 10 to the power minus decimalplaces; if two multiples are equally close, rounding is done away from 0 (so. for example, round(0.5) is 1.0 and round(-0.5) is -1.0).

Example
=======
>>> round(3.333, 1)
3.3
>>> round(2.675, 2)
2.67 #this is not correct in proper arithmetic
>>> round(0, 1)
0.0

See Also
========
#TODO
