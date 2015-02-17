====
; Statement Separator
====

Description
====
Separates two statements.

Syntax
====
statement; another statement
    
Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
====
Avoid having multiple statements on a single line.

Though the language definition allows one to use a semi-colon to delineate statements, doing so without reason makes one's code harder to read. Typically violated with the previous rule.

Harmful

>>> if this_is_bad_code: rewrite_code(); make_it_more_readable();

Idiomatic

>>> if this_is_bad_code: 
... rewrite_code()
... make_it_more_readable()

See Also
========
#TODO