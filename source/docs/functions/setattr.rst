=======
setattr
=======

Description
===========
Assigns a value to the object’s attribute given its name.

Syntax
======
**setattr** *(object, name, value)*

*object*
	Required. An object that allows its attributes to be changed.
*name*
	Required. A string name of the attribute.
*value*
	Required. A new value of any type.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Note that setattr(x, 'foobar', 123) is equivalent to x.foobar = 123.

Example 1
=========
>>> class Foo:
...     def __init__(self, x):
...         self.x = x
...
>>> f = Foo(10)
>>> f.x
10
>>> setattr(f, 'x', 20)
>>> f.x
20
>>> setattr(f, 'y', 10)
>>> f.y
10
>>> f.y = 100
>>> f.y
100

Example 2
=========
>>> # you can dynamically add a function as a method to a class
def b(self):
    print 'bar'

class Foo:
    pass

f = Foo()
print dir(f)             #['__doc__', '__module__']
setattr(Foo, 'bar', b)
print dir(f)             #['__doc__', '__module__', 'bar']
f.bar()                  #bar

See Also
========
#TODO