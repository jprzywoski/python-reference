=====================
** Dictionary Packing
=====================

Description
===========
Packs the consecutive function keyword arguments into a dictionary.

Syntax
======
def function(**kwargs):
    suite

Example
=======
>>> def foo(**kwargs):
...     print kwargs
>>> foo(a=1, b=2, foo='bar')
{'a': 1, 'b': 2, 'foo': 'bar'}