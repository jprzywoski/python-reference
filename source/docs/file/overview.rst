========
Overview
========

File objects are implemented using C’s stdio package and can be created with the built-in open() function. File objects are also returned by some other built-in functions and methods, such as os.popen() and os.fdopen() and the makefile() method of socket objects. Temporary files can be created using the tempfile module, and high-level file operations such as copying, moving, and deleting files and directories can be achieved with the shutil module.

When a file operation fails for an I/O-related reason, the exception IOError is raised. This includes situations where the operation is not defined for some reason, like seek() on a tty device or writing a file opened for reading.


