======
func_dict
======

Description
===========
Returns the namespace supporting arbitrary function attributes.

Syntax
======
function.func_dict

Return Value
============
#TODO

Time Complexity
===============
#TODO

Remarks
====
The func_dict attribute is writeable.

Example 1
=======
>>> def foo(): pass
... 
>>> foo.x = 10
>>> foo.func_dict
{'x': 10}

Example 2
=======
>>> def foo(): pass
... 
>>> foo.func_dict = {'a': 1, 'bamf': 10}
>>> foo.func_dict
{'a': 1, 'bamf': 10}

See Also
========
#TODO
