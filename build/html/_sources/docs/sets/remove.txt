======
remove
======

Description
===========
Removes an element from the set (raises *KeyError* if not found).

Syntax
======
**set**. *remove(element)*

*element*
    Required. The element you want to delete.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> s = {1, 2}
>>> s.remove(1)
>>> s
set([2])
>>> s.remove(2)
>>> s.remove(2)
KeyError: 2

See also
========
#TODO

