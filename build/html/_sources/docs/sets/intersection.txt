============
intersection
============

Description
===========
Returns a new set with elements common to the set and the specified iterables.

Syntax
======
**set**. *intersection(iterable, ...)*

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
>>> {1, 2}.intersection([2, 3])
set([2])
>>> {1, 2}.intersection([0, 1], [1, 2])
set([1])

See also
========
#TODO