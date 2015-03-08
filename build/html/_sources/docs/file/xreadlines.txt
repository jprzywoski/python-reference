==========
xreadlines
==========

Description
===========
Returns an iterator over the lines of the file.

Syntax
======
**file**. *xreadlines()*

Remarks
=======
This method returns the same thing as **iter(file)**. Usage of this function is deprecated since Python 2.3. File objects are iterators by default now. 

Use `for line in file` instead.

Return Value
============
**file**

Time Complexity
===============
#TODO

Example
=======
>>> # test.txt contents:
>>> #ABC AB A
>>> #ABC AB
>>> #ABC
>>> f = open(r'C:\test.txt')
>>> fx = f.xreadlines()
>>> fx.next()
'ABC AB A\n'
>>> fx.next()
'ABC AB\n'
>>> fx.next()
'ABC\n'
>>> fx.next()
StopIteration

See Also
========
#TODO

