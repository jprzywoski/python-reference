=========
| (union)
=========

Description
===========
Returns a new set with elements from the set and the other set.

Syntax
======
**set | other**

*other*
    A set object or expression evaluating to a set.

Return Value
============
**set**

Time Complexity
===============
O(len(s)+len(t))

Example
=======
>>> {1, 2} | {3, 4} | {4, 5}
set([1, 2, 3, 4, 5])

See also
========
#TODO