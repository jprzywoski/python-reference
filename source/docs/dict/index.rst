====
dict
====

Dictionaries are mutable unordered collections (they do not record element position or order of insertion) of key-value pairs. Keys within the dictionary must be unique and must be hashable. That includes types like numbers, strings and tuples. Lists and dicts can not be used as keys since they are mutable. Dictionaries in other languages are also called hash tables or associative arrays.

Numeric types used for keys obey the normal rules for numeric comparison: if two numbers compare equal (such as 1 and 1.0) then they can be used interchangeably to index the same dictionary entry. (Note however, that since computers store floating-point numbers as approximations it is usually unwise to use them as dictionary keys.)

Constructors
====
`dict()`_
    Returns a dictionary object.
`{} dict comprehension`_
    Returns a dictionary based on existing iterables.
`literal syntax`_
    Initializes a new instance of the **dict** type.
    
Methods
====
Contents Access
----
`get`_
    Returns the value for key in the dictionary; if not found returns a default value.
`items`_
    Returns a copy of the dictionary's list of (key, value) pairs.
`keys`_
    Returns a copy of the dictionary's list of keys.
`values`_
    Returns a copy of the dictionary's list of values.
    
Adding Elements
----
`update`_
    Adds key:value pairs to the dictionary.

Deleting
----
`clear`_
    Removes all items from the dictionary.
`pop`_
    Removes the key in the dictionary and returns its value.
`popitem`_
    Removes and returns an arbitrary key:value pair from the dictionary.

Information
----
`has_key`_
    Returns a Boolean stating whether the specified key is in the dictionary.

Other
----
`copy`_
    Returns a shallow copy of the dictionary.
`fromkeys`_
    Returns a new dictionary with keys from a supplied iterable and values all set to specified value.

Iterators
----
`iteritems`_
    Returns an iterator over the dictionary’s key:value pairs.
`itervalues`_
    Returns an iterator over the dictionary’s values.
`iterkeys`_
    Returns an iterator over the dictionary’s keys.

Dictionary Views
----
`viewitems`_
    Returns a new view of the dictionary’s items (key:value pairs).
`viewvalues`_
    Returns a new view of the dictionary’s values.
`viewkeys`_
    Returns a new view of the dictionary’s keys.
    
Dictionary Views Operators
----
`& (intersection)`_
    Returns only the elements that appear both in the dictview and the specified iterable.
`^ (symmetric difference)`_
    Returns the elements that appear in either the dictview or the specified iterable, but not in both.
`- (difference)`_
    Returns the elements that appear in the dictview and not in the specified iterable.
`| (union)`_
    Returns all the elements that appear in the dictview and the specified iterable.

Functions
====
`len`_
    Returns an int type specifying number of elements in the collection.
`min`_
    Returns the smallest item from a collection.
`max`_
    Returns the largest item in an iterable or the largest of two or more arguments.
`sum`_
    Returns a total of the items contained in the iterable object.
`sorted`_
    Returns a sorted list from the iterable.
`reversed`_
    Returns a reverse iterator over a sequence.
`all`_
    Returns a Boolean value that indicates whether the collection contains only values that evaluate to True.
`any`_
    Returns a Boolean value that indicates whether the collection contains any values that evaluate to True.
`enumerate`_
    Returns an enumerate object.
`zip`_
    Returns a list of tuples, where the i-th tuple contains the i-th element from each of the argument sequences or iterables.

Misc
====
`[] (key lookup)`_
    Returns the value associated with the given key.
    
.. _dict(): ../functions/dict.html
.. _[] (key lookup): ../brackets/key_lookup.html
.. _{} dict comprehension: ../comprehensions/dict_comprehension.html
.. _literal syntax: literals.html
.. _update: update.html
.. _clear: clear.html
.. _pop: pop.html
.. _popitem: popitem.html
.. _has_key: has_key.html
.. _items: items.html
.. _keys: keys.html
.. _values: values.html
.. _get: get.html
.. _copy: copy.html
.. _fromkeys: fromkeys.html
.. _itervalues: itervalues.html
.. _iterkeys: iterkeys.html
.. _iteritems: iteritems.html
.. _viewitems: viewitems.html
.. _viewvalues: viewvalues.html
.. _viewkeys: viewkeys.html
.. _& (intersection): intersection.html
.. _^ (symmetric difference): symmetric_difference.html
.. _- (difference): difference.html
.. _| (union): union.html

.. _enumerate: ../functions/enumerate.html
.. _len: ../functions/len.html
.. _reversed: ../functions/reversed.html
.. _sorted: ../functions/sorted.html
.. _sum: ../functions/sum.html
.. _zip: ../functions/zip.html
.. _cmp: ../functions/cmp.html
.. _max: ../functions/max.html
.. _min: ../functions/min.html
.. _all: ../functions/all.html
.. _any: ../functions/any.html
