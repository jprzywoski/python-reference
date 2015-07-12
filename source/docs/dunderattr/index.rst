====
Direct Attribute Access
====

The following methods can be defined to customize the meaning of attribute access (use of, assignment to, or deletion of x.name) for class instances.

Methods
====
`\__getattribute__`_
    Called unconditionally to implement attribute accesses for instances of the class.
`\__getattr__`_
    Called when an attribute lookup has not found the attribute in the usual places.
`\__setattr__`_
    Called when an attribute assignment is attempted.
`\__delattr__`_
    Called when an attribute deletion is attempted.
    
.. _\__getattribute__: ./getattribute.html
.. _\__getattr__: ./getattr.html
.. _\__setattr__: ./setattr.html
.. _\__delattr__: ./delattr.html
    