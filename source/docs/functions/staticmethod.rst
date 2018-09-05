============
staticmethod
============

Description
===========
Returns a static method for function.

Syntax
======
**staticmethod** *(function)*

*function*
	Required. Function to be decorated.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
A static method does not receive an implicit first argument. When function decorated with @staticmethod is called, we don't pass an instance of the class to it (as we normally do with methods). This means we can put a function inside a class but we can't access the instance of that class (this is useful when your method does not use the instance).

staticmethods can be used when the code that belongs to a class doesn't use the object itself at all. Python doesn't have to instantiate a bound method for each object we instantiate. Bound methods are objects too, and creating them has a cost. Having a static method avoids that. There are very few situations where static-methods are necessary in Python.

The @staticmethod form is a function decorator.

Also see classmethod() for a variant that is useful for creating alternate class constructors.

Example 1
=========
>>> class Foo:
...     @staticmethod
...     def bar():
...         print 'bar'
...
>>> Foo.bar
<function bar at 0x00DBC1B0>
>>> Foo().bar
<function bar at 0x00DBC1B0>
>>> Foo.bar()
bar
>>> Foo().bar()
bar

Example 2
=========
>>> # this example uses obsolete no-decorator syntax
>>> class Foo:
...     def bar():
...         print 'bar'
...     bar = staticmethod(bar)
...
>>> Foo.bar
<function bar at 0x00DBC270>
>>> Foo().bar
<function bar at 0x00DBC270>
>>> Foo().bar()
bar
>>> Foo.bar()
bar*
	

See Also
========
#TODO
