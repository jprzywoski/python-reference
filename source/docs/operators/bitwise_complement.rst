==========================
~ bitwise complement
==========================

Description
===========
Sets the 1 bits to 0 and 1 to 0.

Syntax
======
~A

*A*
    Integer object.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The bitwise inversion of A is defined as -(A + 1). It only applies to integral numbers.

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

See also
========
#TODO