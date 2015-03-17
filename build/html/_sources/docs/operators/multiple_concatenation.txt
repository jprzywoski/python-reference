================
* multiple concatenation
================

Description
===========
Returns a sequence self-concatenated specified amount of times.

Syntax
======
**A * N** or **N * A**

*A*
    Any sequence.
*N*
    Any expression evaluating to a numeric type.

Return Value
============
the same as used as sequence operand

Time Complexity
============
O(nk)

Example 1
=======
>>> "A" * 10
'AAAAAAAAAA'
>>> [0, 1] * 2
[0, 1, 0, 1]
>>> (0, 1) * 2
(0, 1, 0, 1)

See also
========
#TODO