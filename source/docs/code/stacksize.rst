======
co_stacksize
======

Description
===========
Returns the required stack size (including local variables).

Syntax
======
code.co_stacksize

Return Value
============
#TODO

Time Complexity
===============
#TODO

Example
=======
>>> c = compile('a = 2+2; b=10', '<string>', 'exec')
>>> c.co_stacksize
2 

See Also
========
#TODO
