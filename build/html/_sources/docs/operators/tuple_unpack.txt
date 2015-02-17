=================
* Tuple Unpacking
=================

Description
===========
Unpacks the contents of a tuple into the function call.

Syntax
======
function(*iterable)

*iterable*
    An iterable object containing the positional arguments.

Return Value
============
#TODO

Time Complexity
============
#TODO

Example 1
=======
>>> def add(a, b):
...     return a + b
... 
>>> t = (2, 3)
>>> add(*t)
5

Example 2
====
>>> def add(a, b):
...     return a + b
... 
>>> add(*[2, 4])
6
>>> add(*"AD")
'AD'
>>> add(*{1: 1, 2: 2})
3

See also
========
#TODO