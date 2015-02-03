======
extend
======

Description
===========
Extends the list by appending all the items from the iterable.

Syntax
======
**list**. *extend(iterable)*

*iterable*
    Required. Any iterable type.

Return Value
============
**None**

Time Complexity
===============
O(k)

Example
=======
>>> l = [1, 2]
>>> l.extend([3, 4])
>>> l
[1, 2, 3, 4]
>>> l.extend('foo')
>>> l
[1, 2, 3, 4, 'f', 'o', 'o']
>>> l.extend((5, 6))
>>> l
[1, 2, 3, 4, 'f', 'o', 'o', 5, 6]
>>> l.extend({'x': 100, 'y': 200})
>>> l
[1, 2, 3, 4, 'f', 'o', 'o', 5, 6, 'y', 'x']

See Also
========
`insert()`_ and `append()`_
