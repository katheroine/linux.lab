[⌂ Home](../../README.md)
<!-- [▲ Previous: ]()
[▼ Next: ]() -->

# Filesystem

## Definition

In computing, a **file system** or **filesystem** (often abbreviated to *FS* or *fs*) *governs file organization and access*. A *local file system* is a capability of an *operating system* that services the applications running on the same computer. A *distributed file system* is a protocol that provides file access between networked computers.

A *file system* provides a data storage service that allows applications to share mass storage. Without a *file system*, applications could access the storage in incompatible ways that lead to resource contention, data corruption, and data loss.

There are many *file system* designs and implementations – with various structures and features and various resulting characteristics such as speed, flexibility, security, size, and more.

*File systems* have been developed for many types of storage devices, including hard disk drives (HDDs), solid-state drives (SSDs), magnetic tapes and optical discs.

A portion of the *computer main memory* can be set up as a *RAM disk* that serves as a storage device for a *file system*. *File systems* such as `tmpfs` can store files in *virtual memory*.

A *virtual file system* provides access to files that are either computed on request, called virtual files (for example those provided by procfs and sysfs), or are mapping into another, backing storage.

-- [Wikipedia](https://en.wikipedia.org/wiki/File_system)

***Files*** are logical units of information created by *processes*. A disk will usually contain thousands or even millions of them, each one independent of the others. In fact, if you think of each file as a kind of address space, you are not that far off, except that they are used to model the disk instead of modeling the RAM.
*Processes* can read existing files and create new ones if need be. Information stored in files must be persistent, that is, not be affected by process creation and termination. A file should disappear only when its owner explicitly removes it. Although operations for reading and writing files are the most common ones, there exist many others [...]
*Files* are managed by the *operating system*. How they are structured, named, accessed, used, protected, implemented, and managed are major topics in operating system design. As a whole, that part of the operating system dealing with files is known as the **file system** [...]

-- [Andrew S. Tanenbaum, Herbert Bos, *Modern Operating Systems*, Pearson 2015](https://en.wikipedia.org/wiki/Modern_Operating_Systems)

## UNIX file system

The UNIX file system is characterized by:
* a hierarchical structure,
* consisen treatment of file data,
* the ability to create and delete files,
* dynamic growth of files,
* the protection of file data,
* the treatment of peripheral devices (such as terminals and tape units) as files.

- [Maurice J. Bach, *The Design of the UNIX Operating System*, Pearson Education 1986, page 6](https://archive.org/details/DesignUNIXOperatingSystem/mode/2up)
