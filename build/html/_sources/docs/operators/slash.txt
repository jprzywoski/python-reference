====
\ Line Continuation
====

Description
====
Breaks the line of code allowing for the next line continuation.

Syntax
====
line \\
    
Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
====
A line ending in a backslash cannot carry a comment. A backslash does not continue a comment. A backslash does not continue a token except for string literals (i.e., tokens other than string literals cannot be split across physical lines using a backslash). A backslash is illegal elsewhere on a line outside a string literal.

Example
====
>>> if 1900 < year < 2100 and 1 <= month <= 12 \
... and 1 <= day <= 31 and 0 <= hour < 24 \
... and 0 <= minute < 60 and 0 <= second < 60:   # Looks like a valid date
...     return 1

See Also
========
#TODO