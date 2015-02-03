================
& (intersection)
================

Description
===========
Returns only the elements that appear both in the dictview and the specified iterable.

Syntax
======
**dictview & other**

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
>>> {'a': 1, 'b': 2}.viewitems() & {'b': 2, 'c': 3}.viewitems()
set([('b', 2)])
>>> {'a': 1, 'b': 2}.viewkeys() & {'b': 2, 'c': 3}.viewkeys()
set(['b'])

Example 2
=========
>>> {'a': 1, 'b': 2}.viewkeys() & ['b', 'c']
set(['b'])
>>> {'a': 1, 'b': 2}.viewitems() & [('b', 2), ('c', 3)]
set([('b', 2)]) 
