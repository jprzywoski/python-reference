===
pop
===

Description
===========
Removes and returns the item at the specified index.

Syntax
======
**list**. *pop([index])*

*index*
    Optional. Index of the item you want to delete. Default value is -1 (the last item in the list).

Return Value
============
The same that was deleted.

Time Complexity
===============
O(1) for pop()
O(n) for pop(index)

Example
=======
>>> [1, 2, 3].pop()
3
>>> [1, 2, 3].pop(0)
1

See Also
========
`remove()`_, `del`_ statement
