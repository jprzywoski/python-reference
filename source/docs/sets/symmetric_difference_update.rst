===========================
symmetric_difference_update
===========================

Description
===========
Updates the set, keeping only elements found in either set, but not in both. 

Syntax
======
**set**. *symmetric_difference_update(iterable)*

*iterable*
    Required. Any iterable.

Return Value
============
**None**

Time Complexity
===============
O(len(t)) to O(len(t) * len(s)) 

Example
=======
>>> s = {1, 2}
>>> s.symmetric_difference_update((2, 3))
>>> s
set([1, 3])

See also
========
#TODO