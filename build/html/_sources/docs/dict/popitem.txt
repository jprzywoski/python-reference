=======
popitem
=======

Description
===========
Removes and returns an arbitrary (key, value) pair from the dictionary.

Syntax
======
**dict**. *popitem()*

Return Value
============
**tuple**

Time Complexity
===============
#TODO

Remarks
=======
*popitem()* is useful to destructively iterate over a dictionary, as often used in set algorithms. If the dictionary is empty, calling *popitem()* raises a KeyError.

Example
=======
>>> d = {'a': 1, 'b': 2}
>>> d.popitem()
('a', 1)
>>> d.popitem()
('b', 2)
>>> d.popitem()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
KeyError: 'popitem(): dictionary is empty'

See Also
========
#TODO
