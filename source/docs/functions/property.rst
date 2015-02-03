========
property
========

Description
===========
Returns a property attribute for new-style classes (classes that derive from object).

Syntax
======
**property** *([fget[, fset[, fdel[, doc]]]])*

*fget*
	Optional. Function for getting an attribute value.
*fset*
	Optional. Function for setting an attribute value.
*fdel*
	Optional. Function for deleting an attribute value.
*doc*
	Optional. The docstring of the property attribute. If omitted, the property will copy fget‘s docstring (if it exists).

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Property decorator allows a class’ attribute to be managed, validated, proxied, secured, or protected in any other way from direct access.
Typical use of property()is to define a managed attribute:

Example 1
=========
class C(object):
    def __init__(self):
        self._x = None

    def getx(self):
        return self._x
    def setx(self, value):
        self._x = value
    def delx(self):
        del self._x
    x = property(getx, setx, delx, "I'm the 'x' property.")
    
If then c is an instance of C, c.x will invoke the getter, c.x = value will invoke the setter and del c.x the deleter.
If given, doc will be the docstring of the property attribute. Otherwise, the property will copy fget‘s docstring (if it exists). This makes it possible to create read-only properties easily using property() as a decorator:

Example 2
=========
class Parrot(object):
    def __init__(self):
        self._voltage = 100000

    @property
    def voltage(self):
        """Get the current voltage."""
        return self._voltage
turns the voltage() method into a “getter” for a read-only attribute with the same name.
A property object has getter, setter, and deleter methods usable as decorators that create a copy of the property with the corresponding accessor function set to the decorated function. This is best explained with an example:

Example 3
=========
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

See Also
========
#TODO
