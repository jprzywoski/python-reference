====
@ Decorator Operator
====

Description
====
Returns a callable wrapped by another callable.

Syntax
====
@decorator
def function():
    suite

*decorator*
    A callable that takes another callable as an argument.
    
Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
====

Decorator syntax

>>> def decorator(f):
...     pass
... 
>>> @decorator
... def function():
...     pass

is equivalent to:

>>> def function():
...     pass
>>> function = decorator(function)

Example
====
>>> # this example shows how to use a decorator to add functionality to a function
>>> def decorator(f):
...     def inner():
...         print('before')
...         retval = f()
...         print('after')
...         return retval
...     return inner
... 
>>> @decorator
... def example():
...     print('inside')
...     
>>> example()
before
inside
after

See Also
========
#TODO