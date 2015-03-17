======
co_lnotab
======

Description
===========
Returns a string encoding the mapping from bytecode offsets to line numbers.

Syntax
======
code.co_lnotab

Return Value
============
#TODO

Time Complexity
===============
#TODO

Remarks
====
For details see the source code of the interpreter.

Example
=======
>>> c = compile('a = 2+2; b=10', '<string>', 'exec')
>>> c.co_lnotab
'\x06\x00'

See Also
========
#TODO
