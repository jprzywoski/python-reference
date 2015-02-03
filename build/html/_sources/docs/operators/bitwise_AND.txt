=============
& Bitwise AND
=============

Description
===========
Yields the bitwise AND of its arguments.

Syntax
======
A & B

Remarks
=======
A and B must be plain or long integers. The arguments are converted to a common type.
Bitwise AND performs the logical AND operation on each pair of bits from the two inputs from the same position. Takes 0 as False and 1 as True.

Example 1
=========
>>> bin(0b1111 & 0b1111)
'0b1111'
>>> bin(0b1111 & 0b0000)
'0b0'
>>> bin(0b0000 & 0b1111)
'0b0'
>>> bin(0b1010 & 0b1111)
'0b1010'

Example 2 
=========
>>> # this example checks  if an integer is even/uneven using bitwise AND
>>> bool(8 & 1)
False
>>> bool(9 & 1)
True