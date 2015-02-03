====
hash
====

Description
===========
Return the hash value of the object (if it has one).

Syntax
======
**hash** *(object)*

*object*
	Required. The object which hash value is to be returned. Only immutable types can be hashed.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The hash values are calculated by hashing algorithm.
Hash values are integers. They are used to quickly compare dictionary keys during a dictionary lookup. Numeric values that compare equal have the same hash value (even if they are of different types, as is the case for 1 and 1.0).
The hash value -1 is reserved (it’s used to flag errors in the C implementation).
For ordinary integers, the hash value is simply the integer itself (unless it’s -1).

Hashable types:
* bool
* int
* long
* float
* string
* unicode
* tuple
* code object

Non-hashable types:
* bytearray
* list
* set
* dictionary
* memoryview

Example
=======
>>> hash(1)
1
>>> hash(1.0)
1
>>> hash(1 + 2j)
2000007
>>> hash('foo')
-740391237
>>> hash((1, 2))
1299869600
>>> hash([1, 2])
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
TypeError: unhashable type: 'list'
>>> hash({'a': 1, 'b': 2})
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
TypeError: unhashable type: 'dict'
>>> hash({1, 2})
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
TypeError: unhashable type: 'set'

See Also
========
#TODO
