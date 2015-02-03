=========================
&= Bitwise AND Assignment
=========================

Description
===========
Performs bitwise AND and assigns value to the left operand.

Syntax
======
A &= B

Remarks
=======
Equivalent to A = A & B.

Example
=======
>>> b = 0b1111
>>> b &= 0b0101
>>> bin(b)
'0b101' 