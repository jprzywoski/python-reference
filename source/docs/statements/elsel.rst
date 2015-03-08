====
else
====

Description
====
Executes specified block of code after loop terminating condition other then break was met.

Syntax
====
**loop:**
    **suite**
**else:**
    *suite*
        
*loop*
    for or while loop.
*else*
    Optional. Indicates block of code executed when loop terminates without calling break statement.
*suite*
    Block of code.

Remarks
====

Example 1
====
>>> for i in range(3):
...     print i
... else:
...     print "Loop terminating condition was reached"
...     
0
1
2
Loop terminating condition was reached

Example 2
====
>>> i = 0
>>> while i < 3:
...     print i
...     i = i + 1
... else:
...     print "Loop terminating condition was reached"
...     
0
1
2
Loop terminating condition was reached

Example 3
====
>>> # in this example else *suite* is not executed since breaks terminates the whole loop
>>> for i in range(3):
...     if i == 2:
...         break
...     print i
... else:
...     print "Loop terminating condition was reached"
...     
0
1

Example 4
====
>>> # in this example else simply means: no-break
>>> for i in range(3):
...     if i == 5:
...         break
...     print i
... else:
...     print "Loop terminating condition was reached"
...     
0
1
2
Loop terminating condition was reached

Example 5
====
>>> # else *suite* is executed after continue
>>> for i in range(3):
...     if i == 2:
...         continue
...     print i
... else:
...     print "Loop terminating condition was reached"
...     
0
1
Loop terminating condition was reached

See Also
====
#TODO
