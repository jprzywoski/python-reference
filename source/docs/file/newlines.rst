========
newlines
========

Description
===========
Return type of newlines encountered while reading the file.

Syntax
======
**file**. *newlines*

Remarks
=======
If Python was built with universal newlines enabled (the default) this read-only attribute exists, and for files opened in universal newline read mode it keeps track of the types of newlines encountered while reading the file. The values it can take are *'\r', '\n', '\r\n',* **None** (unknown, no newlines read yet) or a **tuple** containing all the newline types seen, to indicate that multiple newline conventions were encountered. For files not opened in universal newlines read mode the value of this attribute will be **None**. 

Return Value
============
**None**

Time Complexity
===============
#TODO

See Also
========
#TODO
