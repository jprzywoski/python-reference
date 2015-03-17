=======================
() generator expression
=======================

Description
===========
Returns an iterator over elements created by using list comprehension.

Syntax
======
**(expression(variable) for variable in input_set [predicate][, …])**

*expression*
	Optional. An output expression producing members of the new set from members of the input set that satisfy the predicate expression.
*variable*
	Required. Variable representing members of an input set.
*input_set*
	Required. Represents the input set.
*predicate*
	Optional. Expression acting as a filter on members of the input set.
*[, …]]*
	Optional. Another nested comprehension.

Return Value
============
**generator**

Time Complexity
===============
#TODO

Example 1
=========
>>> (n for n in [0, 1])
<generator object <genexpr> at 0x00ED7698>
>>> i = (n for n in [0, 1])
>>> i.next()
0
>>> i.next()
1
>>> i.next()
StopIteration

Example 2
=========
>>> i = (n*2 for n in [0, 1, 2, 3])
>>> i
<generator object <genexpr> at 0x00ED7C10>
>>> i.next()
\0
>>> i.next()
2
>>> i.next()
4
>>> i.next()
6
>>> i.next()
StopIteration

Example 3
=========
>>> i = (n*2 for n in [0, 1, 2, 3] if n % 2)
>>> i.next()
2
>>> i.next()
6
>>> i.next()

Example 4
=========
>>> i = ((n, n**2) for n in range(5))
>>> for j in i: print j
... 
(0, 0)
(1, 1)
(2, 4)
(3, 9)
(4, 16)

Example 5
=========
>>> i = ((n, m) for n in range(2) for m in range(100, 102))
>>> for j in i: print j
... 
(0, 100)
(0, 101)
(1, 100)
(1, 101)
       
See Also
========
#TODO
