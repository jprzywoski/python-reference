=======================
** Dictionary Unpacking
=======================

Description
===========
Unpacks the contents of a dictionary into the function call.

Syntax
======
function(**dict)

*dict*
    The dictionary containing pairs of keyword arguments and their values.
    
Return Value
============
#TODO

Time Complexity
============
#TODO

Example
=======
>>> def add(a=0, b=0):
...     return a + b
... 
>>> d = {'a': 2, 'b': 3}
>>> add(**d)
5

See also
========

In purpose of unpack a dict values as it were a list values.

>>> from operator import itemgetter
>>> d = {'foo': 1, 'bar': 2, 'baz': 3}
>>> foo, baz = itemgetter('foo', 'baz')(d)
(1, 3)

#TODO
