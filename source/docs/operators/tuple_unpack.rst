=================
* Tuple Unpacking
=================

Description
===========
Unpacks the contents of a tuple into the function call.

Syntax
======
function(*tuple)

Example
=======
>>> def foo(a, b):
...     print a + b
...
>>> t = ('foo', 'bar')
>>> foo(*t)
foobar