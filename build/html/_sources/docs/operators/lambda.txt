====
lambda
====

Description
===========
Returns an anonymous function.

Syntax
======
lambda variable, ...: expression

variable, ...
    Optional. One or more variables used in the right part of the expression.
expression
    Required. Return value of the function. 
    
Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
lambda expression is a shorthand way of defining a function that is not bound to a specified name during its creation.

Consider the following function:

>>> def func(a): return a + 1
... 
>>> func(0)
1
>>> 

The same function can be defined using lambda expression as follows:

>>> func = lambda a: a + 1
>>> func(0)
1

Both functions are the same. Note that `lambda` does not include a return statement. The right expression is the implicit return value. Lambda functions need not to be assigned to any variables.
    
Example 1
=======
>>> # this example shows how to use lambda with sorted function
>>> # lambda function is grabage collected after it has been used 
>>> # (there is no reference to it to keep it alive)
>>> sorted(['A', 'b', 'C'], key=lambda x: x.lower())
['A', 'b', 'C']

Example 2
====
>>> # this is a code snippet from a Tkinter gui app
>>> # in this case lambda is quite convenient
>>> self.btn_cancel = Button(self.progress_container, text='Cancel',
>>>     command=lambda: subprocess.call('taskkill /f /im uberzip.exe',
>>>     shell=True))

See also
========
#TODO
