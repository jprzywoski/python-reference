====
bytearray
====

The bytearray type is a mutable sequence of integers in the range between 0 and 255. It allows you to work directly with binary data. It can be used to work with low-level data such as that inside of images or arriving directly from the network. 

Bytearray type inherits methods from both list and str types. This type can be used in lieu of a mutable string if needed.

>>> +-----+-----+-----+-----+
>>> |0-255|0-255|0-255|0-255|
>>> +-----+-----+-----+-----+

An example of a bytearray length 4.


Constructors
====
`bytearray()`_
    Returns a new bytearray object.

Methods
====
`fromhex`_
    Returns a new bytearray object initialized from a string of hex numbers.

`Methods Inherited From str`_
====

`Methods Inherited From list`_
====

.. _bytearray(): ../functions/bytearray.html
.. _fromhex: fromhex.html
.. _Methods Inherited From str: ../str/index.html
.. _Methods Inherited From list: ../list/index.html