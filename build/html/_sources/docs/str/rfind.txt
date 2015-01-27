=====
rfind
=====

Description
----------
Returns the index of the last occurrence of the string searched for.

Syntax
------
**str**. *rfind(sub[, start[, end]])*

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

Remarks
-------
Returns -1 if *sub* is not found.

The rfind() method should be used only if you need to know the position of *sub*. To check if *sub* is a substring or not, use the **in** operator:

>>> 'Py' in 'Python'
True

Example
-------
>>> "ABAB".rfind("B")
3
>>> "ABAB".rfind("B", 0, 2)
1
>>> "ABAB".rfind("B", 2)
3

See Also
--------
`rfind()`_

`index()`_

`rindex()`_

.. _find(): ../bd_strings/find.html
.. _index(): ../bd_strings/strindex.html
.. _rindex(): ../bd_strings/rinddex.html
