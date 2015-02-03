=============
^ Bitwise XOR
=============

Description
===========
Yields the bitwise (exclusive) XOR of its arguments.

Syntax
======
A ^ B

Remarks
=======
A and B must be plain or long integers. The arguments are converted to a common type.
Performs logical XOR (exclusive OR) operation on each pair of bits from the two inputs from the same position. Takes 0 as False and 1 as True.

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