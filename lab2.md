### Assignment 1
1. In the GUI, directories have a folder icon. I could not find `local` or `messages`.
2. Copying and pasting the file in the same folder creates a file with the suffix *(copy {number})*

3. *`SUCCESSFULLY DELETED`*.
4. In the file manager toolbar, go to "view" and check the box called "Show hidden items". Voila!

### Assignment 2
1. 
  * a) `ls -a` lists all files and directories, even hidden.
  * b) `ls -F` lists directories with a '/' appended.
  * c) `ls -l` lists files and directories in an extended format, with more data like time and date created.
2. `cd` is 'change directories' and lets you move between directories. `pwd` prints current working directory (path).

### Assignment 3
1. `/home` contains the users and their respective directories.
`/usr` contains user items, like games and such.
`/var` contains locals, cache and a /tmp directory.
`/tmp` is where temporarily used files are stored. 
`/etc` has configuration files, et cetera.

2. 
  * a) *Shell built-in ccommands* are built into the shell, they work as long as the terminal works. *external commands* are not bulit-in, they need to be found in  files and directories. The executable files for the commands can be found in the $PATH-environmental variable.
  * b) `cd` and `umask` are internal commands.
  * c) External commands are usually stored in `/usr/bin`


### Assignment 4
1. 
  * a) To create a directory I used the command `mkdir`.
  * b) Any characters can be used, but special characters get put inside quotation marks. You cannot name an already existing file.
2. I wrote a file with `nano Lab2Test.txt` and a file with `cat > Lab2Test_1.txt`.
3. 
  * a) `/home/abbwiljoh/Lab2Test/subdir1`
  * b) `subdir1`
4. 
  * a) The dot `.` represents the current working directory, and can be used when copying files to the current directory among other things.
  * b) The double dot `.` represents the parent directory (the directory that contains the current directory). It can be used to go back up the chain of directories, instead of finding your way from the root directory
5. 
  * a) `*` is the globbing command for a range between 1 and an infinite amount of any character combination. You can put it in a `find` command in any place in the search term and find all instances of that. The `?` represents just *one* unknown character, unlike the infinite amount of the `*`. You use it to get more precise results when you know the amount of characters in a name for instance.
  * b) In the `home` -directory you can use `ls D*`, which (in the default version) will list `Desktop`, `Downloads` and `Documents`.
  * c) In the directory I created `Lab2Test/` I used `ls subdir?` to list both `subdir1` and `subdir2`.
6.
7.

### Assignment 5
1.
2.

### Assignment 6
1.
2.
3.
4.
5.

### Assignment 7
1.
2.
3.
4.

### Assignment 8
1.
2.
3.
4.
5.
