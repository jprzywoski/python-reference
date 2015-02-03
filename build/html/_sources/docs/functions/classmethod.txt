===========
classmethod
===========

Description
===========
Returns a class method for the function.

Syntax
======
**classmethod** *(class)*

*class*
	Required. Name of a class.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
When classmethod is called, it gets the class as the first argument instead of the instance of that class (as we normally do with methods). This means we can use the class and its properties inside that method rather than a particular instance.
Class methods are useful when you need to have methods that aren't specific to any particular instance, but still involve the class in some way.
If we have a class, and a module-level function that operates on that class (factory, dependency injection stub, etc), make it a classmethod. Then it'll be available to subclasses.
Class methods can be overridden by subclasses unlike Python's module-level functions.
The @classmethod form is a function decorator.
See also staticmethod(), property() and abstract class in abc module.

Example 1
=========
>>> #This example shows obsolete syntax
>>> #Note that method bar can be called on both class and instance objects
>>> class Foo:
...     def bar(cls):             #
...         print 'bar’           #
...     bar = classmethod(bar)    #<= not pythonic anymore, decorator syntax recommended
...
>>> Foo.bar
<bound method classobj.bar of <class __main__.Foo at 0x00CDAC00>>
>>> Foo.bar()
bar
>>> Foo().bar
<bound method classobj.bar of <class __main__.Foo at 0x00CDAC00>>
>>> Foo().bar()
bar

Example 2
=========
>>> #This example shows usage of decorator syntax which is recommended
class Line:
    def __init__(self, length):
        self.length = length

    @classmethod
    def from_inches(cls, length_in):
        length = float(length_in)*2.54
        return cls(length)

l = Line.from_inches(3)
print l.length         #returns 7.62

See Also
========
#TODO