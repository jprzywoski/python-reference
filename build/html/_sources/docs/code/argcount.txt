======
co_argcount
======

Description
===========
Returns the number of positional arguments (including arguments with default values).

Syntax
======
code.co_argcount

Return Value
============
#TODO

Time Complexity
===============
#TODO

Example
=======
>>> def foo(a, b=10): pass
... 
>>> c = foo.func_code
>>> c.co_argcount
2

See Also
========
#TODO
