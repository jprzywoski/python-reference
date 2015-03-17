======
co_cellvars
======

Description
===========
Returns a tuple containing the names of local variables that are referenced by nested functions. 

Syntax
======
code.co_cellvars

Return Value
============
#TODO

Time Complexity
===============
#TODO

Example
=======
>>> def foo():
...     a = 10
...     def bar():
...         return a
...     return bar()
... 
>>> c = foo.func_code
>>> c.co_cellvars
('a',) 

See Also
========
#TODO
