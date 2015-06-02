====
__getattribute__
====

Description
====
Called unconditionally to implement attribute accesses for instances of the class.

Syntax
====
**object**. *__getattribute__(self, name)*

*self*
    Required. Instance of the class, passed automatically on call.
*name*
    Required. The name of the attribute.

Return Value
====
#TODO

Time Complexity
====
#TODO

Remarks
====
The following method only applies to new-style classes.

If the class also defines __getattr__(), the latter will not be called unless __getattribute__() either calls it explicitly or raises an AttributeError.

This method should return the (computed) attribute value or raise an AttributeError exception.

In order to avoid infinite recursion in this method, its implementation should always call the base class method with the same name to access any attributes it needs, for example, 

>>> object.__getattribute__(self, name).

Note
====
This method may still be bypassed when looking up special methods as the result of implicit invocation via language syntax or built-in functions. See Special method lookup for new-style classes.

Example
====
>>> class Frob(object):
...     def __getattribute__(self, name):
...         print "getting `{}`".format(str(name))
...         object.__getattribute__(self, name)
... 
>>> f = Frob()
>>> f.bamf = 10
>>> f.bamf
getting `bamf`
