========
iterkeys
========

Description
===========
Returns an iterator over the dictionary’s keys.

Syntax
======
**dict**. *iterkeys()*

Return Value
============
**iterator**

Time Complexity
===============
#TODO

Remarks
=======
See also dict.items().
Using iterkeys() while adding or deleting entries in the dictionary may raise a RuntimeError or fail to iterate over all entries.

Example 1
=========
>>> d = {'a': 1, 'b': 2}
>>> dki = d.iterkeys()
>>> dki.next()
'a'
>>> dki.next()
'b'
>>> dki.next()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
StopIteration

Example 2
=========
>>> d = {'a': 1, 'b': 2}
>>> dki = d.iterkeys()
>>> dki.next()
'a'
>>> d['x'] = 'foobar'      # adding a new key:value pair during iterarion
>>> dki.next()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
RuntimeError: dictionary changed size during iteration 
