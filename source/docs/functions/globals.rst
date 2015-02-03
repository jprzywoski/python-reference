=======
globals
=======

Description
===========
Returns a dictionary representing the current global symbol table.

Syntax
======
**globals()**

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Returned value is always the dictionary of the current module (inside a function or method, this is the module where it is defined, not the module from which it is called).

Example
=======
>>> globals()
{'__builtins__': <module '__builtin__' (built-in)>,
 '__doc__': None,
 '__name__': '__main__',
 '__package__': None,
 'pyscripter': <module 'pyscripter' (built-in)>}

See Also
========
#TODO