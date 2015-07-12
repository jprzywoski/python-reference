=====
file
=====

File objects are implemented using C's <stdio.h> package and can be created with the built-in file() and open() functions. File objects are also returned by some other built-in functions and methods, such as os.popen() and os.fdopen() and the makefile() method of socket objects. Temporary files can be created using the tempfile module, and high-level file operations such as copying, moving, and deleting files and directories can be achieved with the shutil module.

When a file operation fails for an I/O-related reason, the exception IOError is raised. This includes situations where the operation is not defined for some reason, like seek() on a tty device or writing a file opened for reading.

Files are viewed as a sequential stream of bytes. A file is terminated with an end of file marker (EOF). When a file is opened a file object is associated with it.

By default, there are three files initialized when the script execution starts - sys.stdin, sys.stdout and sys.stderr. They correspond to the interpreter’s standard input, output and error streams.

Constructors
------------
`file`_
    Returns a file object.
`open`_
    Returns a file object.
    
Methods
-------

Reading
_______
`read`_
    Returns specified amount of bytes from the file.
`readline`_
    Reads one entire line from the file.
`readlines`_
    Returns a list containing lines from the file.
`xreadlines`_
    Returns an iterator over the lines of the file.
`next`_
    Returns a next line from the file.
    
Writing
_______
`write`_
    Writes a string to the file.
`writelines`_
    Writes a sequence of strings to the file.
`flush`_
    Flushes the write buffers of the file.

File Position
_____________    
`tell`_
    Returns the file’s current position.
`seek`_
    Sets the file’s current position.
    
Other
_____
`close`_
    Flushes and closes the file.
`fileno`_
    Returns the integer "file descriptor".
`truncate`_
    Truncates the file’s size.
`isatty`_
    Returns True if the file is if the stream is interactive (i.e., connected to a terminal/tty device).

Properties
----------
`name`_
    Returns the name of the file.
`mode`_
    Returns the I/O mode for the file.
`encoding`_
    Returns the encoding of the file.
`closed`_
    Returns a Boolean stating whether the file is closed.
`errors`_
    Returns the Unicode error handler used along with the encoding.
`newlines`_
    Return type of newlines encountered while reading the file.
`softspace`_
    Returns a Boolean that indicates whether a space character needs to be printed before another value when using the print statement.
    
.. _Overview: overview.html
.. _flush: flush.html
.. _close: close.html
.. _fileno: fileno.html
.. _next: next.html
.. _isatty: isatty.html
.. _xreadlines: xreadlines.html
.. _read: read.html
.. _readline: readline.html
.. _readlines: readlines.html
.. _seek: seek.html
.. _tell: tell.html
.. _truncate: truncate.html
.. _write: write.html
.. _writelines: writelines.html
.. _closed: closed.html
.. _encoding: encoding.html
.. _errors: errors.html
.. _mode: mode.html
.. _name: name.html
.. _newlines: newlines.html
.. _softspace: softspace.html
.. _file: ../functions/file.html
.. _open: ../functions/open.html