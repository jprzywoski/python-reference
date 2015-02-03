=====
super
=====

Description
===========
Returns a proxy object that delegates method calls to a parent or sibling class of type.

Syntax
======
**super** *(type[, object-or-type])*

*type*
	Required.
*object-or-type*
	Optional.

Return Value
============
#TODO

Time Complexity
============
#TODO

Note
====
super() only works for new-style classes.

Remarks
=======
super() is useful for accessing inherited methods that have been overridden in a class. The search order is same as that used by getattr() except that the type itself is skipped.

The __mro__ attribute of the type lists the method resolution search order used by both getattr() and super(). The attribute is dynamic and can change whenever the inheritance hierarchy is updated.

If the second argument is omitted, the super object returned is unbound. If the second argument is an object, isinstance(obj, type) must be true. If the second argument is a type, issubclass(type2, type) must be true (this is useful for classmethods).

There are two typical use cases for super. In a class hierarchy with single inheritance, super can be used to refer to parent classes without naming them explicitly, thus making the code more maintainable. This use closely parallels the use of super in other programming languages.

The second use case is to support cooperative multiple inheritance in a dynamic execution environment. This use case is unique to Python and is not found in statically compiled languages or languages that only support single inheritance. This makes it possible to implement “diamond diagrams” where multiple base classes implement the same method. Good design dictates that this method have the same calling signature in every case (because the order of calls is determined at runtime, because that order adapts to changes in the class hierarchy, and because that order can include sibling classes that are unknown prior to runtime).

For both use cases, a typical superclass call looks like this:

>>> class C(B):
>>>     def method(self, arg):
>>>         super(C, self).method(arg)
        
Note that super() is implemented as part of the binding process for explicit dotted attribute lookups such as super().__getitem__(name). It does so by implementing its own __getattribute__() method for searching classes in a predictable order that supports cooperative multiple inheritance. Accordingly, super() is undefined for implicit lookups using statements or operators such as super()[name].
Also note that super() is not limited to use inside methods. The two argument form specifies the arguments exactly and makes the appropriate references.

For practical suggestions on how to design cooperative classes using super(), see guide to using super().

Example
=======
>>> class Foo(object):
...     def fb(self):
...         print 'foo'
...
>>> class Bar(Foo):
...     def fb(self):
...         super(Bar, self).fb()
...         print 'bar'
...
>>> f = Foo()
>>> f.fb()
foo
>>> b = Bar()
>>> b.fb()
foo
bar

See Also
========
#TODO