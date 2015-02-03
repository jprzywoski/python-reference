===
ord
===

Description
===========
Returns an integer representing the code of the character.

Syntax
======
**ord** *(character)*

*character*
	Required. A character.

Return Value
============
**int**

Time Complexity
============
#TODO

Remarks
=======
This function is the inverse of chr() for 8-bit strings and of unichr() for unicode objects. If a unicode argument is given and Python was built with UCS2 Unicode, then the character’s code point must be in the range [0..65535] inclusive; otherwise the string length is two, and a TypeError will be raised.

Example 1
=========
>>> ord('a')
97
>>> ord('A')
65

Example 2
=========
>>> ord(u'a')
97
>>> ord(u'\u2020')
8224

See Also
========
#TODO