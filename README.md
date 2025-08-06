# Overview
Learn the basic fundamentals of using Shell.

## Introduction
Shell is used to issue commands to the operating system.


## Topics Covered

### Manipulating files and directories
- pwd -> tells you where you are(prints current working directory)
- ls -> lists all files and folders in the current directory
- cd -> changes directory to the specified one
- cp -> copies files to the specified directory or file
``` shell
cd . #-> current directory
cd .. #change to the folder above this one / parent folder
cd ~ # change directory to the home directory
cd / # change directory to the root directory
```
- mv -> moves file to the specified folder / renames files
- rm -> deletes files
- mkdir -> creates a new directory
- rmdir -> deletes directory

### Manipulating data
- cat -> prints out the contents of the file on the screen
- less -> prints the content of 1 page of a file at a go
- head -> prints the first 10 lines of a file
```shell
head -n 3 example.txt #prints the first three lines of the file
```
- man -> prints out what a command does
- cut -> select the columns in a file
```shell
cut -f 2-5 -d , #select columns 2 through 5 and columns 8, using comma as the separator". cut uses -f (meaning "fields") to specify columns and -d (meaning "delimiter") to specify the separator. You need to specify the latter because some files may use spaces, tabs, or colons to separate columns.
```
- history -> lists all the commands you have run
- grep -> takes a piece of text followed by one or more filenames and prints all of the lines in those files that contain that text.
Common flags:
-c: print a count of matching lines rather than the lines themselves
-h: do not print the names of files when searching multiple files
-i: ignore case (e.g., treat "Regression" and "regression" as matches)
-l: print the names of files that contain matches, not the matches
-n: print line numbers for matching lines
-v: invert the match, i.e., only show lines that don't match
