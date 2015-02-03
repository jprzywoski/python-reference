=====
float
=====

Description
===========
Returns an expression converted into a floating point number.

Syntax
======
**float** *(number)*

*number*
	Optional. A numeric type other than complex number or string representation of a number.

Return Value
============
**float**

Time Complexity
============
#TODO

Note
====
When passing in a string, values for NaN and Infinity may be returned, depending on the underlying C library. Float accepts the strings nan, inf and -inf for NaN and positive or negative infinity. The case and a leading + are ignored as well as a leading - is ignored for NaN. Float always represents NaN and infinity as nan, inf or -inf.

Example 1
=========
>>> float(1)
1.0
>>> float(1.34)
1.34
>>> float('2')
2.0
>>> float('-2')
-2.0
>>> float('-2.313123')
-2.313123

Example 2
=========
>>> float('+nan')
nan
>>> float('-infinity')
-inf

See Also
========
#TODO