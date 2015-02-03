==========
itervalues
==========

Description
===========
Returns an iterator over the dictionary’s values.

Syntax
======
**dict**. *itervalues()*

Return Value
============
**iterator**

Time Complexity
===============
#TODO

Remarks
=======
See the note for dict.items().
Using itervalues() while adding or deleting entries in the dictionary may raise a RuntimeError or fail to iterate over all entries.

Example 1
=========
>>> d = {'a': 1, 'b': 2}
>>> dvi = d.itervalues()
>>> dvi.next()
1
>>> dvi.next()
2
>>> dvi.next()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
StopIteration

Example 2
=========
>>> d = {'a': 1, 'b': 2}
>>> dvi = d.itervalues()
>>> dvi.next()
1
>>> d['x'] = 'foobar'      # adding a new key:value pair during iterarion
>>> dvi.next()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
RuntimeError: dictionary changed size during iteration
