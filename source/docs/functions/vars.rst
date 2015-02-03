====
vars
====

Description
===========
Returns the mapping of an object’s (writable) attributes.

Syntax
======
**vars** *([object])*

*object*
	Optional. An object with __dict__() special attribute.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Objects such as modules and instances have an updateable __dict__ attribute; however, other objects may have write restrictions on their __dict__ attributes (for example, new-style classes use a dictproxy to prevent direct dictionary updates).

Without an argument, vars() acts like locals(). Note, the locals dictionary is only useful for reads since updates to the locals dictionary are ignored.

Example 1
=========
>>> vars()
{'Foo': <class '__main__.Foo'>,
 '__builtins__': <module '__builtin__' (built-in)>,
 '__doc__': None,
 '__name__': '__main__',
 '__package__': None,
 'f': <__main__.Foo object at 0x02BF35F0>,
 'pyscripter': <module 'pyscripter' (built-in)>}

Example 2
=========
>>> class Foo:
...     x = 10
...     y = 20
...
>>> vars(Foo)
{'__doc__': None, '__module__': '__main__', 'x': 10, 'y': 20}

See Also
========
#TODO