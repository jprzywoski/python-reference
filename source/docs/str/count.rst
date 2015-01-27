=====
count
=====

Description
----------
Returns the number of non-overlapping occurrences of a substring in the searched string.

Syntax
------
**str**. *count(sub[, start[, end]])*

*sub*
    Required. The string searched for.
*start*
    Optional. Index from which to start counting. Default is 0 (start of the string).
*end*
    Optional. The end index for the search. End of the string is the default value.

Return Value
------------
**int**

Time Complexity
---------------
#TODO

Remarks
-------
Optional arguments *start* and *end* are interpreted as in slice notation.

Example
-------
>>> "ABCAB".count("A")
2
>>> "ABCAB".count("A", 1)
1
>>> "ABCAB".count("A", 1, 2)
0
>>> "ABCAB".count("D", 1, 2)
0

See Also
--------
#TODO
