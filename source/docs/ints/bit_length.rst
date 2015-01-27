==========
bit_length
==========

Description
-----------
Returns the number of bits necessary to represent an integer in binary, excluding the sign and leading zeros.

Syntax
------
**int**. *bit_length()*

Return Value
------------
**int**

Remarks
-------
If x is nonzero, then x.bit_length() is the unique positive integer k such that 2**(k-1) <= abs(x) < 2**k. Equivalently, when abs(x) is small enough to have a correctly rounded logarithm, then k = 1 + int(log(abs(x), 2)). If x is zero, then x.bit_length() returns 0.

Example
-------
>>> n = -37
>>> bin(n)
'-0b100101'
>>> n.bit_length()
6
