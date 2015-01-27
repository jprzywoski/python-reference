=====
zfill
=====

Description
----------
Returns the numeric string left filled with zeros in a string of specified length.

Syntax
------
**str**. *zfill(width)*

*width*
    Required. Width of the padding field.

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Remarks
-------
A sign prefix is handled correctly. The original string is returned if *width* is less than or equal to **len(str)**.

Example
-------
>>> '350'.zfill(1)
'350'
>>> '350'.zfill(2)
'350'
>>> '350'.zfill(3)
'350'
>>> '350'.zfill(4)
'0350'
>>> '350'.zfill(10)
'0000000350'
>>> '350'.zfill(20)
'00000000000000000350'
>>> '-350'.zfill(5)
'-0350'

See Also
--------
#TODO

