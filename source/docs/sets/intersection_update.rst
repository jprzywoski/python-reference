===================
intersection_update
===================

Description
===========
Updates the set, keeping only elements found in it and all others.

Syntax
======
**set**. *intersection_update(iterable, ...)*

*iterable, ...*
    Required. Iterable or multiple iterables to be compared against the set.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> s = {1, 2}
>>> s.intersection_update([2, 3])
>>> s
set([2])
>>> s = {1, 2}
>>> s.intersection_update([0, 1], [1, 2])
>>> s
set([1])

See also
========
#TODO