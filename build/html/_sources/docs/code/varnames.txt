======
co_varnames
======

Description
===========
Returns a tuple containing the names of the local variables (starting with the argument names). 

Syntax
======
code.co_varnames

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
>>> c.co_varnames
('a', 'b', 'c')

See Also
========
#TODO
