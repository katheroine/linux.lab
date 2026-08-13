# Files managing

## Creating files

**`touch`**

```console
$ ls
$ touch some_file
$ ls
some_file
$ cat some_file
```

**`echo`**

```console
$ echo 'Hello, world!' > other_file
$ ls
other_file  some_file
$ cat other_file
Hello, world!
```

**`printf`**

```console
$ printf 'Hi, there!'"\n" > another_file
$ ls
another_file  other_file  some_file
$ cat another_file
Hi, there!
```

**`cat`**

```console
$ cat > yet_another_file
Roses are red and cornflower is blue,
I like Linux and hope that you too.
$ ls
another_file  other_file  some_file  yet_another_file
$ cat yet_another_file
Roses are red and cornflower is blue,
I like Linux and hope that you too.
```

**`>`** - output redirection

```console
$ > further_file
$ ls
another_file  other_file_again  yet_another_file
further_file  some_file
$ cat further_file
```

## Reading files

**`cat`**

```console
$ cat some_content
Videmus nunc per speculum
et in aeingmate.

```

```console
$ cat content_1
Stat rosa pristina nomine.
$ cat content_2
Nomina nuda tenemus.
$ cat content_1 content_2
Stat rosa pristina nomine.
Nomina nuda tenemus.
```

**`more`**

```console
$ more some_content
Videmus nunc per speculum
et in aeingmate.

```

```console
$ more content_1
Stat rosa pristina nomine.
$ more content_2
Nomina nuda tenemus.
$ more content_1 content_2
::::::::::::::
content_1
::::::::::::::
Stat rosa pristina nomine.
::::::::::::::
content_2
::::::::::::::
Nomina nuda tenemus.
```

**`less`**

```console
$ less some_content

```

## Updating files

**`cat`**

```console
$ cat some_text
Omnis mundi creatura
quasi liber et pictura
$ echo 'nobis est in speculum.' >> some_text
$ cat some_text
Omnis mundi creatura
quasi liber et pictura
nobis est in speculum.
```

## Deleting files

**`rm`**

```console
$ ls
$ touch file1 file2 file3 file4 file5
$ ls
file1  file2  file3  file4  file5
$ rm file2
$ ls
file1  file3  file4  file5
$ rm file3 file4
$ ls
file1  file5
```

**`find`**

```console
$ find file5 -delete
$ ls
file1
```

## Renaming files

**`mv`**

```console
$ ls
some_file
$ mv some_file renamed_file
$ ls
renamed_file
```

**`rename`**

```console
$ ls
some_file
$ rename some_file renamed_file some_file
$ ls
renamed_file
```

## Listing files

**`ls`**

```console
$ ls
another_file  file2       some_directory
file1         other_file  some_file
$ ls ./
another_file  file2       some_directory
file1         other_file  some_file
$ ls -l
total 4
-rw------- 1 u0_a79 u0_a79    0 Aug 11 08:41 another_file
-rw------- 1 u0_a79 u0_a79    0 Aug 11 08:41 file1
-rw------- 1 u0_a79 u0_a79    0 Aug 11 08:41 file2
-rw------- 1 u0_a79 u0_a79    0 Aug 11 08:41 other_file
drwx------ 2 u0_a79 u0_a79 3488 Aug 11 08:50 some_directory
-rw------- 1 u0_a79 u0_a79    0 Aug 11 08:41 some_file
$ ls -a
.   another_file  file2       some_directory
..  file1         other_file  some_file
$ ls -al
total 11
drwx------ 3 u0_a79 u0_a79 3488 Aug 11 08:49 .
drwx------ 5 u0_a79 u0_a79 3488 Aug 11 08:40 ..
-rw------- 1 u0_a79 u0_a79    0 Aug 11 08:41 another_file
-rw------- 1 u0_a79 u0_a79    0 Aug 11 08:41 file1
-rw------- 1 u0_a79 u0_a79    0 Aug 11 08:41 file2
-rw------- 1 u0_a79 u0_a79    0 Aug 11 08:41 other_file
drwx------ 2 u0_a79 u0_a79 3488 Aug 11 08:50 some_directory
-rw------- 1 u0_a79 u0_a79    0 Aug 11 08:41 some_file
$ ls some_directory
file_1  file_2  file_3
```

**`tree`**

```console
$ tree
.
├── another_file
├── file1
├── file2
├── other_file
├── some_directory
│   ├── file_1
│   ├── file_2
│   └── file_3
└── some_file

2 directories, 8 files
$ tree ./
./
├── another_file
├── file1
├── file2
├── other_file
├── some_directory
│   ├── file_1
│   ├── file_2
│   └── file_3
└── some_file

2 directories, 8 files
$ tree some_directory/
some_directory/
├── file_1
├── file_2
└── file_3

1 directory, 3 files
```

# Directories managing

## Creating directories

**`mkdir`**

```console
$ ls
$ mkdir some_directory
$ ls
some_directory
$ mkdir other_directory another_directory
$ ls
another_directory  other_directory  some_directory
$ ls -l
total 11
drwx------ 2 u0_a79 u0_a79 3488 Aug 12 08:40 another_directory
drwx------ 2 u0_a79 u0_a79 3488 Aug 12 08:40 other_directory
drwx------ 2 u0_a79 u0_a79 3488 Aug 12 08:38 some_directory
```

## Deleting directories

**`rmdir`**

```console
$ ls
another_directory  other_directory  some_directory
$ rmdir some_directory
$ ls
another_directory  other_directory
$ rmdir other_directory another_directory
$ ls
```
