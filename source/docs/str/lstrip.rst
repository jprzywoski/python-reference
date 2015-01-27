======
lstrip
======

Description
----------
Returns a copy of the string with leading characters removed.

Syntax
------
**str**. *lstrip([chars])*

*chars*
    Optional. String specifying the set of characters to be removed.
    If omitted or None, the chars argument defaults to removing whitespace.
    The *chars* argument is not a prefix; rather, all combinations of its values are stripped.

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Example
-------
>>> '   spacious   '.lstrip()
'spacious   '
>>> "AABAA".lstrip("A")
'BAA'
>>> "ABBA".lstrip("AB") # both AB and BA are stripped
''
>>> "ABCABBA".rstrip("AB")
'ABC'
>>> "ABCABBA".lstrip("AB")
'CABBA'

See Also
--------
`strip()`_ and `rstrip()`_

.. _lstrip(): ../str/lstrip.html
.. _rstrip(): ../str/rstrip.html
.. _strip(): ../str/strip.html
