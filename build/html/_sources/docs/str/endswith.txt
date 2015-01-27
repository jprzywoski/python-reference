========
endswith
========

Description
----------
Returns a Boolean stating whether a string ends with the specified suffix.

Syntax
------
**str**. *startswith(suffix[, start[, end]])*

*suffix*
    Required. The substring looked for. *suffix* can also be a tuple of suffixes to look for.
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
>>> "image.png".endswith("png")
True
>>> "image.png".endswith(("png", "jpg"))
True
>>> "123_log_ABC".endswith("log", 4, 7)
True

See Also
--------
#TODO
