============
| Bitwise Inclusive OR
============

Description
===========
Returns the result of bitwise OR of two integers.

Syntax
======
A | B

*A*
    Integer object.
*B*
    Integer object.

Return Value
============
**int**

Time Complexity
============
#TODO

Remarks
====
Bitwise OR sets the bits in the result to 1 if either of the corresponding bits in the two operands is 1.

Example
=======
>>> bin(0b1111 | 0b1111)
'0b1111'
>>> bin(0b1111 | 0b0000)
'0b1111'
>>> bin(0b0000 | 0b1111)
'0b1111'
>>> bin(0b1010 | 0b1111)
'0b1111'

See also
========
#TODO