================================
^= (symmetric_difference_update)
================================

Description
===========
Updates the set, keeping only elements found in either the set or the other set, but not in both.

Syntax
======
**set ^= other**

*other*
    A set object or expression evaluating to a set.

Return Value
============
**set**

Time Complexity
===============
#TODO

Example
=======
>>> s = {1, 2}
>>> s ^= {2, 3}
>>> s
set([1, 3]) 

See also
========
#TODO