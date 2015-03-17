=====
index
=====

Description
===========
Returns the index of the first occurrence of the specified list item.

Syntax
======
**list**. *index(item)*

*item*
    Required. Any valid type. ValueError is raised if item is not in the list.

Return Value
============
**int**

Time Complexity
===============
O(1)

Example
=======
>>> [1, 2, 3].index(2)
1
>>> [1, 2, 3].index('foo')
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
ValueError: 'foo' is not in list

See Also
========
`in`_ statement
