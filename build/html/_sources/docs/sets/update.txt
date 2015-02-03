======
update
======

Description
===========
Adds elements to the set.

Syntax
======
**set**. *update(other, ...)*

*other, ...*
    Required. Iterable or multiple iterables which elements are to be added to the set. The elements must be hashable.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> s = {1, 2}
>>> s.update({3, 4}, [5, 6])
>>> s
set([1, 2, 3, 4, 5, 6])

See also
========
#TODO

