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
