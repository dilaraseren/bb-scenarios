## Detailed Archiving with Man Command
To better understand the usage of these commands, you can get detailed information about each one by using the man command.
The **man** (manual) command is a command available on Linux and Unix-based operating systems and shows guides with information on using other commands. The **man** command provides users with detailed information about the system's commands, files, libraries, processes, settings, and other important elements.
You can use the **man** command as follows:
```sh
man command_name
```
The basic parameters of the archiving commands are as follows.
-c: Archive creation mode
-x: Unarchive mode
-v: Gives detailed output during processing
-f: Specifies the archive file name
-z: Compress with gzip
-j: Compress with Bzip2
-J: Compress with Xz

Using the man gzip command, you can see the gzip command's usage and all its options. For example, with the -c option you can print the compressed file to standard output:
```sh
man gzip
```