====
if
====

Description
====
Used for conditional execution.

Syntax
====
if expression:
    suite
elif expression:
    suite
else:
    suite
    
if
    Required. Branching starting point.
elif
    Optional. Another conditional expression.
else
    Optional. Indicates block of code executed when none of the conditions specified in if or elif constructs was True.
    
Return Value
====
**TODO**

Time Complexity
====
#TODO

Remarks
====
It selects exactly one of the suites by evaluating the expressions one by one until one is found to be true; then that suite is executed (and no other part of the if statement is executed or evaluated). If all expressions are false, the suite of the else clause, if present, is executed.

Example
====

See Also
====
#TODO

.. _XXX: XXX.html

