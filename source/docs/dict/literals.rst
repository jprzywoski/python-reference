==============
Literal Syntax
==============

Dictionaries can be initialized by enclosing comma separated colon delimited key: value pairs in squiggly brackets {}. Keys within the dict must be unique. Dictionaries do not maintain the items order.

Example 1
=========
>>> d = {'A': 1, 'B': 2}
>>> d
{'A': 1, 'B': 2}

Any duplicated keys are discarded during dict creation.

Example 2
=========
>>> d = {'A': 1, 'B': 2, 'A': 3}
>>> d
{'A': 3, 'B': 2}

