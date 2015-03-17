======
func_defaults
======

Description
===========
Returns a tuple containing default argument values for those arguments that have defaults, or None if no arguments have a default value.

Syntax
======
function.func_defaults

Return Value
============
**tuple**

Time Complexity
===============
#TODO

Remarks
====
The func_defaults attribute is writeable.

Example
=======
>>> def foo(a, b='bar'): pass
... 
>>> foo.func_defaults
('bar',) 
EXAMPLE 2
>>> def foo(a, b='bar'): pass
... 
>>> foo.func_defaults = 'bamf', 
>>> foo.func_defaults
('bamf',)

See Also
========
#TODO
