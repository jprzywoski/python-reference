=========
iteritems
=========

Description
===========
Returns an iterator over the dictionary’s (key, value) pairs.

Syntax
======
**dict**. *iteritems()*

Return Value
============
**iterator**

Time Complexity
===============
#TODO

Remarks
=======
See also dict.items().
Using iteritems() while adding or deleting entries in the dictionary may raise a RuntimeError or fail to iterate over all entries.

Example 1
=========
>>> d = {'a': 1, 'b': 2}
>>> di = d.iteritems()
>>> di.next()
('a', 1)
>>> di.next()
('b', 2)
>>> di.next()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
StopIteration

Example 2
=========
>>> d = {'a': 1, 'b': 2}
>>> di = d.iteritems()
>>> di.next()
('a', 1)
>>> d['x'] = 'foobar'     # adding a new key:value pair during iterarion;
>>> di.next()             # that raises an error later on
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
RuntimeError: dictionary changed size during iteration

