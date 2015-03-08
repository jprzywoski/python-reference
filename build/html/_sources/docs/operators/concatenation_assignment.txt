======================
+= concatenation assignment
======================

Description
===========
Concatenates the sequence with the right operand and assigns the result to that sequence.

Syntax
======
**A += B**

*A*
    Any sequence.
*B*
    Sequence of the same type as A.

Return Value
============
the same as used as sequence operand

Time Complexity
============
#TODO

Remarks
=======
Equivalent to A = A + B.

Example 1
=======
>>> s = "AA"
>>> s += "BB"
>>> s
'AABB'

Example 2
=======
>>> l = [0, 1]
>>> l += [2, 3]
>>> l
[0, 1, 2, 3]

Example 3
=======
>>> t = (0, 1)
>>> t += (2, 3)
>>> t
(0, 1, 2, 3)

See Also
========
#TODO