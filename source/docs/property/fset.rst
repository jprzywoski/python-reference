====
fset
====

Description
====
Overrides attribute access mechanism.

Syntax
====
property.fset

Return Value
====
None

Time Complexity
====
#TODO

Remarks
====
fget is a function for getting an attribute value, likewise fset is a function for setting, and fdel a function for del’ing, an attribute. Typical use is to define a managed attribute x:

::

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
