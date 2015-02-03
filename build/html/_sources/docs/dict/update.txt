======
update
======

Description
===========
Adds key:value elements to the dictionary.

Syntax
======
**dict**. *update([mapping])*

*mapping*
    Required. Either another dictionary object or an iterable of key:value pairs (iterables of length two). If keyword arguments are specified, the dictionary is then updated with those key:value pairs.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example 1
=========
>>> d = {'a': 1, 'b': 2}
>>> d.update({'a': 'I', 'c': 3})
>>> d
{'a': 'I', 'b': 2, 'c': 3}

Example 2
=========
>>> d = {'a': 1, 'b': 2}
>>> d.update([('x', 10), ('y', 20)])
>>> d
{'a': 1, 'b': 2, 'x': 10, 'y': 20}

Example 3
=========
>>> d = {'a': 1, 'b': 2}
>>> d.update(foo='bar', sn='afu')
>>> d
{'a': 1, 'b': 2, 'foo': 'bar', 'sn': 'afu'}

See Also
========
#TODO
