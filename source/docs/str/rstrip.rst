======
rstrip
======

Description
----------
Returns a copy of the string with trailing characters removed.

Syntax
------
**str**. *rstrip([chars])*

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
>>> '   spacious   '.rstrip()
'   spacious'
>>> "AABAA".rstrip("A")
'AAB'
>>> "ABBA".rstrip("AB") # both AB and BA are stripped
''
>>> "ABCABBA".rstrip("AB")
'ABC'

See Also
--------
`strip()`_ and `lstrip()`_

.. _lstrip(): ../str/lstrip.html
.. _rstrip(): ../str/rstrip.html
.. _strip(): ../str/strip.html
