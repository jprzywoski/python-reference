====
for
====

Description
====
Loops over elements of an iterable object.

Syntax
====
**for item in iterable:**
    *suite*
**else:**
    *suite*
    
*item*
    Item retrieved from the iterable. This variable is bound to the current element of the iterable.
*iterable*
    Any iterable object.
*else*
    Optional. Indicates block of code executed when loop terminates without calling break statement.
*suite*
    Block of code to be executed.

Remarks
====
After each iteration, next item is retrieved from the iterable container. The loop's *suite* is executed repeatedly until the container is empty. 

Python has only one `for` loop, which is functionally the same as `for each` in some other languages. To loop specified number of times range() or xrange() function is used.

Example 1
====
>>> for i in range(3):
...     print i
...     
0
1
2

Example 2
====
>>> # this example shows how files can be iterated over with a for loop
>>> for line in open("C:\\test\\test.txt"):
...     print line
... 
line 1
line 2
line 3

See Also
====
#TODO
