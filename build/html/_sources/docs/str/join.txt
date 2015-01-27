====
join
====

Description
----------
Returns a string made from the elements of an iterable.

Syntax
------
**str**. *join(iterable)*

*iterable*
    Required. The *iterable* used for creating the string.

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Remarks
-------
The separator between elements is the string providing this method.

Example
-------
>>> ''.join(['A', 'B', 'C'])
'ABC'
>>> ''.join({'A': 0, 'B': 0, 'C': 0}) # note that dicts are unordered
'ACB'
>>> '-'.join(['A', 'B', 'C'])  # '-' string is the seprator
'A-B-C'

See Also
--------
#TODO
