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

`pwd` - show current working directory path

`mkdir dirname` - create a directory

`rmdir dirname` - remove an empty directory

`rm -rf dirname` - delete a directory and all its contents

`touch filename.extension` - create file with filename and extension

`rm filename` - delete a file

`mv filename1 filename2` - rename a file

`ls -a` listing all hidden files

`cp dir1/filename dir2` - copying file from one directory into another

`history | grep prevcommand` - search terminal history for use of a previous command

`clear` - clears the cobwebs, gives you a visual fresh start!





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

----

`ls` - list files in the current working directory

`ls -a` - list files all files including hidden ones starting with .

`ls -l` - display files in longform with extra info

`ls -lh` - display files in longform with unit suffixes, reducing number of digits

`ls -lah` - display all files including hidden in longform with unit suffixes

`ls -t` - display files in chronological order, newest first

`ls -Glp` - display files in longform with directories coded in blue, and with /'s at the end of the pathname

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

`ls -d` - displays only directories

`ls -R` - recursively display all files in all directories inside current directory

`ls -m` - displays names of files as a comma separated list

`ls -r` - display files in reverse order

`ls -1` - display each file on a separate line



---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

xargs is used to pass constructed argument lists from other bash commands in executing a different command

 `find . -name "0*" | xargs head -n 1. ` - grabs all files in the current directory that start with the character "0" and prints the first line of each file