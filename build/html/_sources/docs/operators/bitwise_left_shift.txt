=====================
<< Bitwise Left Shift
=====================

Description
===========
Shifts the bits of the first operand left by the specified number of bits.

Syntax
======
A << B

*A*
    Integer object.
*B*
    Integer object.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Negative shift counts are illegal and cause a ValueError to be raised.

A left shift by n bits is equivalent to multiplication by pow(2, n). A long integer is returned if the result exceeds the range of plain integers.

Example 1
=========
>>> bin(0b1111 << 1)
'0b11110'
>>> bin(0b1111 << 2)
'0b111100'
>>> bin(0b1111 << 3)
'0b1111000'
>>> bin(0b1111 << 4)
'0b11110000'

Example 2
=========
>>> 128 * 2
256
>>> 128 << 1
256

See also
========
#TODO