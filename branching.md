#  Git Branching

#What is git branching?

A branch in Git is simply a lightweight movable pointer to one of these commits. The default branch name in Git is master. As you initially make commits, you’re given a master branch that points to the last commit you made. Every time you commit, it moves forward automatically.

What happens if you create a new branch? Well, doing so creates a new pointer for you to move around. Let’s say you create a new branch called testing. You do this with the `git branch` command:

`$ git branch testing`

## Branching Workflow


>>The main branches ¶
The central repo holds two main branches with an infinite lifetime:       |
                                                                          |
1. master                                                                 | ![Main git branches](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/main_branches.PNG)
2. develop                                                                |
                                                                          |
The **master branch** at origin should be familiar to every Git user.     |
Parallel to the master branch, another branch exists called **develop**.  |  
                                                                          |
We consider **origin/master** to be the main branch                       |
where the source code of HEAD always reflects a production-ready state.   |
                                                                          |
We consider **origin/develop** to be the main branch                      |
where the source code of HEAD always reflects a state with the latest     |
delivered development changes for the next release.                       |
                                                                          |
When develop branch reaches a stable point and is ready to be released,   |
 all of the changes should be merged back into master somehow             |
 and then tagged with a release number.                                   |