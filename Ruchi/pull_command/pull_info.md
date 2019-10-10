# GIT PULL DEFINITION 

## The git pull command is used to fetch and download content from a remote repository and immediately update the local repository to match that content. Merging remote upstream changes into your local repository is a common task in Git-based collaboration work flows.

# SYNOPSIS

## `git pull [<options>] [<repository> [<refspec>…​]]`

# DESCRIPTION

## Incorporates changes from a remote repository into the current branch. In its default mode, git pull is shorthand for git fetch followed by git merge FETCH_HEAD.

## More precisely, git pull runs git fetch with the given parameters and calls git merge to merge the retrieved branch heads into the current branch. With --rebase, it runs git rebase instead of git merge.

## <repository> should be the name of a remote repository as passed to git-fetch[1]. <refspec> can name an arbitrary remote ref (for example, the name of a tag) or even a collection of refs with corresponding remote-tracking branches (e.g., refs/heads/*:refs/remotes/origin/*), but usually it is the name of a branch in the remote repository.

## Default values for <repository> and <branch> are read from the "remote" and "merge" configuration for the current branch as set by git-branch[1] --track.

![IMAGES](https://www.jquery-az.com/wp-content/uploads/2018/07/10.0_3-Git-pull-remote.png)


