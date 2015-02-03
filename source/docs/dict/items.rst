=====
items
=====

Description
===========
Returns a copy of the dictionary's list of (key, value) pairs.

Syntax
======
**dict**. *items()*

Return Value
============
**list**

Time Complexity
===============
#TODO

Remarks
=======
CPython implementation detail: Keys and values are listed in an arbitrary order which is non-random, varies across Python implementations, and depends on the dictionary’s history of insertions and deletions.

If items(), keys(), values(), iteritems(), iterkeys(), and itervalues() are called with no intervening modifications to the dictionary, the lists will directly correspond. This allows the creation of (value, key) pairs using zip():

>>> pairs = zip(d.values(), d.keys())

The same relationship holds for the iterkeys() and itervalues() methods: pairs = zip(d.itervalues(), d.iterkeys()) provides the same value for pairs. Another way to create the same list is pairs = [(v, k) for (k, v) in d.iteritems()].

Example
=======
>>> d = {'a': 1, 'b': 2}
>>> d.items()
[('a', 1), ('b', 2)]

See Also
========
#TODO
