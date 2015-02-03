======
errors
======

Description
===========
Returns the Unicode error handler used along with the encoding.

Syntax
======
**file**. *errors*

Example
=======
>>> f = io.open(r'C:\aiw.txt', errors='ignore')
>>> f.errors
'ignore' 