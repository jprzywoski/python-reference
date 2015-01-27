================
as_integer_ratio
================

Description
-----------
Returns a pair of integers whose ratio is exactly equal to the original float and with a positive denominator.

Syntax
------
**float**. *as_integer_ratio()*

Return Value
------------
**tuple**

Remarks
-------
Raises OverflowError on infinities and a ValueError on NaNs.

Example
-------
>>> 3.14.as_integer_ratio()
(7070651414971679L, 2251799813685248L)
>>> 1.5.as_integer_ratio()
(3, 2) 