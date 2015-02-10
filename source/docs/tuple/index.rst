=====
tuple
=====

Tuples are immutable ordered and indexed collections of objects. Tuples of two or more items are formed by comma-separated lists of expressions. A tuple of one item (a ‘singleton’) can be formed by affixing a comma to an expression (an expression by itself does not create a tuple, since parentheses must be usable for grouping of expressions). An empty tuple can be formed by an empty pair of parentheses.

Constructors
============
`tuple`_
    Returns a tuple built from iterable.
`literal syntax`_

Misc
====
`[] (index operator)`_
    Gives access to a sequence's element.
`[::] (slicing)`_
    Gives access to a specified range of sequence's elements.
    
Methods
=======

Information
-----------
`index`_
    Returns the index of the first occurrence of the specified tuple item.
`count`_
    Returns the number of times the specified item appears in the tuple.

.. _[] (index operator): ../brackets/indexing.html
.. _[::] (slicing): ../brackets/slicing.html
.. _index: lindex.html
.. _count: count.html
.. _literal syntax: literals.html

