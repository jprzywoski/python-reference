=======
discard
=======

Description
===========
Removes an element from the set.

Syntax
======
**set**. *discard(element)*

element
    Required. The item you want to delete.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> s = {1, 2}
>>> s.discard(1)
>>> s
set([2])
>>> s.discard(3)
>>> s
set([2])

See also
========
See also `remove()`_.

