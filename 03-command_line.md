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

> > pwd
mkdir
rm -r (or -rf to suppress messages asking if you want to delete every file in the directory)
touch
rm
mv old_name new_name
ls -a
cp [optional source] destination
man <command> : search manual for command's options
man -k : search manual for commands using keywords
cat : show data in file
head: list the fist 10 lines. Helpful for peeking at long files
echo: print
nl: number of lines


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

> > ls: list files and directories in the current directory
-a: list all. This includes hidden files
-l: list files in long formate (shows permissions)
-lh: long format with reasonable file size (human readable)
-lah: long format with reasonable file size including hidden files
-t: sort by time and date (last edit time)
-Glp: use long format (l), but don't print group names (G), and display directories with a / (p)

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > -d: display only directories
-R: displays subdirectories
-F: displays directories with / (like p), but also flags files with *
-i: lists the innode for each file
-1: displays each entry on one line

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > Xargs allows you to feed a stream of multiple inputs from STDIN into a command. One example would be to feed into the command "find" to find multiple types of files. For example: Xargs -0 find filename. You could then input ".mp4", ".mkv", and however many file types you wanted (although Linux does not necesitate file type endings for names).

 

