====
while
====

Description
====
Executes block of code repeatedly while the specified condition is True.

Syntax
====
**while condition:**
    *suite*
**else:**
    *suite*
    
*condition*
    Any expression that has a Boolean value.
*else*
    Optional. Indicates block of code executed when loop terminates without calling break statement.
*suite*
    Block of code to be executed.

Remarks
====
The while statement provides an iterative condition based loop. The *suite* is executed repeatedly as long as expression is True. The test on expression takes place before each execution of statement.

Example
====
>>> i = 0
>>> while i < 3:
...     print i
...     i = i + 1
...     
0
1
2

See Also
====
#TODO
