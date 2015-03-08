====================
{} set comprehension
====================

Description
===========
Returns a set based on existing iterables.

Syntax
======
**{expression(variable) for variable in input_set [predicate][, …]}**

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
**set**

Time Complexity
===============
#TODO

Example 1
=========
>>> {s for s in [1, 2, 1, 0]}
set([0, 1, 2])
>>> {s**2 for s in [1, 2, 1, 0]}
set([0, 1, 4])
>>> {s**2 for s in range(10)}
set([0, 1, 4, 9, 16, 25, 36, 49, 64, 81])

Example 2
=========
>>> {s for s in [1, 2, 3] if s % 2}
set([1, 3])

Example 3
=========
>>> {(m, n) for n in range(2) for m in range(3, 5)}
set([(3, 0), (3, 1), (4, 0), (4, 1)])
  
See Also
========
#TODO