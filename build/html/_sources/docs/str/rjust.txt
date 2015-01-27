=====
rjust
=====

Description
----------
Returns the string right justified in a string of specified length.

Syntax
------
**str**. *rjust(width[, fillchar])*

*width*
    Required. The width of the field containing the string.
*fillchar*
    Optional. Specifies the padding character (default is a space).

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Remarks
-------
The original string is returned if *width* is less than or equal to **len(str)**.

Example
-------
>>> "ABC".rjust(10)
'       ABC'
>>> "ABC".rjust(10, "#")
'#######ABC'
>>> "ABC".rjust(2, "#")
'ABC'

See Also
--------
`ljust()`_, `rjust()`_, `center()`_

.. _ljust(): ../str/ljust.html
.. _center(): ../str/center.html
.. _rjust(): ../str/rjust.html
