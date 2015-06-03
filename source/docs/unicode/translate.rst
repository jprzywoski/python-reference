=========
translate
=========

Description
----------
Returns a copy of the string with characters mapped through the given translation table or deleted.

Syntax
------
**str**. *translate(table[, deletechars])*

*table*
    Required. Must be a string of length 256.
*deletechars*
    Optional. Characters to be deleted from the string.

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Remarks
-------
You can use the **maketrans()** helper function in the **string** module to create a translation table.

For string objects, set the table argument to **None** for translations that only delete characters:

Example 1
---------
>>> # this example deletes all the vowels from the string
>>> "ABCDE".translate(None, "AEIOU")
'BCD'

Example 2
---------
>>> import string
>>> translation_table = string.maketrans('aeiou', '!@#$%')
>>> translation_table   # note the replaced vowels
'\x00\x01\x02\x03\x04\x05\x06\x07\x08\t\n\x0b\x0c\r\x0e\x0f\x10\x11\x12\x13\x14\x15\x16\x17\x18\x19\x1a\x1b\x1c\x1d\x1e\x1f !"#$%&\'()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\\]^_`!bcd@fgh#jklmn$pqrst%vwxyz{|}~\x7f\x80\x81\x82\x83\x84\x85\x86\x87\x88\x89\x8a\x8b\x8c\x8d\x8e\x8f\x90\x91\x92\x93\x94\x95\x96\x97\x98\x99\x9a\x9b\x9c\x9d\x9e\x9f\xa0\xa1\xa2\xa3\xa4\xa5\xa6\xa7\xa8\xa9\xaa\xab\xac\xad\xae\xaf\xb0\xb1\xb2\xb3\xb4\xb5\xb6\xb7\xb8\xb9\xba\xbb\xbc\xbd\xbe\xbf\xc0\xc1\xc2\xc3\xc4\xc5\xc6\xc7\xc8\xc9\xca\xcb\xcc\xcd\xce\xcf\xd0\xd1\xd2\xd3\xd4\xd5\xd6\xd7\xd8\xd9\xda\xdb\xdc\xdd\xde\xdf\xe0\xe1\xe2\xe3\xe4\xe5\xe6\xe7\xe8\xe9\xea\xeb\xec\xed\xee\xef\xf0\xf1\xf2\xf3\xf4\xf5\xf6\xf7\xf8\xf9\xfa\xfb\xfc\xfd\xfe\xff'
>>> translation_table = string.maketrans('AEIOU', '!@#$%')
>>> "ABCDE".translate(translation_table)
'!BCD@'
>>> "ABCDE".translate(translation_table, "B")
'!CD@'

See Also
--------
#TODO
