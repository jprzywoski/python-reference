==========
rpartition
==========

Description
----------
Returns a tuple containing the left part of the string split by the specified separator, the separator itself and the right part of the string (starting from right).

Syntax
------
**str**. *rpartition(sep)*

*sep*
    Required. Separator for the returned tuple. If the separator is not found, partition returns a 3-tuple containing two empty strings, followed by the string itself.

Return Value
------------
**tuple**

Time Complexity
---------------
#TODO

Example 1
--------
>>> "AB-CD-EF".rpartition('-')
('AB-CD', '-', 'EF')
>>> "AB-CD-EF".rpartition(' ')
('', '', 'AB-CD-EF')
>>> "AB-CD-EF".rpartition('D')
('AB-C', 'D', '-EF')

Example 2
---------
>>> "image.png".rpartition('.') # this example breaks image file-path into its components 
('image', '.', 'png')

See Also
--------
`partition()`_

.. _partition(): ../str/partition.html
