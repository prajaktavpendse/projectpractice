#                      Git Checkout


## Table of contents:

* Git checkout

* Checking out branch

* Difference between 'git clone' and 'git cheeckout'

* What is 'git checkout -b <new-branch>' ?

* What is 'git checkout -b <new-branch><existing-branch>' ?

* Git checkout a Remote branch

* Reference



# Git checkout

-------------------------------------------------------------------------------------------------
 
In Git terms, a "checkout" is the act of switching between different versions of a target entity. The git checkout command operates upon three distinct entities: files, commits, and branches.

In addition to the definition of "checkout" the phrase "checking out" is commonly used to imply the act of executing the git checkout command. 


# Checking out branch

-----------------------------------------------------------------------------------------------------

The git checkout command lets you navigate between the branches created by git branch. Checking out a branch updates the files in the working directory to match the version stored in that branch, and it tells Git to record all new commits on that branch.

Having new branch for each feature makes your work very easy.It makes you work on many unrelated features at the same time.Moreover branches also facilitate several collaborative workflows.

You can enter command `git branch` and hit enter button.List of available branches in the current repository will appear.

![here is screenshot of branches created by me in my repository:](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/git_branch.PNG)

As we can see in the screenshot,I have created two branches here namely checkout and cloning_forking

Now if you want to checkout the branch then hit command `git checkout <branch name>`

![here is screenshot](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/git_checkout.PNG)



# Difference between git clone and git checkout

------------------------------------------------------------------------------------------------------

The git checkout command may occasionally be confused with git clone. The difference between the two commands is that clone works to fetch code from a remote repository, alternatively checkout works to switch between versions of code already on the local system.

# What is `git checkout -b <new-branch>` ?

----------------------------------------------------------------------------------------------------

The git checkout command accepts a -b argument that acts as a convenience method which will create the new branch and immediately switch to it. You can work on multiple features in a single repository by switching between them with git checkout.

`git checkout -b <new-branch>` -This command will simultaneously creates and checks out <new-branch> .
The -b option is a convenience flag that tells Git to run git branch <new-branch> before running git checkout <new-branch>.

![Here is screenshot:](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/checkout_b.PNG)

----------------------------------------------------------------------------------------------------

# What is 'git checkout -b <new-branch> <exiisting-branch>' ?

-------------------------------------------------------------------------------------------------------

By default git **checkout -b** will base the new-branch off the current HEAD. An optional additional branch parameter can be passed to git checkout. In the above example, <existing-branch> is passed which then bases new-branch off of existing-branch instead of the current HEAD.

![Here is screenshot:](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/new_existing%20branch.PNG)

------------------------------------------------------------------------------------------------------

# Git checkout a Remote branch

------------------------------------------------------------------------------------------------------

When collaborating with a team it is common to utilize remote repositories. These repositories may be hosted and shared or they may be another colleague's local copy. Each remote repository will contain its own set of branches. In order to checkout a remote branch you have to first fetch the contents of the branch.

`git fetch --all`

Check branch like  a local branch:

`git checkout <remotebranch>`

Additionally you can checkout a new local branch and reset it to the remote branches last commit.

`git checkout -b <branchname>
git reset --hard origin/<branchname>`

-----------------------------------------------------------------------------------------------------

# Reference

-----------------------------------------------------------------------------------------------------

1. https://www.atlassian.com/git/tutorials/using-branches/git-checkout

2. https://git-scm.com/docs/git-checkout

-----------------------------------------------------------------------------------------------------