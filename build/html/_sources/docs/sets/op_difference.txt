==============
- (difference)
==============

Description
===========
Returns a new set with elements in the set that are not in the other set.

Syntax
======
**set - other**

*other*
    A set object or expression evaluating to a set.

Return Value
============
**set**

Time Complexity
===============
O(len(s))

Example
=======
>>> {1, 2} - {2, 3}
set([1])
>>> {1, 2, 3} - {2, 3, 4} - {3, 4, 5}
set([1])

See also
========
#TODO