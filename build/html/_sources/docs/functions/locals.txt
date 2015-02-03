======
locals
======

Description
===========
Returns a dictionary representing the current local symbol table.

Syntax
======
**locals()**

Return Value
============
#TODO

Time Complexity
============
#TODO

Note
====
The contents of this dictionary should not be modified; changes may not affect the values of local and free variables used by the interpreter.

Example
=======

>>> locals()
{'__builtins__': <module '__builtin__' (built-in)>,
 '__doc__': None,
 '__name__': '__main__',
 '__package__': None,
 'pyscripter': <module 'pyscripter' (built-in)>}
>>> a = 10
>>> locals()
{'__builtins__': <module '__builtin__' (built-in)>,
 '__doc__': None,
 '__name__': '__main__',
 '__package__': None,
 'a': 10,
 'pyscripter': <module 'pyscripter' (built-in)>}

See Also
========
#TODO