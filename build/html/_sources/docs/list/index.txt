====
list
====

Lists are mutable ordered and indexed collections of objects. Often called arrays in other languages. The items of a list are arbitrary Python objects. Lists are formed by placing a comma-separated list of expressions in square brackets. (Note that there are no special cases needed to form lists of length 0 or 1.)
    
Constructors
============
`list()`_
    Converts an object into a list.    
`[] list comprehensions`_
    Returns a list based on existing iterables.
`literal syntax`_

Misc
====
`[] (index operator)`_
    Gives access to a sequence's element.
`[::] (slicing)`_
    Gives access to a specified range of sequence's elements.

Methods
=======

Adding Elements
_______________
`append`_
    Adds an item to the end of the list.
`insert`_
    Inserts an item at a given position.
`extend`_
    Extends the list by appending all the items from the iterable.

Deleting
________
`pop`_
    Removes and returns the item at the specified index.
`remove`_
    Removes the first item from the list which matches the specified value.

Information
___________
`index`_
    Returns the index of the first occurrence of the specified list item.
`count`_
    Returns the number of times the specified item appears in the list.

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

