=====
strip
=====

Description
----------
Returns a copy of the string with the leading and trailing characters removed.

Syntax
------
**str**. *strip([chars])*

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

Example 1
---------
>>> '   spacious   '.strip()
'spacious'
>>> "AABAA".strip("A")
'B'
>>> "ABBA".strip("AB")
''
>>> "ABCABBA".strip("AB")
'C'

Example 2
---------
>>> 'www.example.com'.strip('cmowz.') # this example extracts web address
'example'

See Also
--------
`lstrip()`_ and `rstrip()`_

.. _lstrip(): ../str/lstrip.html
.. _rstrip(): ../str/rstrip.html
.. _strip(): ../str/strip.html
