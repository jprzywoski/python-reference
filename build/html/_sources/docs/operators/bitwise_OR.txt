============
| Bitwise OR
============

Description
===========
Yields the bitwise (inclusive) OR of its arguments.

Syntax
======
A | B

Remarks
=======
A and B must be plain or long integers. The arguments are converted to a common type.
Bitwise OR performs logical OR operation on each pair of bits from the two inputs from the same position. Takes 0 as False and 1 as True.

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