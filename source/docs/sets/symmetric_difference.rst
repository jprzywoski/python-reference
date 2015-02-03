====================
symmetric_difference
====================

Description
===========
Returns a new set with elements in either the set or the specified iterable but not both.

Syntax
======
**set**. *symmetric_difference(iterable)*

*iterable*
    Required. Any iterable.

Return Value
============
**set**

Time Complexity
===============
#TODO

Example
=======
>>> {1, 2}.symmetric_difference([2, 3])
set([1, 3])
>>> {1, 2}.symmetric_difference([4, 5])
set([1, 2, 4, 5])

See also
========
#TODO