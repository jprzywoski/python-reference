===========
|= (update)
===========

Description
===========
Adds elements from another set.

Syntax
======
**set |= other**

*other*
    A set object or expression evaluating to a set.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example 1
=========
>>> s = {0, 1}
>>> s |= {1, 2}
>>> s
set([0, 1, 2])

Example 2
=========
>>> s = {0, 1}
>>> s |= {1, 2} | {3, 4}
>>> s
set([0, 1, 2, 3, 4])

See also
========
#TODO
