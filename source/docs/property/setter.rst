====
setter
====

Description
====
Overrides attribute access mechanism.

Syntax
====
property.setter(method)

method
    A method to decorate.

Return Value
====
None

Time Complexity
====
#TODO

Remarks
====
A property object has getter, setter, and deleter methods usable as decorators that create a copy of the property with the corresponding accessor function set to the decorated function. This is best explained with an example:

::

    class C(object):
        def __init__(self):
            self._x = None

        @property
        def x(self):
            """I'm the 'x' property."""
            return self._x

        @x.setter
        def x(self, value):
            self._x = value

        @x.deleter
        def x(self):
            del self._x
            
This code is exactly equivalent to the first example. Be sure to give the additional functions the same name as the original property (x in this case.)

The returned property also has the attributes fget, fset, and fdel corresponding to the constructor arguments.

Example
====
>>> c = C()
>>> c.x == None
True
>>> c.x = 'bar'
>>> c.x
'bar'

