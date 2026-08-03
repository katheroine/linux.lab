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
$ printf 'Hi,there!' > another_file
$ ls
another_file  other_file  some_file
$ cat another_file
Hi,there!$
```

