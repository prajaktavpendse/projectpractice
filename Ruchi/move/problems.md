# **PROBLEMS**

## **A. In your Git working directory, you wish to rename a previously committed file named mycoolclass.cs to myCoolClass.cs and commit the newly renamed file.**

## **Solution**

1. Change to the directory containing your repository: for example,
cd /Repo/MyProject/.

2. Run the following git command:

git mv mycoolclass.cs myCoolClass.cs

*There will be no output.*

3. Run the following command to commit the change:

git commit --message 'Rename the cool class'

The output will like the following:

`git commit --message ‘Rename the cool class’
   [master c6eed66] Rename the coolclass
      1 file changed, 0 insertions(+), 0 deletions(-)
         rename thecoolclass.cs => theCoolClass.cs (100%)`

### You’ve renamed thecoolclass.cs to theCoolClass.cs and committed it.

## **B. What if the new file name already exists?**

## If the filename you move to already exists, you’ll need to use the following command

`git mv -f` 

or

`git mv --force`

*to request that Git overwrite whatever file is at the destination. If the destination file hasn’t already been added or committed to Git, then it won’t be possible to retrieve the contents if you erroneously asked Git to overwrite it.*

## **C. Does GIT MV preserve history?**

## Answers. Git detects renames rather than persisting the operation with the commit, so whether you use git mv or mv doesn't matter. It is possible to rename a file and keep the history intact, although it causes the file to be renamed throughout the entire history of the repository.

## **D. How to use mv command in Linux?**

## If you want to just rename a file, you can use the mv command in the following way:

  mv [filename] [new_filename]

  For example:

  mv names.txt fullnames.txt

## if the requirement is to move a file to a new location, use the mv command in the following way:

mv [filename] [dest-dir]

For example:

mv fullnames.txt /home/ruchi/Downloads

## **E. How to make sure mv prompts before overwriting?**

## By default, the mv command doesn't prompt when the operation involves overwriting an existing file. For example, the following screenshot shows the existing full_names.txt was overwritten by mv without any warning or notification.

## However, if you want, you can force mv to prompt by using the -i command line option.

## `mv -i [file_name] [new_file_name]`

*So the above screenshots clearly shows that -i leads to mv asking for user permission before overwriting an existing file. Please note that in case you want to explicitly specify that you don't want mv to prompt before overwriting, then use the -f command line option.*

## **F. How to make mv remove trailing slashes (if any) from source argument?**

## To remove any trailing slashes from source arguments, use the --strip-trailing-slashes command line option.

### `mv --strip-trailing-slashes [source][dest]`

## **G. How to make mv treat destination as normal file?**

## To be absolutely sure that the destination entity is treated as a normal file (and not a directory), use the -T command line option.

### `mv -T [source] [dest]`

## **H. How to make mv move file only when its newer than destination file?**

*Suppose there exists a file named fullnames.txt in Downloads directory of your system, and there's a file with same name in your home directory. Now, you want to update ~/Downloads/fullnames.txt with ~/fullnames.txt, but only when the latter is newer. Then in this case, you'll have to use the -u command line option.*

### `mv -u ~/fullnames.txt ~/Downloads/fullnames.txt`

*This option is particularly useful in cases when you need to take such decisions from within a shell script.*

## **I. How make mv emit details of what all it is doing?**

## If you want mv to output information explaining what exactly it's doing, then use the -v command line option.

### `mv -v [filename] [new_filename]`


