====
__set__
====

Description
====
Called to set the attribute on an instance instance of the owner class to a new value, value.

Syntax
====
**object**. *__set__(self, instance, value)*

*self*
    Required. Instance of the class, passed automatically on call.
*instance*
    Required. Instance is the instance that the attribute was accessed through, or None when the attribute is accessed through the owner.
*value*
    Required. The value we want to assign to the attribute.

Remarks
====
The following method only apply to new-style classes.

The following methods only apply when an instance of the class containing the method (a so-called descriptor class) appears in an owner class (the descriptor must be in either the owner’s class dictionary or in the class dictionary for one of its parents).

Example
====
::

    # this is our descriptor object
    class Bar(object):
        def __init__(self):
            self.value = ''
        def __get__(self, instance, owner):
            print "returned from descriptor object"
            return self.value
        def __set__(self, instance, value):
            print "set in descriptor object"
            self.value = value
        def __delete__(self, instance):
            print "deleted in descriptor object"
            del self.value

    class Foo(object):
        bar = Bar()

    f = Foo()
    f.bar = 10
    print f.bar
    del f.bar

    set in descriptor object
    returned from descriptor object
    10
    deleted in descriptor object
