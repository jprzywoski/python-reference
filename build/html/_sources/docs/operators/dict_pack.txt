=====================
** Dictionary Packing
=====================

Description
===========
Packs the consecutive function keyword arguments into a dictionary.

Syntax
======
def function(**dict):
    suite

*dict*
    A dictionary object used for storing the passed in arguments. All the arguments can be accessed within the function body the same way as with any other dictionary.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
====
The dict name **kwargs is used by convention.

Example
=======
>>> def example(**kwargs):
...     return kwargs.keys()
... 
>>> example(a=10, b=20, c=[0, 0, 0])
['a', 'c', 'b']

See also
========
#TODO