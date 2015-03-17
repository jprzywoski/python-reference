======
func_doc
======

Description
===========
Returns the function’s documentation string, or None if unavailable. 

Syntax
======
type.func_doc

Return Value
============
#TODO

Time Complexity
===============
#TODO

Remarks
====
The func_doc attribute is writeable.

Example 1
=======
>>> def foo():
...     ''' This is my docstring.'''
...     pass
... 
>>> foo.func_doc
' This is my docstring.' 

Example 2
=======
>>> def foo():
...     ''' This is my docstring.'''
...     pass
>>> 
>>> foo.func_doc = 'foobar'
>>> foo.func_doc
'foobar'

See Also
========
#TODO
