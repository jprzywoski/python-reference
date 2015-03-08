====
continue
====

Description
====
Skips the execution of the code below it and starts a new cycle of the loop.

Syntax
====
**loop:**
    *continue*
**else:**
    *suite*
    
loop
    for or while loop.

Remarks
====
The continue statement can only appear in a loop body. It causes the rest of the statement body in the loop to be skipped.

continue may only occur syntactically nested in a for or while loop, but not nested in a function or class definition or finally clause within that loop. It continues with the next cycle of the nearest enclosing loop.

When continue passes control out of a try statement with a finally clause, that finally clause is executed before really starting the next loop cycle.

A continue statement executed in the first *suite* skips the rest of the *suite* and continues with the next item, or with the else clause if there was no next item.

Example 1
====
>>> for i in range(5):
...     if i == 3:
...         continue
...     print i
...     
0
1
2
4

Example 2
====
>>> i = 0
>>> while i < 5:
...     try:
...         i += 1
...         if i == 3:
...             continue
...         print i
...     finally:
...         print i
...         
1
1
2
2
3
4
4
5
5

See Also
====
#TODO
