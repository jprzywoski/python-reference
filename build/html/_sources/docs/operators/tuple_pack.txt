===============
* Tuple Packing
===============

Description
===========
Packs the consecutive function positional arguments into a tuple.

Syntax
======
def function(*args):
    suite

Example
=======
>>> def foo(*args):
...     print args
...
>>> foo(1, 2, 'foobar')
(1, 2, 'foobar')