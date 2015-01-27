======
rsplit
======

Description
----------
Returns a list of the words in the string, separated by the delimiter string (starting from right).

Syntax
------
**str**. *rsplit([sep[, maxsplit]])*

*sep*
    Optional. Character dividing the string into split groups; default is space.
*maxsplit*
    Optional. Number of splits to do; default is -1 which splits all the items.

Return Value
------------
**list**

Time Complexity
---------------
#TODO

Example 1
---------
>>> ' a b c '.rsplit()
['a', 'b', 'c']
>>> ' a b c '.rsplit(None, 1)
[' a b', 'c']
>>> ' a b c '.rsplit(None, 2)
[' a', 'b', 'c']
>>> ' a b c '.rsplit(None, 3)
['a', 'b', 'c']
>>> ' a b c '.rsplit(None, 4)
['a', 'b', 'c']
>>> ' a b c '.rsplit(None, 5)
['a', 'b', 'c']

Example 2
---------
>>> '----a---b--c-'.rsplit('-')
['', '', '', '', 'a', '', '', 'b', '', 'c', '']
>>> '----a---b--c-'.rsplit('-', 1)
['----a---b--c', '']
>>> '----a---b--c-'.rsplit('-', 2)
['----a---b-', 'c', '']
>>> '----a---b--c-'.rsplit('-', 3)
['----a---b', '', 'c', '']
>>> '----a---b--c-'.rsplit('-', 4)
['----a--', 'b', '', 'c', '']
>>> '----a---b--c-'.rsplit('-', 5)
['----a-', '', 'b', '', 'c', '']
>>> '----a---b--c-'.rsplit('-', 6)
['----a', '', '', 'b', '', 'c', '']

See Also
--------
`split()`_

.. _split(): ../str/split.html
.. _rsplit(): ../str/rsplit.html