===
pop
===

Description
===========
Removes the key in the dictionary and returns its value.

Syntax
======
**dict**. *pop(key[, default])*

*key*
    Required. A dictionary key.
*default*
    Optional. Default value to be returned if key is not found.

Return Value
============
The same as deleted item.

Time Complexity
===============
#TODO

Remarks
=======
If default is not given and key is not in the dictionary, a KeyError is raised.

Example
=======
>>> d = {'a': 1, 'b': 2}
>>> d.pop('a')
1
>>> d.pop('x', 'foobar')
'foobar'
>>> d
{'b': 2}

See Also
========
#TODO
