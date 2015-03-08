=====
flush
=====

Description
===========
Flushes the write buffers of the file.

Syntax
======
**file**. *flush()*

Note
====
It works like stdio‘s *fflush()*. This may be a no-op on some file-like objects. *flush()* does not necessarily write the file’s data to disk. Use *flush()* followed by *os.fsync()* to ensure this behavior. 

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> fw = open(r'C:\test.txt', "w")
>>> fw.write('foobar')
>>> fr = open(r'C:\test.txt')
>>> fr.readlines() # even though we just wrote a line to the fr file it appears empty until close() method is called
[]
>>> fw.flush() # flushing forces the buffer content into the file without closing it
>>> fr.readlines()
['foobar']

See Also
========
#TODO
