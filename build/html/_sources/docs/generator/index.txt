====
generator
====
Generator iterators are created by the `yield` keyword. The real difference between them and ordinary functions is that `yield` unlike return is both exit and entry point for the function's body. That means, after each `yield` call not only the generator returns something but also remembers its state. Calling the next() method brings control back to the generator starting after the last executed `yield` statement. Each `yield` statement is executed only once, in the order it appears in the code. After all the yield statements have been executed iteration ends.

Since generators support iterator protocol, they can be used in `for` loops.

Constructors
====
`yield`_
    
`() generator expression`_
    Returns an iterator over elements created by using list comprehension. 

Methods
=======
`next`_
    Starts the execution of a generator function or resumes it at the last executed yield expression.
`send`_
    Resumes the execution and “sends” a value into the generator function.
`throw`_
    Raises a specified exception at the point where generator was paused, and returns the next value yielded by the generator function.
`close`_
    Raises a GeneratorExit at the point where the generator function was paused.
    
.. _next: next.html
.. _send: send.html
.. _throw: throw.html
.. _close: close.html
.. _() generator expression: ../comprehensions/gen_expression.html

