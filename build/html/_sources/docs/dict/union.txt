=========
| (union)
=========

Description
===========
Returns all the elements that appear in the dictview and the specified iterable.

Syntax
======
**dictview | other**

*other*
    Any iterable item.

Return Value
============
**set**

Time Complexity
===============
#TODO

Example 1
=========
>>> {'a': 1, 'b': 2}.viewitems() | {'b': 2, 'c': 3}.viewitems()
set([('a', 1), ('b', 2), ('c', 3)])
>>> {'a': 1, 'b': 2}.viewkeys() | {'b': 2, 'c': 3}.viewkeys()
set(['a', 'b', 'c'])

Example 2
=========
>>> {'a': 1, 'b': 2}.viewkeys() | ['b', 'c']
set(['a', 'b', 'c'])
>>> {'a': 1, 'b': 2}.viewitems() | [('b', 2), ('c', 3)]
set([('a', 1), ('b', 2), ('c', 3)]) 
