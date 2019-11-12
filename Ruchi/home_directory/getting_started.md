# **FINDING YOUR WAY AROUND**

1. As the name already implies, the command line is used to execute commands: you type something and confirm the command by hitting ENTER. Most of these commands are dependent on your current location - where "location" means a certain directory or path on your computer.
So, let's issue our first command to find out where we currently are:

`$ pwd`

You can easily remember this command when you know what it stands for: "print working directory". It will return the path to a local folder on your computer's disk.

2. To change this current working directory, you can use the "cd" command (where "cd" stands for "change directory"). For example, to move one directory upwards (into the current folder's parent folder), you can just call:

`$ cd ..`

3. To move into subfolders, you would call something like this:

`$ cd name-of-subfolder/sub-subfolder/`

4. Often, you'll see a special kind of path notation: "~". This sign stands for your user account's home folder. So, instead of typing something like "cd /Users/your-username/projects/", you should use this shorthand form:

`$ cd ~/projects/`

5. Also very important is the "ls" command that lists the file contents of a directory. I suggest you always use this command with two additional options: "-l" formats the output list a little more structured and "-a" also lists "hidden" files (which is helpful when working with version control). Showing the contents of the current directory works as follows:

`$ ls -la`

# **Working with Files**

## The most important file operations can be controlled with just a handful of commands.

1. Let's start by removing a file:

`$ rm path/to/file.ext`

2. When trying to delete a folder, however, please note that you'll have to add the "-r" flag (which stand for "recursive"):

`$ rm -r path/to/folder`

3. Moving a file is just as simple:

`$ mv path/to/file.ext different/path/file.ext`

*The "mv" command can also be used to rename a file:*

`$ mv old-filename.ext new-filename.ext`

4. If,instead of moving the file, you want to copy it, simply use "cp" instead of "mv".

5. Finally, to create a new folder, you call the "make directory" command:

`$ mkdir new-folder`
