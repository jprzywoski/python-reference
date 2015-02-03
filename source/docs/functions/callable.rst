========
callable
========

Description
===========
Returns a Boolean stating whether the object argument appears callable.

Syntax
======
**callable** *(object)*

*object*
	Required. Any valid object.

Return Value
============
#TODO

Time Complexity
============
#TODO

Note
====
If callable() returns True, it is still possible that a call fails, but if it is False, calling object will never succeed. Note that classes are callable (calling a class returns a new instance); class instances are callable if they have a __call__() method.

Example
=======
>>> def bar(): pass
...
>>> callable(bar)
True
>>> class foo: pass
...
>>> callable(foo)
True
>>> callable(10)
False
>>> callable('hello')
False
>>> callable(True)
False

See Also
========
#TODO