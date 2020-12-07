# Laboration 3
Third Laboration centering around text editors and alike.


## Assignment 1
1. Created file easily.
2. `vi file` and in the editor used `:x`+ enter to save and exit.
3. `nano a.txt`, wrote some text and used CTRL+X and then enter to save and exit.

## Assignment 2
1. `find /usr | egrep "man"` worked pretty well for me to find all files with "man" in the name.
2. 
  - a) `ls -C1 /usr/bin | egrep "^a"` lists all files in `/usr/bin` starting with "a".
  - b) `ls -C1 /usr/bin | egrep "st$"` lists all file-names ending with "st".
  - c) `ls -C1 /usr/bin | egrep "p.*n"` lists all files with substrings that start with a "p" and ending with an "n", no     matter the characters in between. The substring will be as long as possible, so a filename like `penPseudonym.txt` would   be highlighted in "penPseudon"
3. For this question I used [this cheatsheet](https://cheatography.com/davechild/cheat-sheets/regular-expressions/) as a crutch, whenever I felt unsure of a definition. It will most likely be very helpful in the future.
  * a) The dot (`.`) character means any character (except newline '\n') 
  * b) The star (`*`) character means any amount, of any character. (0 or more)
  * c) The plus (`+`) character is similar to `*`, but with 1 or more instance of any character.
  * d) The question mark (`?`) means just one or zero instances of any character.
4. `ls /usr/bin -la | egrep "\->"` (The `\` is to disable the `-` command which would ruin the command)

## Assignment 3
1.
2.
3.

## Assignment 4
1.
2.
3.

## Assignment 5
1.
2.
3.

## Assignment 6
1.
2.
3.
