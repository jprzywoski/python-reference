======
co_nlocals
======

Description
===========
Returns the number of local variables used by the function (including arguments).

Syntax
======
code.co_nlocals

Return Value
============
#TODO

Time Complexity
===============
#TODO

Example
=======
>>> def foo(a, b=10):
...     c = 10
...     return a+b+c
... 
>>> c = foo.func_code
>>> c.co_nlocals
3

See Also
========
#TODO
