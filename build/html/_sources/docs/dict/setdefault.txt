setdefault

Description
===========
Returns a value of the key in the dictionary; if key is not found inserts that key with the specified value and returns that value.

Syntax
======
**dict**. *setdefault(key[, default])*

*key*
    Required. A dictionary key.
*default*
    Optional. The value that is inserted when the key is not found. Defaults to None.

Return Value
============
The value of the key.

Time Complexity
===============
#TODO

Example
=======
>>> d = {'a': 1, 'b': 2}
>>> d.setdefault('a')
1
>>> d
{'a': 1, 'b': 2}
>>> d.setdefault('x')
>>> d
{'a': 1, 'b': 2, 'x': None}
>>> d.setdefault('y', 'foobar')
'foobar'
>>> d
{'a': 1, 'b': 2, 'x': None, 'y': 'foobar'} 

See Also
========
#TODO
