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
#TODO