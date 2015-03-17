======
co_firstlineno
======

Description
===========
Returns the first line number of the function. 

Syntax
======
code.co_firstlineno

Return Value
============
#TODO

Time Complexity
===============
#TODO

Example
=======
>>> def foo():
...     print 'bar'
...     
>>> c = foo.func_code
>>> c.co_firstlineno
1

See Also
========
#TODO
