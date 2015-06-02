====
__delattr__
====

Description
====
Called when an attribute deletion is attempted.

Syntax
====
**object**. *__delattr__(self, name)*

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
Like __setattr__() but for attribute deletion instead of assignment. This should only be implemented if del obj.name is meaningful for the object.

Example
====
>>> class Frob:
...     def __delattr__(self, name):
...         print "deleting `{}`".format(str(name))
...         del self.__dict__[name]
...         print "`{}` deleted".format(str(name))
...         
>>> f = Frob()
>>> f.bamf = 10
>>> del f.bamf
deleting `bamf`
`bamf` deleted
