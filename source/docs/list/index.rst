====
list
====
Lists are mutable ordered and indexed collections of objects. The items of a list are arbitrary Python objects. Lists are formed by placing a comma-separated list of expressions in square brackets. (Note that there are no special cases needed to form lists of length 0 or 1.)
    
Constructors
====
`list()`_
    Converts an object into a list.    
`[] list comprehensions`_
    Returns a list based on existing iterables.
`literal syntax`_
    Initializes a new instance of the **list** type.

Methods
====

Adding Elements
----
`insert`_
    Inserts an item at a given position.
`append`_
    Adds an item to the end of the list.
`extend`_
    Extends the list by appending all the items from the iterable.

Deleting
----
`remove`_
    Removes the first item from the list which matches the specified value.
`pop`_
    Removes and returns the item at the specified index.
    
Information
----
`index`_
    Returns the index of the first occurrence of the specified list item.
`count`_
    Returns the number of times the specified item appears in the list.
    
Modifying
----
`sort`_
    Sorts the list in place.
`reverse`_
    Reverses the elements of the list, in place.

Functions
====
`len`_
    Returns an int type specifying number of elements in the collection.
`min`_
    Returns the smallest item from a collection.
`max`_
    Returns the largest item in an iterable or the largest of two or more arguments.
`cmp`_
    Compares two objects and returns an integer according to the outcome.
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

Operators
====
`[] (index operator)`_
    Gives access to a sequence's element.
`[::] (slicing)`_
    Gives access to a specified range of sequence's elements.
`+ (concatenation)`_
    Returns a concatenation of two sequences.
`* (multiple concatenation)`_
    Returns a sequence self-concatenated specified amount of times.
    
    
.. _[] (index operator): ../brackets/indexing.html
.. _[::] (slicing): ../brackets/slicing.html
.. _list(): ../functions/list.html
.. _literal syntax: literals.html
.. _[] list comprehensions: ../comprehensions/list_comprehension.html
.. _append: append.html
.. _insert: insert.html
.. _extend: extend.html
.. _pop: pop.html
.. _remove: remove.html
.. _index: lindex.html
.. _count: count.html
.. _reverse: reverse.html
.. _sort: sort.html
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
.. _+ (concatenation): ../operators/concatenation.html
.. _* (multiple concatenation): ../operators/multiple_concatenation.html
