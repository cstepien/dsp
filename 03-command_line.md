# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands

Here's a list of items with which you should be familiar:
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)

> > 1) `pwd` show current working directory path  
> > 2) `mkdir` creating a directory  
> > 3) `rm -r` deleting a directory with children (`rmdir` will delete empty directories)
> > 4) `touch` creating a file using `touch` command  
> > 5) `rm` deleting a file  
> > 6) `mv` moving a file from one directory to another (and renaming a file if no directory specified)
> > 7) `ls -a` listing hidden files  
> > 8) `cp` copying a file from one directory to another  
> > 9) `echo` write arguments to output  
> > 10) `man` opens user manual for the argument entered
---

### Q2.  List Files in Unix

What do the following commands do:
`ls`
`ls -a`
`ls -l`
`ls -lh`
`ls -lah`
`ls -t`
`ls -Glp`

> > 1) `ls` lists all files and directories in the current working directory  
> > 2) `ls -a` lists files beginning with `.` in addition to the above `ls` files and directories  
> > 3) `ls -l` lists files and directories with more details about each object  
> > 4) `ls -lh` lists files and directories with more details, and file size in human-readable format (K, M, G)  
> > 5) `ls -lah` lists all content including hidden files, in long format, human-readable  
> > 6) `ls -t` lists files and directories in the order they were last edited  
> > 7) `ls -Glp` lists files and directories in long format, with a backslash before directories and showing files and directories in different colors

---

### Q3.  More List Files in Unix

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > 1) `ls -alt` is a combo of ls options that lists all contents including hidden ones, in long format, and ordered by most recently edited  
> > 2) `ls -1` displays files and directories 1 per line, easier to read  
> > 3) `ls -R` displays subdirectories and files in addition to files in working directory  
> > 4) `ls -F` flags filenames with a slash for directories, * for executable, and other flags  
> > 5) `ls -S` sort files by size

---

### Q4.  Xargs

What does `xargs` do? Give an example of how to use it.

> > `xargs` allows for creating an execution pipeline for standard input, for commands that can't directly take standard input.  One example is piping in arguments to `mkdir` using `xargs` : `echo "one two three" | xargs mkdir` will make three new directories (called one, two and three) in the working directory. Typing `echo "one two three" | xargs rmdir` will remove them. 



