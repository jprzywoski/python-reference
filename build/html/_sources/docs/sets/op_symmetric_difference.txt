========================
^ (symmetric_difference)
========================

Description
===========
Returns a new set with elements in either the set or the other set but not both.

Syntax
======
**set ^ other**

*other*
    A set object or expression evaluating to a set.

Return Value
============
**set**

Time Complexity
===============
O(len(s)) to O(len(s) * len(t)) 

Example
=======
>>> {1, 2} ^ {2, 3}
set([1, 3])
>>> {1, 2} ^ {1, 2}
set([]) 

See also
========
#TODO