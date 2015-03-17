======
co_freevars
======

Description
===========
Returns a tuple containing the names of free variables.

Syntax
======
code.co_freevars

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
>>> c.co_freevars
()

See Also
========
#TODO
