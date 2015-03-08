=====
close
=====

Description
===========
Flushes and closes the file.

Syntax
======
**file**. *close()*

Remarks
=======
A closed file cannot be read or written any more. Any operation which requires that the file be open will raise a *ValueError* after the file has been closed. Calling *close()* more than once is allowed.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example 1
=========
>>> f = open(r'C:\aiw.txt')
>>> f.readline()
"                ALICE'S ADVENTURES IN WONDERLAND\n"
>>> f.close()
>>> f.readline()
ValueError: I/O operation on closed file

You can avoid having to call this method explicitly if you use the with statement. For example, the following code will automatically close f when the with block is exited:

Example 2
=========
::

    with open(r'C:\aiw.txt') as f:
        for line in f:
            print line,
        
In older versions of Python, you would have needed to do this to get the same effect:

Example 3
=========
::

    f = open("hello.txt")
    try:
        for line in f:
            print line,
    finally:
        f.close()

Note
====
Not all “file-like” types in Python support use as a context manager for the with statement. If your code is intended to work with any file-like object, you can use the function *contextlib.closing()* instead of using the object directly.

See Also
========
#TODO
