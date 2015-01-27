=====
split
=====

Description
----------
Returns a list of the words in the string, separated by the delimiter string.

Syntax
------
**str**. *split([sep[, maxsplit]])*

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

Remarks
-------
If *sep* is given, consecutive delimiters are not grouped together and are deemed to delimit empty strings (for example, 

>>> '1,,2'.split(',')

returns ['1', '', '2']). The *sep* argument may consist of multiple characters (for example, 

>>> '1<>2<>3'.split('<>') 

returns ['1', '2', '3']). Splitting an empty string with a specified separator returns [''].

If *sep* is not specified or is **None**, a different splitting algorithm is applied: runs of consecutive whitespace are regarded as a single separator, and the result will contain no empty strings at the start or end if the string has leading or trailing whitespace. Consequently, splitting an empty string or a string consisting of just whitespace with a **None** separator returns [].

Example 1
---------
>>> ' a b c '.split()
['a', 'b', 'c']
>>> ' a b c '.split(None)
['a', 'b', 'c']
>>> ' a b c '.split(' ', 1)
['', 'a b c ']
>>> ' a b c '.split(' ', 2)
['', 'a', 'b c ']
>>> ' a b c '.split(' ', 3)
['', 'a', 'b', 'c ']
>>> ' a b c '.split(' ', 4)
['', 'a', 'b', 'c', '']
>>> ' a b c '.split(' ', 5)
['', 'a', 'b', 'c', '']

Example 2
---------
>>> '-a-b-c-'.split('-')
['', 'a', 'b', 'c', '']
>>> '-a-b-c-'.split('-', 1)
['', 'a-b-c-']
>>> '-a-b-c-'.split('-', 2)
['', 'a', 'b-c-']
>>> '-a-b-c-'.split('-', 3)
['', 'a', 'b', 'c-']
>>> '-a-b-c-'.split('-', 4)
['', 'a', 'b', 'c', '']
>>> '-a-b-c-'.split('-', 5)
['', 'a', 'b', 'c', '']

Example 3
---------
>>> '----a---b--c-'.split('-')
['', '', '', '', 'a', '', '', 'b', '', 'c', '']
>>> '----a---b--c-'.split('-', 1)
['', '---a---b--c-']
>>> '----a---b--c-'.split('-', 2)
['', '', '--a---b--c-']
>>> '----a---b--c-'.split('-', 3)
['', '', '', '-a---b--c-']
>>> '----a---b--c-'.split('-', 4)
['', '', '', '', 'a---b--c-']
>>> '----a---b--c-'.split('-', 5)
['', '', '', '', 'a', '--b--c-']
>>> '----a---b--c-'.split('-', 6)
['', '', '', '', 'a', '', '-b--c-']

See Also
--------
`rsplit()`_ for version that splits from the right

.. _split(): ../str/split.html
.. _rsplit(): ../str/rsplit.html
