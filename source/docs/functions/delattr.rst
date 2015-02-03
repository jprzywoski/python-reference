=======
delattr
=======

Description
===========
Deletes the named attribute of an object.

Syntax
======
**delattr** *(object, name)*

*object*
	Required. The name of the object which attribute will be deleted. Must be an object.
*name*
	Required. The name of the attribute to delete. Must be a string.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
See also setattr().

Example
=======
>>> class Foo:
...     def __init__(self, x=0):
...         self.x = x
...
>>> f = Foo(10)
>>> f.x
10
>>> delattr(f, 'x')
>>> f.x
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
AttributeError: Foo instance has no attribute 'x'

See Also
========
#TODO
