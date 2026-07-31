# `touch`

## Description

**`touch`**

`touch` is a shell command that sets the modification timestamp of an existing file to be current – which on a Unix-based file system includes special files such as directories. If the input path does not specify an existing file, then it creates a new, regular file at the path.

-- [Wikipedia](https://en.wikipedia.org/wiki/Touch_%28command%29)

The `touch` command updates the access and modification times of each file specified by the File parameter of each directory specified by the Directory parameter. If you do not specify a value for the Time variable, the touch command uses the current time. If you specify a file that does not exist, the touch command creates the file unless you specify the `-c` flag.

-- [IBM Documetation](https://www.ibm.com/docs/en/aix/7.3.0?topic=t-touch-command)

Update the access and modification times of each `FILE` to the current time.

A `FILE` argument that does not exist is created empty, unless `-c` or `-h` is supplied.

A `FILE` argument string of - is handled specially and causes touch to change the times of the file associated with standard output.

Mandatory arguments to long options are mandatory for short options too.

-- [Linux Man Pages](https://linux.die.net/man/1/touch) 
