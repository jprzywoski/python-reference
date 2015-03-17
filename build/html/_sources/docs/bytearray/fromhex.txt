====
fromhex
====

Description
===========
Returns a new bytearray object initialized from a string of hex numbers.

Syntax
======
**bytearray**. *fromhex(string)*

*string*
    Required. String containing hex numbers.

Return Value
============
**bytearray**

Time Complexity
===============
#TODO

Remarks
====
Spaces between numbers can be used.

Example
=======
>>> bytearray.fromhex("A1 FF 92")
bytearray(b'\xa1\xff\x92')
>>> bytearray.fromhex("A1FF92")
bytearray(b'\xa1\xff\x92')

See Also
========

