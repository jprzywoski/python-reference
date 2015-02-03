===
dir
===

Description
===========
Returns the list of names in the current local scope. If supplied with an argument attempts to return a list of valid attributes for that object.

Syntax
======
**dir** *([object])*

*object*
	Optional. Name of the object which attributes will be displayed.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
If the object has a method named __dir__(), this method will be called and must return the list of attributes. This allows objects that implement a custom __getattr__() or __getattribute__() function to customize the way dir() reports their attributes.
If the object does not provide __dir__(), the function tries its best to gather information from the object’s __dict__ attribute, if defined, and from its type object. The resulting list is not necessarily complete, and may be inaccurate when the object has a custom __getattr__().
The default dir() mechanism behaves differently with different types of objects, as it attempts to produce the most relevant, rather than complete, information:
If the object is a module object, the list contains the names of the module’s attributes.
If the object is a type or class object, the list contains the names of its attributes, and recursively of the attributes of its bases.
Otherwise, the list contains the object’s attributes’ names, the names of its class’s attributes, and recursively of the attributes of its class’s base classes.

Example 1
=========
>>> class Foo:
...     def __init__(self, x):
...         self.x = x
...
>>> dir(Foo)
['__doc__', '__init__', '__module__']

Example 2
=========
>>> dir()
['Foo', '__builtins__', '__doc__', '__name__', '__package__', 'pyscripter']

See Also
========
#TODO
