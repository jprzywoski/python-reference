===
get
===

Description
===========
Returns the value for key in the dictionary; if not found returns a default value.

Syntax
======
**dict**. *get(key[, default])*

*key*
    Required. A key in the dictionary.
*default*
    Optional. Value that is returned when the key is not found. Defaults to None, so that this method never raises a KeyError.

Return Value
============
The value of the key.

Time Complexity
===============
#TODO

Example
=======
>>> d = {'a': 1, 'b': 2}
>>> d.get('a')
1
>>> d.get('x')
>>> d.get('x', 'foobar')
'foobar'

See Also
========
#TODO
