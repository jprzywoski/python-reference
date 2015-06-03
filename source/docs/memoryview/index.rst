====
memoryview
====


Constructors
====
`memoryview()`_
    Returns a new memoryview object.

Methods
====
`tobytes`_
    Returns the data in the buffer as a string.
`tolist`_
    Returns the data in the buffer as a list of integers.
    
Properties
====
`format`_
    Returns a string containing the format (in struct module style) for each element in the view. 
`itemsize`_
    Returns the size in bytes of each element of the memoryview. 
`ndim`_
    Returns an integer indicating how many dimensions of a multi-dimensional array the memory represents.
`readonly`_
    Returns a Boolean indicating whether the memory is read only. 
`shape`_
    Returns a tuple of integers the length of ndim giving the shape of the memory as a N-dimensional array.
`strides`_
    Returns a tuple of integers the length of ndim giving the size in bytes to access each element for each dimension of the array. 

.. _memoryview(): ../functions/memoryview.html
.. _tobytes: tobytes.html
.. _tolist: tolist.html
.. _format: format.html
.. _itemsize: itemsize.html
.. _ndim: ndim.html
.. _readonly: readonly.html
.. _shape: shape.html
.. _strides: strides.html

