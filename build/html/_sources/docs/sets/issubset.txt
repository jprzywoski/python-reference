========
issubset
========

Description
===========
Returns a Boolean stating whether the set is contained in the specified set or iterable.

Syntax
======
**set**. *issubset(iterable)*

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
If the *iterable* is empty, returns **False**.

Example
=======
>>> {0, 1}.issubset({0, 1, 2})
True
>>> {1}.issubset({0, 1, 2})
True
>>> {1}.issubset({'A', 'B', 'C'})
False
>>> {1}.issubset(())
False

See also
========
#TODO