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
