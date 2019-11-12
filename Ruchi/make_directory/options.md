## **The mkdir command is is used to create new directories.**

### A directory, referred to as a folder in some operating systems, appears to the user as a container for other directories and files. However, Unix-like operating systems treat directories as merely a special type of file that contains a list of file names and their corresponding inode numbers. Each inode number refers to an inode, which is located in inode tables (which are kept at strategic locations around the filesystem) and which contains all information about a file (e.g., size, permissions and date of creation) except its name and the actual data that the file contains.

## **mkdir has the following syntax:**

`mkdir [option] directory_name(s)`

### Directories created by mkdir automatically include two hidden directories, one representing the directory just created (and represented by a single dot) and the other representing its parent directory (and represented by two consecutive dots). This can be seen by using the ls (i.e., list) command with its -a option, which tells ls to show all directories and files, (including hidden ones) in any directory provided to it as an argument, or in the current directory if there are no arguments, i.e.,

`ls -a`

### `mkdir's -m` option is used to control the permissions of new directories. New directories are by default created with the read, write and execute (i.e., run as a program if a program) permissions enabled for the owner (i.e., the creator of the directory by default) and group and the read and execute permissions enabled for other users. 

### The `-p` (i.e., parents) option creates the specified intermediate directories for a new directory if they do not already exist. For example, it can be used to create the following directory structure:

mkdir -p food/fruit/citrus/oranges

