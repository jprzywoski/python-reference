==========
startswith
==========

Description
----------
Returns a Boolean stating whether a string starts with the specified prefix.

Syntax
------
**str**. *startswith(prefix[, start[, end]])*

*prefix*
    Required. The substring looked for. *prefix* can also be a tuple of prefixes to look for.
*start*
    Optional. Specifies beginning position for the search.
*end*
    Optional. Specifies ending position for the search.

Return Value
------------
**bool**

Time Complexity
---------------
#TODO

Example
-------
>>> "log_A1.csv".startswith("log")
True
>>> "log_A1.csv".startswith(("log", "out"))
True
>>> "in_A1.csv".startswith(("log", "out"))
False
>>> "013232_log_B.csv".startswith("log", 7)
True

See Also
--------
#TODO
