=============
& Bitwise AND
=============

Description
===========
Returns the result of bitwise AND of two integers.

Syntax
======
A & B

*A*
    Integer object.
*B*
    Integer object.

Remarks
=======
Bitwise AND sets the bits in the result to 1 if both the corresponding bits in the two operands are 1.

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

See also
========
#TODO