# FILE PATHS IN LINUX

> A path is a location that is unique to a file in a file system. It is 
> a list of derectories that tell you where to look for programs. But 
> different operating system have different ways to add a new directory.

> .bashrc is a shell script that Bash runs whenever it is started 
> interactively. It initializes an interactive shell session. You can 
> put any command in that file that you could type at the command prompt.

## SYNTAX:

- open .bashrc file in your home directory

- then add 

''' python
export PATH="your-dir:$PATH" 
'''
where dir is the directory you want

- save the .bashrc file