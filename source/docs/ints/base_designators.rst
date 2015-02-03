=======================
0... (Base Designators)
=======================

Description
===========
Returns a decimal integer converted from the specified base. 

Syntax
======

Base 2 (binary):

0b[0-1]

0B[0-1]

Base 8 (octal):

0o[0-7]

0O[0-7]

0[0-7]

Base 16 (hexadecimal, hex):

0x[0-9a-fA-F]

0X[0-9a-fA-F]

Remarks
-------
Lowercase and uppercase letters work exactly the same.

Example 1
=========
>>> 0b111
7
>>> 0B111
7

Example 2
=========
>>> 0o11
9
>>> 0O11
9
>>> 011
9

Example 3
=========
>>> 0xff
255
>>> 0Xff
255

See Also
========
#TODO
