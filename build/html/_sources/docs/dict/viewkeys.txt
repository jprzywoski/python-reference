========
viewkeys
========

Description
===========
Returns a new view of the dictionary’s keys.

Syntax
======
**dict**. *viewitems()*

Return Value
============
**dict_keys** object

Time Complexity
===============
#TODO

Remarks
=======
Keys views are set-like since their entries are unique and hashable. If all values are hashable, so that (key, value) pairs are unique and hashable, then the items view is also set-like. (Values views are not treated as set-like since the entries are generally not unique.)

Example
=======
>>> d = {'a': 1, 'b': 2}
>>> dk = d.viewkeys()
>>> dk
dict_keys(['a', 'b'])

See Also
========
See dict views set operators.
