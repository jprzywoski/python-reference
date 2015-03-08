========
encoding
========

Description
===========
Returns the encoding of the file.

Syntax
======
**file**. *encoding*

Return Value
============
**None**

Time Complexity
===============
#TODO

Remarks
=======
When Unicode strings are written to a file, they will be converted to byte strings using this *encoding*. In addition, when the file is connected to a terminal, the attribute gives the encoding that the terminal is likely to use (that information might be incorrect if the user has misconfigured the terminal). The attribute is read-only and may not be present on all file-like objects. It may also be **None**, in which case the file uses the system default encoding for converting **Unicode** strings.

Example
=======
>>> f = io.open(r'C:\aiw.txt', encoding='utf-8')
>>> f.encoding
'utf-8'

See Also
========
#TODO
