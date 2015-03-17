======
co_names
======

Description
===========
Returns a tuple containing the names used by the bytecode.

Syntax
======
code.co_names

Return Value
============
#TODO

Time Complexity
===============
#TODO

Example
=======
>>> c = compile('a = 2+2; b=10', '<string>', 'exec')
>>> c.co_names
('a', 'b')

See Also
========
#TODO
