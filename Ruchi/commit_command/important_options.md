# **OPTIONS**

There are a number of options that can be include with git commit. 

**1. `The -m Option`**

The most common option used with git commit is the -m option. The -m stands for message. When calling git commit, it is required to include a message. The message should be a short description of the changes being committed. The message should be at the end of the command and it must be wrapped in quotations " ".

*An example of how to use the -m option

*git commit -m "My message"*

**2. `The -a Option`**

The -a stands for all. This option automatically stages all modified files to be committed. If new files are added the -a option will not stage those new files. Only files that the Git repository is aware of will be committed.

*For example


Let’s say that you have a README.md file that has already been committed to your repository. If you make changes to this file, you can use the -a option in your commit command to stage and add the changes to your repository. However, what if you also added a new file called index.html? The -a option will not stage the index.html as it does not currently exist in the repository. When new files have been added, the git add command should be invoked in order to stage the files before they can be committed to the repository.

An example of how to use the -a option

*git commit -am “My new changes”*

**3. `The —amend Option`**

The --amend option allows you to change your last commit. Let’s say you just committed and you made a mistake in your commit log message. You can conveniently modify the most recent commit using the command

*An example of how to use the-amend option

*git commit --amend -m "an updated commit message"*

**4. `-v or —verbose Option`**

The -v or --verbose option is used without the -m option. The -v option can be useful when you wish to edit a Git commit message in your default editor while being able to see the changes you made for the commit. The command opens your default text editor with a commit message template as well as a copy of the changes you made for this commit. 





