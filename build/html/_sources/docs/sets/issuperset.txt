==========
issuperset
==========

Description
===========
Returns a Boolean stating whether the set contains the specified set or iterable.

Syntax
======
**set**. *issuperset(iterable)*

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
If the *iterable* is empty, returns **True**.

Example
=======
>>> {0, 1, 2}.issuperset([1])
True
>>> {0, 1, 2}.issuperset([0, 1])
True
>>> {0, 1, 2}.issuperset([2, 3])
False
>>> {0, 1, 2}.issuperset(())
True

See also
========
#TODO