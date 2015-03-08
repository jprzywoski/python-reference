===========================
{} dictionary comprehension
===========================

Description
===========
Returns a dictionary based on existing iterables.

Syntax
======
**{expression(variable): expression(variable) for variable, variable in input_set [predicate][, …]}**

*expression*
	Optional. An output expression producing members of the new set from members of the input set that satisfy the predicate expression.
*variable*
	Required. Variables representing members of an input set.
*input_set*
	Required. Represents the input set.
*predicate*
	Optional. Expression acting as a filter on members of the input set.
*[, …]]*
	Optional. Another nested comprehension.

Return Value
============
**dict**

Time Complexity
===============
#TODO

Example 1
=========
>>> {k: v for k, v in [(1, 2), (3, 4)]}
{1: 2, 3: 4}
>>> {n: n for n in range(2)}
{0: 0, 1: 1}
>>> {chr(n): n for n in (65, 66, 66)}
{'A': 65, 'B': 66}
>>> {k: v for k, v in (('I', 1), ('II', 2))}
{'I': 1, 'II': 2}

Example 2
=========
>>> {k: v for k, v in (('a', 0), ('b', 1)) if v == 1}
{'b': 1}
       
See Also
========
#TODO
