=======================
** Dictionary Unpacking
=======================

Description
===========
Unpacks the contents of a dictionary into the function call.

Syntax
======
function(**dict)

Example
=======
>>> def foo(a=None, b=None):
...     return a, b
...
>>> d = {'a': 1, 'b': 2}
>>> foo(**d)
(1, 2)