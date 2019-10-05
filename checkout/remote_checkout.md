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