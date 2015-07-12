====
__setattr__
====

Description
====
Called when an attribute assignment is attempted.

Syntax
====
**object**. *__setattr__(self, name, value)*

*self*
    Required. Instance of the class, passed automatically on call.
*name*
    Required. The name of the attribute.
*value*
    Required. The value we want to assign to the attribute.

Return Value
====
#TODO

Time Complexity
====
#TODO

Remarks
====
This method is called instead of the normal mechanism (i.e. store the value in the instance dictionary).

If __setattr__() wants to assign to an instance attribute, it should not simply execute self.name = value — this would cause a recursive call to itself.

Instead, it should insert the value in the dictionary of instance attributes, e.g., self.__dict__[name] = value.

For new-style classes, rather than accessing the instance dictionary, it should call the base class method with the same name, for example,

>>> object.__setattr__(self, name, value).

Example
====
>>> # this example uses __setattr__ to dynamically change attribute value to uppercase
>>> class Frob:
...     def __setattr__(self, name, value):
...         self.__dict__[name] = value.upper()
...         
>>> f = Frob()
>>> f.bamf = "bamf"
>>> f.bamf
'BAMF'
