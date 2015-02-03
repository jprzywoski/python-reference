==========================
~ Unary Bitwise Complement
==========================

Description
===========
Flipps bits.

Syntax
======
~A

Remarks
=======
Performs logical NOT operation on bits. Takes 0 as False and 1 as True.

Unlike &, | and  ^, 1’s complement is a unary operator (takes only one input).

The bitwise inversion of A is defined as -(A+1). It only applies to integral numbers.

Example
=======
>>> bin(~0b1111)
'-0b10000'
>>> bin(~0b0000)
'-0b1'
>>> bin(~0b1010)
'-0b1011'
>>> bin(~0b1011)
'-0b1100'