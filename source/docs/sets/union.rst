=====
union
=====

Description
===========
Returns a new set with elements from the set and the specified iterables.

Syntax
======
**set**. *union(iterable, ...)*

*iterable, ...*
    Required. Iterable or multiple iterables to be compared against the set.

Return Value
============
**set**

Time Complexity
===============
#TODO

Example
=======
>>> {1, 2}.union([2, 3])
set([1, 2, 3])
>>> {1, 2}.union([3, 4])
set([1, 2, 3, 4])
>>> {1, 2}.union([3, 4], (5, 6), {7, 8})
set([1, 2, 3, 4, 5, 6, 7, 8])

See also
========
#TODO