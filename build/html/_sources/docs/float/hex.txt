===
hex
===

Description
-----------
Returns a representation of a floating-point number as a hexadecimal string.

Syntax
------
**float**. *hex()*

Return Value
------------
**str**

Discussion
----------
For finite floating-point numbers, this representation will always include a leading 0x and a trailing p and exponent.
Since Python’s floats are stored internally as binary numbers, converting a float to or from a decimal string usually involves a small rounding error. In contrast, hexadecimal strings allow exact representation and specification of floating-point numbers. This can be useful when debugging, and in numerical work.

Example
-------
>>> 1.5.hex()
'0x1.8000000000000p+0'
>>> 1.0.hex()
'0x1.0000000000000p+0'
>>> 16.0.hex()
'0x1.0000000000000p+4' 