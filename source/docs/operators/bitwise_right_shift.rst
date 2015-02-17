======================
>> Bitwise Right Shift
======================

Description
===========
Shifts the bits of the first operand right by the specified number of bits.

Syntax
======
A >> B

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

A right shift by n bits is equivalent to division by pow(2, n).

Example 1
=========
>>> bin(0b1111 >> 1)
'0b111'
>>> bin(0b1111 >> 2)
'0b11'
>>> bin(0b1111 >> 3)
'0b1'
>>> bin(0b1111 >> 4)
'0b0'

Example 2
=========
>>> 128 / 2
64
>>> 128 >> 1
64

See also
========
#TODO