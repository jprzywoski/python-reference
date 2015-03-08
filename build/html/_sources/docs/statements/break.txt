====
break
====

Description
====
Terminates the execution of a loop.

Syntax
====
**loop:**
    *break*
**else:**
    *suite*

*loop*
    for or while loop.

Remarks
====
break may only occur syntactically nested in a for or while loop, but not nested in a function or class definition within that loop.

It terminates the nearest enclosing loop, skipping the optional else clause if the loop has one.

If a for loop is terminated by break, the loop control target keeps its current value.

When break passes control out of a try statement with a finally clause, that finally clause is executed before really leaving the loop.

A break statement executed in the first *suite* terminates the loop without executing the else clause’s *suite*.

Example 1
====
>>> for i in range(5):
...     if i == 3:
...         break
...     print i
...     
0
1
2

Example 2
====
::

    i = 0
    while i < 10:
        try:
            if i == 5:
                break
            print i
            i += 1
        finally:
            print 'that line was executed, i = ', i
    *** Remote Interpreter Reinitialized  ***
    >>> 
    0
    that line was executed, i =  1
    1
    that line was executed, i =  2
    2
    that line was executed, i =  3
    3
    that line was executed, i =  4
    4
    that line was executed, i =  5
    that line was executed, i =  5

See Also
====
#TODO
