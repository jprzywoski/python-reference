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

Example 1
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

Example 2
====
>>> # this is actually a useful example - decorator is used to measure
>>> # time taken to execute a function
>>> def timeit(func, *args, **kwargs):
...     def inner(*args, **kwargs):
...         import time
...         start = time.clock()
...         retval = func(*args, **kwargs)
...         finish = time.clock() - start
...         return finish, retval
...     return inner
...
>>> @timeit
... def adder(a):
...    return sum(a)
...
>>> adder(range(10))
(3.682225269585615e-06, 45)
>>> adder(range(1000))
(1.8076378694331652e-05, 499500)
>>> adder(range(1000000))
(0.0833967122414947, 499999500000L)

See Also
========
#TODO