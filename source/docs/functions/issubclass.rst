==========
issubclass
==========

Description
===========
Returns a Bool type indicating whether an object is a subclass of a class.

Syntax
======
**issubclass** *(class, classinfo)*

*class*
	Required. A class.
*classinfo*
	Required. A class, type or a tuple of classes and/or types.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
A class is considered a subclass of itself. classinfo may be a tuple of class objects, in which case every entry in classinfo will be checked. In any other case, a TypeError exception is raised.

Example
=======
>>> class Foo: pass
...
>>> class Bar(Foo): pass
...
>>> class Snafu: pass
...
>>> issubclass(Bar, Foo)
True
>>> issubclass(Bar, Snafu)
False
>>> issubclass(Foo, Foo)
True
>>> issubclass(Bar, (Foo, Snafu))
True

See Also
========
#TODO