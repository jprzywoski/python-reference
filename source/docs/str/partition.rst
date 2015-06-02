=========
partition
=========

Description
----------
Returns a tuple containing the left part of the string split by the specified separator, the separator itself and the right part of the string.

Syntax
------
**str**. *partition(sep)*

*sep*
    Required. Separator for the returned tuple. If the separator is not found, partition returns a 3-tuple containing the string itself, followed by two empty strings.

Return Value
------------
**tuple**

Time Complexity
---------------
#TODO

Example
-------
>>> "AB-CD-EF".partition('-')
('AB', '-', 'CD-EF')
>>> "AB-CD-EF".partition(' ')
('AB-CD-EF', '', '')
>>> "AB-CD-EF".partition('D')
('AB-C', 'D', '-EF')

Example 2
---------
>>> "image.png".partition('.') # this example breaks image file-path into its components 
('image', '.', 'png')

See Also
--------
`rpartition()`_ for version that splits from right.

.. _rpartition(): ../str/rpartition.html
