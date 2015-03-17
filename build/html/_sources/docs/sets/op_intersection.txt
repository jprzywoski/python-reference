================
& (intersection)
================

Description
===========
Returns a new set with elements common to the set and the other set.

Syntax
======
**set & other**

*other*
    A set object or expression evaluating to a set.

Return Value
============
**set**

Time Complexity
===============
O(min(len(s), len(t)) to O(len(s) * len(t)) 

Example
=======
>>> {1, 2} & {2, 3}
set([2])
>>> {1, 2} & {2, 3} & {2, 'foo'}
set([2])

See also
========
#TODO