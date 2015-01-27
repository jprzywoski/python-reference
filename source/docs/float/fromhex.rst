=======
fromhex
=======

Description
-----------
Returns the float represented by a hexadecimal string s.

Syntax
------
**float**. *fromhex(s)*

*s*
    Required. Must be a string; may have leading and trailing whitespace.

Return Value
------------
**str** or **float** depending on arguments

Remarks
-------
Note that float.hex() is an instance method, while float.fromhex() is a class method.

A hexadecimal string takes the form:

[sign] ['0x'] integer ['.' fraction] ['p' exponent]

where the optional sign may by either + or -, integer and fraction are strings of hexadecimal digits, and exponent is a decimal integer with an optional leading sign. Case is not significant, and there must be at least one hexadecimal digit in either the integer or the fraction. This syntax is similar to the syntax specified in section 6.4.4.2 of the C99 standard, and also to the syntax used in Java 1.5 onwards. In particular, the output of float.hex() is usable as a hexadecimal floating-point literal in C or Java code, and hexadecimal strings produced by C’s %a format character or Java’s Double.toHexString are accepted by float.fromhex().
Note that the exponent is written in decimal rather than hexadecimal, and that it gives the power of 2 by which to multiply the coefficient. For example, the hexadecimal string 0x3.a7p10 represents the floating-point number (3 + 10./16 + 7./16**2) * 2.0**10, or 3740.0:

Example 1
---------
>>> float.fromhex('0x3.a7p10')
3740.0

Applying the reverse conversion to 3740.0 gives a different hexadecimal string representing the same number:

Example 2
---------
>>> float.hex(3740.0)
'0x1.d380000000000p+11'
