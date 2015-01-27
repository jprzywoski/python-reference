=======
replace
=======

Description
----------
Returns a copy of the string with a specified substring replaced specified number of times.

Syntax
------
**str**. *replace(old, new[, count])*

*old*
    Required. String to be replaced.
*new*
    Optional. String to replace the old one.
*count*
    Optional. Number of *old* occurrences to replace.

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Example
-------
>>> "ABCAB".replace('AB', 'ab')
'abCab'
>>> "ABCAB".replace('YZ', 'ab')
'ABCAB'
>>> "ABCAB".replace('AB', 'ab', 1)
'abCAB'
>>> "ABCAB".replace('AB', 'ab', 2)
'abCab'

See Also
--------
`str.translate()`_

.. _str.translate(): ../bd_strings/translate.html