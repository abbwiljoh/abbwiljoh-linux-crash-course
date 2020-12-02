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

6. Using `cat` I can print the contents of one or more files in the terminal. With `more` you can print the contents of a file like with `cat`, but with just one file, and one page at a time. `less` "opens" the whole file, and you can search for strings with `/search_word`

7. 
  * a) To search for a specific word in a file opened with `less`, use a forward slash and write your search term (`/search_word`)
  * b) When in the file opened with `less`, write `p` to get to the first line in the file.
  * c) Use `G` to go to the last line of the file.


### Assignment 5
1. 
  * a) `find` finds all files and directories with the specified name, in the specified location.
  * b) `locate` finds *one* file or directory matching the given name.
  * c) `whereis` is a command for finding the executable and man page of a command or program.
  * d) `which` gives the path for the executable file of a command.
2. Use flag `-iname` for a case insensitive.

### Assignment 6
1.  
  * a) `cp Lab2Test.txt Lab2Test_backup.txt` is the command I used. 
  * b)   
  * `-v` "verbose". Explains what is done
  * `-u` "update". Copy only when the copied file or directory is newer than the destination file, or when there is no existing destination file.
  * '-r' "recursive". Copies directories recursivly
  * `-p` "preserve". Shorthand for `--preserve=mode,ownerships,timestamps`.
  * `-b` "backup". Backs up files without an argument.
  * `-i` "interactive". Prompt before overwrite.
  
2. Working: a, g, h. Not working: You cannot copy a file into the same file. You cannot copy a file into two different files in the same directory. Also you can't copy into the same directory and another at the same time. You cannot copy a directory into a file. 

3. To copy all files in a directory with `.txt`-file extension use `cp *.txt subdir2`.

4. 
  * a) `mv file2.txt subdir2` to move `file2.txt` to `subdir2/`
  * b) To remove `file4.txt` from subdirectory `subdir1/`, use `rm subdir1/file4.txt`

5. `mv * subdir2/` There will be an error trying to move subdir2/ to itself, but every other file will be moved.

### Assignment 7
1. 
  * `tar` An archiving utility which stores multiple files in the same file.
  * `gzip` Compress or expand files, reduces their sizes
  * `gunzip` Decompresses the `gzip`-compressed files and alike.

2. (used `tar -cf abcdef.tar *`)

3. From the subdirectory `unpack_test` I used the command `tar -xf ../abcdef.tar `

4. used `gzip abcdef.tar` then `tar -xf abcdef.tar.gz`.

### Assignment 8
1. The `noclobber`-option disables the ability to overwrite existing files with the `>`-command.
2. I used `ls Lab2Test/ | wc -w Lab2test` and got the answer `3` as I had three directories there.
3. 
  * a) From `home` I created a file called `listing.log`. To redirect filenames of `/usr/bin/` to it I used 
  `ls /usr/bin/ > ~/listing.log`
  * b) Used `ls /etc >> listing.log`
4. 
  * a) `cat Documents/Laboration2/numbers.txt | sort -rn` to sort the numbers from largest --> smallest. To reverse order, just remove `-r`.
  * b) `cat Documents/Laboration2/numbers.txt | sort -rnu` to sort with just unique items.
  * c) `sort numbers.txt -n > sorted_numbers.txt` to redirect sorted list to `sorted_numbers.txt`-file.
5. `ls -a|head -c 10|sort -n` ? I do not know...
