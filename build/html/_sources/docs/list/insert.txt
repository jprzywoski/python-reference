======
insert
======

Description
===========
Inserts an item at a given position.

Syntax
======
**list**. *insert(index, object)*

*index*
    Required. The index of the element before which to insert.
*object*
    Required. The item to insert.

Return Value
============
**None**

Time Complexity
===============
O(n)

Example
=======
>>> l = [1, 2]
>>> l.insert(0, 0)
>>> l
[0, 1, 2]
>>> l.insert(2, 1.5)
>>> l
[0, 1, 1.5, 2]

See Also
========
`append()`_ and `extend()`_

