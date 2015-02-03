=======
has_key
=======

Description
===========
Returns a Boolean stating whether the specified key is in the dictionary.

Syntax
======
**dict**. *has_key(key)*

*key*
    Required. The key you are looking for.

Return Value
============
**bool*

Time Complexity
===============
#TODO

Note
====
has_key() is deprecated in favor of *key* **in** *d*.

Example
=======
>>> d = {'a': 1, 'b': 2}
>>> d.has_key('a')
True
>>> d.has_key('x')
False
>>> 'a' in d              # <= this is recommended instead
True

See Also
========
#TODO
