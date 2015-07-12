=====
tuple
=====
Tuples are immutable ordered and indexed collections of objects. Tuples of two or more items are formed by comma-separated lists of expressions. A tuple of one item (a ‘singleton’) can be formed by affixing a comma to an expression (an expression by itself does not create a tuple, since parentheses must be usable for grouping of expressions). An empty tuple can be formed by an empty pair of parentheses.

Constructors
====
`tuple`_
    Returns a tuple built from iterable.
`literal syntax`_
    Initializes a new instance of the **tuple** type.

Methods
====

Information
----
`index`_
    Returns the index of the first occurrence of the specified tuple item.
`count`_
    Returns the number of times the specified item appears in the tuple.

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
.. _index: lindex.html
.. _count: count.html
.. _literal syntax: literals.html
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
