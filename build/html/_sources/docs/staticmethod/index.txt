=======
staticmethod
=======
staticmethod is basically a function defined inside a class. The difference is, we don't have to pass the instance of the class to the method as its first argument (`self` by convention). Since staticmethods don't receive the object itself as an argument we can't access its attributes inside the staticmethod body.

Also, while using staticmethod there is only one instance of the decorated method bound to the class rather then to respective objects instantiated from it.

Constructors
====
`staticmethod`_
    Returns a static method for function.
    
.. _staticmethod: ../functions/staticmethod.html
