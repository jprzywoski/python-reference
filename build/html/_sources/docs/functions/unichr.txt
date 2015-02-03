======
unichr
======

Description
===========
Returns a Unicode character specified by the code.

Syntax
======
**unichr** *(number)*

*number*
	Required. An integer specifying the Unicode code value of the character to be returned.

Return Value
============
**unicode**

Time Complexity
============
#TODO

Remarks
=======
This function is the inverse of ord() for Unicode strings. The valid range for the argument depends how Python was configured – it may be either UCS2 [0..0xFFFF] or UCS4 [0..0x10FFFF]. ValueError is raised otherwise. For ASCII and 8-bit strings see chr().

Example
=======
>>> unichr(97)
u'a'
>>> unichr(65)
u'A'

See Also
========
#TODO