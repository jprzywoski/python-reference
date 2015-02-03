======
remove
======

Description
===========
Removes the first item from the list which matches the specified value.

Syntax
======
**list**. *remove(object)*

*object*
    Required. Any valid type. If not found error is raised.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> l = [1, 2]
>>> l.remove(2)
>>> l
[1]
>>> l.remove('foo')
ValueError: list.remove(x): x not in list

See Also
========
`pop()`_, `del`_ statement
