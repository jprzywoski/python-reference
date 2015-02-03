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
This method returns the same thing as **iter(f)**.

Note
====
Deprecated since version 2.3:

Use `for line in file` instead.

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

