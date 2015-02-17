====
. (attribute access)
====

Description
====
Gives access to an object's attribute.

Syntax
====
object.attribute

*object*
    Any object.
*attribute*
    The attribute to be accessed or created.
    
Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
====
Note that Python is a dynamic language and attributes can be accessed and created explicitly.

Example 1
====
>>> "ABCD".islower()
False

Example 2
====
>>> # this example adds a new attribute to a class instance
>>> class Example:
...     pass
... 
>>> e = Example()
>>> e.dummy = 10

See Also
========
#TODO