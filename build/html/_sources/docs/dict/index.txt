====
dict
====

Dictionaries are mutable unordered collections (they do not record element position or order of insertion) of key-value pairs. Keys within the dictionary must be unique and must be hashable. That includes types like numbers, strings and tuples. Lists and dicts can not be used as keys since they are mutable. Dictionaries are also called hash tables or associative arrays.

Numeric types used for keys obey the normal rules for numeric comparison: if two numbers compare equal (such as 1 and 1.0) then they can be used interchangeably to index the same dictionary entry. (Note however, that since computers store floating-point numbers as approximations it is usually unwise to use them as dictionary keys.)

Constructors
------------
`dict()`_
    Returns a dictionary object.
`{} dict comprehension`_
    Returns a dictionary based on existing iterables.
`literal syntax`_

Misc
----
`[] (key lookup)`_
    Returns the value associated with the given key.
    
Methods
-------

Adding Elements
_______________
`update`_
    Adds key:value pairs to the dictionary.

Deleting
________
`clear`_
    Removes all items from the dictionary.
`pop`_
    Removes the key in the dictionary and returns its value.
`popitem`_
    Removes and returns an arbitrary key:value pair from the dictionary.

Information
___________
`has_key`_
    Returns a Boolean stating whether the specified key is in the dictionary.
`items`_
    Returns a copy of the dictionary's list of key:value pairs.
`keys`_
    Returns a copy of the dictionary's list of keys.
`values`_
    Returns a copy of the dictionary's list of values.
`get`_
    Returns the value for key in the dictionary; if not found returns a default value.

Other
_____
`copy`_
    Returns a shallow copy of the dictionary.
`fromkeys`_
    Returns a new dictionary with keys from a supplied iterable and values all set to specified value.

Iterators
_________
`iteritems`_
    Returns an iterator over the dictionary’s key:value pairs.
`itervalues`_
    Returns an iterator over the dictionary’s values.
`iterkeys`_
    Returns an iterator over the dictionary’s keys.

Dictionary Views
________________
`viewitems`_
    Returns a new view of the dictionary’s items (key:value pairs).
`viewvalues`_
    Returns a new view of the dictionary’s values.
`viewkeys`_
    Returns a new view of the dictionary’s keys.
    
Dictionary Views Operators
__________________________
`& (intersection)`_
    Returns only the elements that appear both in the dictview and the specified iterable.
`^ (symmetric difference)`_
    Returns the elements that appear in either the dictview or the specified iterable, but not in both.
`- (difference)`_
    Returns the elements that appear in the dictview and not in the specified iterable.
`| (union)`_
    Returns all the elements that appear in the dictview and the specified iterable.

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

