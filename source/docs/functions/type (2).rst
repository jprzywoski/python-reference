========
type (2)
========

Description
===========
Returns a new type object.

Syntax
======
**type** *(name, bases, dict)*

*name*
	The name string is the class name and becomes the __name__ attribute
*bases*
	the bases tuple itemizes the base classes and becomes the __bases__ attribute
*dict*
	the dict dictionary is the namespace containing definitions for class body and becomes the __dict__ attribute

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
This is essentially a dynamic form of the class statement. For example, the following two statements create identical type objects:

Example
=======
>>> class X(object):
...     a = 1
...
>>> x = X()
>>> x
<__main__.X object at 0x00DCE570>
>>> x.a
1
>>> X = type('X', (object,), dict(a=1))
>>> x = X()
>>> x
<__main__.X object at 0x00DCE5F0>
>>> x.a
1

See Also
========
#TODO