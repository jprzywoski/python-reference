==========
splitlines
==========

Description
----------
Returns a list of the lines in the string, breaking at line boundaries.

Syntax
------
**str**. *splitlines([keepends])*

*keepends*
    Optional. When set to **True** line breaks are included in the resulting list.

Return Value
------------
**list**

Time Complexity
---------------
#TODO

Remarks
-------
This method uses the universal newlines approach to splitting lines.

Unlike `split()`_ when a delimiter string *sep* is given, this method returns an empty list for the empty string, and a terminal line break does not result in an extra line.

Example
-------
>>> "AB\nCD\n".splitlines()
['AB', 'CD']
>>> "AB\nCD\n".splitlines(True)
['AB\n', 'CD\n']
>>> "\n\n".splitlines()
['', '']
>>> "".splitlines()
[]

See Also
--------
`split()`_, `rsplit()`_, `partition()`_, `rpartition()`_

.. _split(): ../str/split.html
.. _rsplit(): ../str/rsplit.html
.. _partition(): ../str/partition.html
.. _rpartition(): ../str/rpartition.html
