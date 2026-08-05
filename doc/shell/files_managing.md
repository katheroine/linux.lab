5# Files managing

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

**`more`**

```console
$ more some_content
Videmus nunc per speculum
et in aeingmate.

```

**`less`**


```console
$ less some_content

```
