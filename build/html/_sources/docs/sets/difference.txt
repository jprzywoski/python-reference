==========
difference
==========

Description
===========
Returns a new set with elements in the set that are not in the specified iterables.

Syntax
======
**set**. *difference(iterable, ...)*

*iterable, ...*
    Required. Iterable or multiple iterables to be compared against the set.

Return Value
============
**set**

Time Complexity
===============
#TODO

Example 1
=========
>>> {1, 2}.difference([2, 3])
set([1])
>>> {1, 2}.difference((2, 3))
set([1])
>>> {1, 2}.difference({2, 3})
set([1])
>>> {1, 2}.difference({'a': 2, 'b': 3})
set([1, 2])
>>> {1, 2}.difference({'a': 2, 'b': 3}.values())
set([1])

Example 2
=========
>>> {1, 2}.difference([2, 3], [4, 5])
set([1])

See also
========
#TODO

