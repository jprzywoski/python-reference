=======
getattr
=======

Description
===========
Returns the value of the named attribute of object.

Syntax
======
**getattr** *(object, name[, default])*

*object*
	Required. An object whose attribute is to be returned.
*name*
	Required. Must be a string. If the named attribute does not exist, default is returned if provided, otherwise AttributeError is raised.
*default*
	Optional. Default value returned if the named attribute does not exist.

Return Value
============
#TODO

Time Complexity
============
#TODO

Example
=======
>>> class Foo:
...     def __init__(self, x):
...         self.x = x
...
>>> f = Foo(10)
>>> getattr(f, 'x')
10
>>> f.x
10
>>> getattr(f, 'y', 'bar')
'bar'

See Also
========
#TODO