=============
^ Bitwise Exclusive XOR
=============

Description
===========
Returns the result of bitwise XOR of two integers.

Syntax
======
A ^ B

*A*
    Integer object.
*B*
    Integer object.

Remarks
=======
Bitwise XOR sets the bits in the result to 1 if either, but not both, of the corresponding bits in the two operands is 1.

Example 1
=========
>>> bin(0b1111 ^ 0b1111)
'0b0'
>>> bin(0b1111 ^ 0b0000)
'0b1111'
>>> bin(0b0000 ^ 0b1111)
'0b1111'
>>> bin(0b1010 ^ 0b1111)
'0b101'

Example 2
=========
>>> # this example swaps integers without a temporary variable using XOR
>>> a = 2
>>> b = 8
>>> a ^= b
>>> b ^= a
>>> a ^= b
>>> a
8
>>> b
2

See also
========
#TODO
