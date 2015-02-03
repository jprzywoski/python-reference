=====
apply
=====

Description
===========
Returns the result of a function or class object called with supplied arguments.

Syntax
======
**apply** *(function, args[, kwargs])*

*function*
	Required. The function argument must be a callable object (a user-defined or built-in function or method, or a class object).
*args*
	Required. A sequence of positional arguments.
*kwargs*
	Optional. The kwargs argument must be a dictionary whose keys are strings. It specifies keyword arguments to be added to the end of the argument list.

Return Value
============
#TODO

Time Complexity
============
#TODO

Note
====
This function is obsolete. Use function(*args, **kwargs) instead of apply(function, args, kwargs).

Example 1
=========
>>> def foo(a, b):
...     return a, b
...
>>> apply(foo, (1, 2))
(1, 2)

Example 2
=========
>>> def bar(a, b, c=None):
...     return a, b, c
...
>>> apply(bar, (1, 2), {'c': 3})
(1, 2, 3)

See Also
========
#TODO