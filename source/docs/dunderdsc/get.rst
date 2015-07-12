====
__get__
====

Description
====
Called to get the attribute of the owner class (class attribute access) or of an instance of that class (instance attribute access).

Syntax
====
**object**. *__get__(self, instance, owner)*

*self*
    Required. Instance of the class, passed automatically on call.
*instance*
    Required. Instance is the instance that the attribute was accessed through, or None when the attribute is accessed through the owner.
*owner*
    Required. Owner is always the owner class.

Remarks
====
The following method only applies to new-style classes.

The following methods only apply when an instance of the class containing the method (a so-called descriptor class) appears in an owner class (the descriptor must be in either the owner’s class dictionary or in the class dictionary for one of its parents).

This method should return the (computed) attribute value or raise an AttributeError exception.

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
