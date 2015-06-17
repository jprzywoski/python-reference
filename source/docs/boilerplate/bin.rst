Shebang (Unix)
From Wikipedia, the free encyclopedia
	It has been suggested that this article be merged with Interpreter directive. (Discuss) Proposed since June 2014.
A "shebang" character sequence

In computing, a shebang (also called a sha-bang,[1][2][3] hashbang,[4][5] pound-bang,[2][6] or hash-pling[2][7]), is the character sequence consisting of the characters number sign and exclamation mark (that is, "#!") at the beginning of a script.

Under Unix-like operating systems, when a script with a shebang is run as a program, the program loader parses the rest of the script's initial line as an interpreter directive; the specified interpreter program is run instead, passing to it as an argument the path that was initially used when attempting to run the script.[8] For example, if a script is named with the path "path/to/script", and it starts with the following line:

    #!/bin/sh

then the program loader is instructed to run the program "/bin/sh" instead (usually this is the Bourne shell or a compatible shell), passing "path/to/script" as the first argument.

The shebang line is usually ignored by the interpreter because the "#" character is a comment marker in many scripting languages; some language interpreters that do not use the hash mark to begin comments (such as Scheme) still may ignore the shebang line in recognition of its purpose.[9]

Contents

    1 Syntax
    2 Examples
    3 Purpose
        3.1 Strengths
    4 Portability
        4.1 Magic number
        4.2 Security issues
    5 Etymology
    6 History
    7 Notes
    8 See also
    9 References
    10 External links

Syntax

The form of a shebang interpreter directive is as follows:[8]

    #! interpreter [optional-arg]

The interpreter must be an absolute path to an executable[1] program (if this interpreter program is a script, it must contain a shebang as well). The optional‑arg should either not be included or it should be a string that is meant to be a single argument (for reasons of portability, it should not contain any whitespace).
Examples

Some typical shebang lines:

    #!/bin/sh — Execute the file using sh, the Bourne shell, or a compatible shell
    #!/bin/csh -f — Execute the file using csh, the C shell, or a compatible shell, and suppress the execution of the user’s .cshrc file on startup
    #!/usr/bin/perl -T — Execute using Perl with the option for taint checks

Shebang lines may include specific options that are passed to the interpreter (see the Perl example above). However, implementations vary in the parsing behavior of options; for portability, only one option should be specified (if any) without any embedded whitespace. Further portability guidelines are found below.
Purpose

Interpreter directives allow scripts and data files to be used as system commands, hiding the details of their implementation from users and other programs, by removing the need to prefix scripts with their interpreter on the command line.

Consider a Bourne shell script that is identified by the path "some/path/to/foo" and that has the following as its initial line:

#!/bin/sh -x

If the user attempts to run this script with the following command line (specifying "bar" and "baz" as arguments):

some/path/to/foo bar baz

then the result would be similar to having actually executed the following command line instead:

/bin/sh -x some/path/to/foo bar baz

If "/bin/sh" specifies the Bourne shell, then the end result is that all of the shell commands in the file "some/path/to/foo" are executed with the positional variables $1 and $2 set to "bar" and "baz", respectively. Also, because the initial number sign is the character used to introduce comments in the Bourne shell language (and in the languages understood by many other interpreters), the entire shebang line is ignored by the interpreter.

However, it is up to the interpreter to ignore the shebang line; thus, a script consisting of the following two lines simply echos both lines to standard output when run:

#!/bin/cat
Hello world!

Strengt