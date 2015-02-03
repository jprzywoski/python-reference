====
copy
====

Description
===========
Returns a shallow copy of the dictionary.

Syntax
======
**dict**. *copy()*

Return Value
============
**dict**

Time Complexity
===============
#TODO

Example 1
=========
>>> d = {'a': 1, 'b': 2}
>>> dd = d.copy()
>>> dd
{'a': 1, 'b': 2}

Example 2
=========
>>> d = {'a': 1, 'b': [1, 2]}
>>> dd = d.copy()
>>> dd
{'a': 1, 'b': [1, 2]}
>>> d['b'][0] = 'foo'      # since copy() returns a shallow copy
>>> dd                     # (only references to the copied elements are returned),
{'a': 1, 'b': ['foo', 2]}  # altering the objects in original dictionary will affect it’s copy as well

See Also
========
#TODO
