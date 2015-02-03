=======
hasattr
=======

Description
===========
Returns a Boolean stating whether the object has the specified attribute.

Syntax
======
**hasattr** *(object, name)*

*object*
	Required. Any object.
*name*
	Required. String representation of the attribute.

Return Value
============
#TODO

Time Complexity
============
#TODO

Example
=======
>>> class Foo:
...     pass
...
>>> f = Foo()
>>> hasattr(f, 'x')
False
>>> f.x = 5
>>> hasattr(f, 'x')
True

See Also
========
#TODO