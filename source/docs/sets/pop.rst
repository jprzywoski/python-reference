===
pop
===

Description
===========
Removes and returns an arbitrary element from the set. 

Syntax
======
**set**. *pop()*

Return Value
============
The same as deleted by calling this method.

Time Complexity
===============
#TODO

Remarks
=======
Raises KeyError if the set is empty.

Example
=======
>>> s = {1, 2}
>>> s.pop()
1
>>> s
set([2])
>>> s.pop()
2
>>> s.pop()
KeyError: 'pop from an empty set'

See also
========
#TODO

