====
set
====

Sets are mutable unordered collections of unique elements. Common uses include membership testing, removing duplicates from a sequence, and computing standard math operations on sets such as intersection, union, difference, and symmetric difference.

Sets do not record element position or order of insertion. Accordingly, sets do not support indexing, slicing, or other sequence-like behavior.

Sets are implemented using dictionaries. They cannot contain mutable elements such as lists or dictionaries. However, they can contain immutable collections.

Constructors
====
`set()`_
    Returns a set type initialized from iterable.   
`{} set comprehension`_
    Returns a set based on existing iterables.
`literal syntax`_
    Initializes a new instance of the **set** type.

Methods
====

Adding Elements
----
`add`_
    Adds a specified element to the set.
`update`_
    Adds specified elements to the set.

Deleting
----
`discard`_
    Removes an element from the set.
`remove`_
    Removes an element from the set (raises *KeyError* if not found).
`pop`_
    Removes and returns an arbitrary element from the set. 
`clear`_
    Removes all elements from the set.
    
Information
----
`issuperset`_
    Returns a Boolean stating whether the set contains the specified set or iterable.
`issubset`_
    Returns a Boolean stating whether the set is contained in the specified set or iterable.
`isdisjoint`_
    Returns a Boolean stating whether the set contents do not overlap with the specified set or iterable.
    
Set Operations
----
`difference`_
    Returns a new set with elements in the set that are not in the specified iterables.
`intersection`_
    Returns a new set with elements common to the set and the specified iterables.
`symmetric_difference`_
    Returns a new set with elements in either the set or the specified iterable but not both.
`union`_
    Returns a new set with elements from the set and the specified iterables.
    
Set Operations Assignment
----
`difference_update`_
    Updates the set, removing elements found in the specified iterables.
`intersection_update`_
    Updates the set, keeping only elements found in it and the specified iterables.
`symmetric_difference_update`_
    Updates the set, keeping only elements found in either set or the specified iterable, but not in both.
    
Copying
----
`copy`_
    Returns a copy of the set.
    
Set Operators
====

Adding Elements
----
`|= (update)`_
    Adds elements from another set.

Relational Operators
----
`== (is equal)`_
    Returns a Boolean stating whether the set has the same elements as the other set.
`!= (is not equal)`_
    Returns a Boolean stating whether the set has different elements as the other set.
`<= (issubset)`_
    Returns a Boolean stating whether the set is contained in the other set.
`< (issubset proper)`_
    Returns a Boolean stating whether the set is contained in the specified set and that the sets are not equal.
`>= (issuperset)`_
    Returns a Boolean stating whether the set contains the other set.
`> (issuperset proper)`_
    Returns a Boolean stating whether the set contains the other set and that the sets are not equal.

Set Operations
----
`- (difference)`_
    Returns a new set with elements in the set that are not in the other set.
`& (intersection)`_
    Returns a new set with elements common to the set and the other set.
`^ (symmetric_difference)`_
    Returns a new set with elements in either the set or the other set but not both.
`| (union)`_
    Returns a new set with elements from the set and the other set.
    
Set Operations Assignment
----
`-= (difference_update)`_
    Updates the set, removing elements found in the other set.
`&= (intersection_update)`_
    Updates the set, keeping only elements found in it and the other set.
`^= (symmetric_difference_update)`_
    Updates the set, keeping only elements found in either set or the other set, but not in both.

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
    
    
.. _set(): ../functions/set.html
.. _{} set comprehension: ../comprehensions/set_comprehension.html
.. _literal syntax: literals.html
.. _add: add.html
.. _update: update.html
.. _clear: clear.html
.. _discard: discard.html
.. _pop: pop.html
.. _remove: remove.html
.. _isdisjoint: isdisjoint.html
.. _issubset: issubset.html
.. _issuperset: issuperset.html
.. _difference: difference.html
.. _intersection: intersection.html
.. _symmetric_difference: symmetric_difference.html
.. _union: union.html
.. _difference_update: difference_update.html
.. _intersection_update: intersection_update.html
.. _symmetric_difference_update: symmetric_difference_update.html
.. _copy: copy.html
.. _|= (update): op_update.html
.. _<= (issubset): op_issubset.html
.. _< (issubset proper): op_issubset_proper.html
.. _>= (issuperset): op_issuperset.html
.. _> (issuperset proper): op_issuperset_proper.html
.. _- (difference): op_difference.html
.. _& (intersection): op_intersection.html
.. _| (union): op_union.html
.. _-= (difference_update): op_difference_update.html
.. _&= (intersection_update): op_intersection_update.html
.. _^ (symmetric_difference): op_symmetric_difference.html
.. _^= (symmetric_difference_update): op_symmetric_difference_update.html
.. _== (is equal): op_eq.html
.. _!= (is not equal): op_neq.html

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
