===================
< (issubset proper)
===================

Description
===========
Returns a Boolean stating whether the set is contained in the specified set and that the sets are not equal.

Syntax
======
**set < other**

*other*
    A set object or expression evaluating to a set.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> {1, 2} < {1, 2}
False
>>> {1, 2} < {1, 2, 3}
True
>>> {1, 2} < {'frob'}
False

See also
========
#TODO