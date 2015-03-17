====
assert
====

Description
====
Raises AssertionError if the specified expression evaluates to False.

Syntax
====
assert expression, argument

expression
    Required. Expression to evaluate.
argument
    Optional. Argument passed to the exception raised.
    
Return Value
====
**exception**

Time Complexity
====
#TODO

Remarks
====
Assert statements are a convenient way to insert debugging assertions into a program.
The simple form, assert expression, is equivalent to

>>> if __debug__:
>>>    if not expression: raise AssertionError

The extended form, assert expression1, expression2, is equivalent to

>>> if __debug__:
>>>    if not expression1: raise AssertionError(expression2)

These equivalences assume that __debug__ and AssertionError refer to the built-in variables with those names. In the current implementation, the built-in variable __debug__ is True under normal circumstances, False when optimization is requested (command line option -O). The current code generator emits no code for an assert statement when optimization is requested at compile time. Note that it is unnecessary to include the source code for the expression that failed in the error message; it will be displayed as part of the stack trace.

Assignments to __debug__ are illegal. The value for the built-in variable is determined when the interpreter starts.

Example 1
====
>>> assert 2 + 2 == 4
>>> assert 2 + 2 == 3
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
AssertionError

Example 2
====
>>> assert 1 == False, "That can't be right."
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
AssertionError: That can't be right.

See Also
====
#TODO
