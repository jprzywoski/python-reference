==========
isinstance
==========

Description
===========
Returns a Boolean stating whether the object is an instance or subclass of another object.

Syntax
======
**isinstance** *(object, classinfo)*

*object*
	Required. An object instance.
*classinfo*
	Required. A class, type or a tuple containing classes, types or other tuples.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Also returns True if classinfo is a type object (new-style class) and object is an object of that type or of a (direct, indirect or virtual) subclass thereof. If object is not a class instance or an object of the given type, the function always returns false. If classinfo is neither a class object nor a type object, it may be a tuple of class or type objects, or may recursively contain other such tuples (other sequence types are not accepted). If classinfo is not a class, type, or tuple of classes, types, and such tuples, a TypeError exception is raised.

Example 1
=========
>>> isinstance('foo', basestring)
True
>>> isinstance('foo', float)
False

Example 2
=========
>>> class Foo: pass
...
>>> class Bar(Foo): pass
...
>>> b = Bar()
>>> isinstance(b, Foo)
True
>>> isinstance(Bar, Foo)
False
>>> isinstance(Bar(), Foo)
True

Example 3
=========
>>> isinstance(u'foo', (basestring, str, unicode))
True
>>> isinstance(u'foo', (basestring, str))
True
>>> isinstance(u'foo', (basestring))
True
>>> isinstance(u'foo', (str))
False

See Also
========
#TODO
