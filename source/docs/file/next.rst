====
next
====

Description
===========
Returns a next line from the file.

Syntax
======
**file**. *next()*

Remarks
=======
A file object is its own iterator, for example iter(f) returns f (unless f is closed). When a file is used as an iterator, typically in a for loop (for example:

>>> for line in f:
...    print line.strip()

), the next() method is called repeatedly. This method returns the next input line, or raises *StopIteration* when *EOF* is hit when the file is open for reading (behavior is undefined when the file is open for writing).

In order to make a for loop the most efficient way of looping over the lines of a file (a very common operation), the *next()* method uses a hidden read-ahead buffer. As a consequence of using a read-ahead buffer, combining *next()* with other file methods (like *readline()*) does not work right. However, using *seek()* to reposition the file to an absolute position will flush the read-ahead buffer.

Return Value
============
**str**

Time Complexity
===============
#TODO

Example
=======
>>> f = open(r'C:\aiw.txt')
>>> f.next()
"                ALICE'S ADVENTURES IN WONDERLAND\n"
>>> f.next()
'\n'
>>> f.next()
'                          Lewis Carroll\n'

See Also
========
#TODO
