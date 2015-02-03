==================================
<<= Bitwise Left Shift Assignment
==================================

Description
===========
Performs bitwise left shift and assigns value to the left operand.

Syntax
======
A >>= B

Remarks
=======
Equivalent to A = A << B.

Example
=======
>>> b = 0b1111
>>> b <<= 1
>>> bin(b)
'0b11110' 