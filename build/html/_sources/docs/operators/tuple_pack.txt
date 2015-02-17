===============
* Tuple Packing
===============

Description
===========
Packs the consecutive function positional arguments into a tuple.

Syntax
======
def function(*tuple):
    suite

*tuple*
    A tuple object used for storing the passed in arguments. All the arguments can be accessed within the function body the same way as with any other tuple.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
====
The tuple name *args is used by convention.

Example
=======
>>> def add(*args):
...     total = 0
...     for arg in args:
...         total += arg
...     return total
... 
>>> add(1, 2, 3)
6

See also
========
#TODO