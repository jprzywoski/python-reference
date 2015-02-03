========================
&= (intersection_update)
========================

Description
===========
Updates the set, keeping only elements found in it and the other set.

Syntax
======
set &= other & ...

*other*
    A set object or expression evaluating to a set.

Return Value
============
**set**

Time Complexity
===============
#TODO

Example
=======
>>> s = {1, 2}
>>> s &= {2, 3}
>>> s
set([2])

See also
========
#TODO