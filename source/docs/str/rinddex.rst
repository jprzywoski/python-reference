======
rindex
======

Description
----------
Returns the index of the first occurrence of the string searched for (raises *ValueError* if not found).

Syntax
------
**str**. *rindex(sub[, start[, end]])*

*sub*
    Required. The string searched for.
*start*
    Optional. Search start position.
*end*
    Optional. Search end position.

Return Value
------------
**int**

Time Complexity
---------------
#TODO

Example
-------
>>> "ABAB".rindex("B")
3
>>> "ABAB".rindex("B", 2, 4)
3
>>> "ABAB".rindex("B", 2)
3
>>> "ABAB".rindex("C")
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
ValueError: substring not found

See Also
--------
`find()`_

`rfind()`_

`index()`_


.. _find(): ../bd_strings/find.html
.. _rfind(): ../bd_strings/rfind.html
.. _index(): ../bd_strings/strindex.html
