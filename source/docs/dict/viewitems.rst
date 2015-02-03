=========
viewitems
=========

Description
===========
Returns a new view of the dictionary’s items ((key, value) pairs).

Syntax
======
**dict**. *viewitems()*

Return Value
============
**dict_items** object

Time Complexity
===============
#TODO

Remarks
=======
The objects returned by dict.viewkeys(), dict.viewvalues() and dict.viewitems() are view objects. They provide a dynamic view on the dictionary’s entries, which means that when the dictionary changes, the view reflects these changes.

Example
=======
>>> d = {'a': 1, 'b': 2}
>>> dv = d.viewitems()
>>> dv
dict_items([('a', 1), ('b', 2)])
>>> d['a'] = 'foobar'
>>> d
{'a': 'foobar', 'b': 2}
>>> dv                                   #note that the view returns the
dict_items([('a', 'foobar'), ('b', 2)])  #current contents of the dictionary

See Also
========
See dict views set operators.
