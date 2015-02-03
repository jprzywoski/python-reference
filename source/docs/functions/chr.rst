===
chr
===

Description
===========
Returns a string of one character whose ASCII code is the specified number.

Syntax
======
**chr** *(number)*

*number*
	Required. Any integer within the 0-255 range.

Return Value
============
**str**

Time Complexity
============
#TODO

Example
=======
>>> chr(65)
'A'
>>> chr(97)
'a'
>>> ''.join([chr(c) for c in range(65, 91)])
'ABCDEFGHIJKLMNOPQRSTUVWXYZ'

See Also
========
#TODO