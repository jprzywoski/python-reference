==========
isdisjoint
==========

Description
===========
Returns a Boolean stating whether the set contents overlap with the specified set or iterable.

Syntax
======
**set**. *isdisjoint(iterable)*

*iterable*
    Required. Iterable to be compared against the set.

Return Value
============
**bool**

Time Complexity
===============
#TODO

Remarks
=======
Sets are disjoint if and only if their intersection is the empty set.
If the *iterable* is empty, returns **True**.

Example
=======
>>> {0, 1, 2}.isdisjoint([1])
False
>>> {0, 1, 2}.isdisjoint([0, 1])
False
>>> {0, 1, 2}.isdisjoint([3, 4])
True
>>> {0, 1, 2}.isdisjoint(())
True

See also
========
#TODO