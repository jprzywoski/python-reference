=================
difference_update
=================

Description
===========
Updates the set, removing elements found in others. 

Syntax
======
**set**. *difference_update(iterable, ...)*

*iterable, ...*
    Required. Iterable or multiple iterables to be compared against the set.

Return Value
============
**None**

Time Complexity
===============
O(len(t))

Example
=======
>>> s = {1, 2}
>>> s.difference_update([2, 3])
>>> s
set([1])
>>> s.difference_update([1, 2], [3, 4])
>>> s
set([])

See also
========
#TODO