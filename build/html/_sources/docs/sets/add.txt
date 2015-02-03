===
add
===

Description
===========
Adds an element to the set. 

Syntax
======
**set**. *add(element)*

*element*
    Required. Element to be added to the set. Must be of a hashable type.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example 1
=========
>>> s = {1, 2}
>>> s.add(3)
>>> s
set([1, 2, 3])

Example 2
=========
>>> s = {1, 2}
>>> s.add({3, 4})
TypeError: unhashable type: 'set'
>>> s.add([3, 4])
TypeError: unhashable type: 'list'
>>> s.add({'a': 5})
TypeError: unhashable type: 'dict' 

See also
========
#TODO

