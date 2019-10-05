#  Git Branching

#What is git branching?

A branch in Git is simply a lightweight movable pointer to one of these commits. The default branch name in Git is master. As you initially make commits, you’re given a master branch that points to the last commit you made. Every time you commit, it moves forward automatically.

What happens if you create a new branch? Well, doing so creates a new pointer for you to move around. Let’s say you create a new branch called testing. You do this with the `git branch` command:

`$ git branch testing`

****Branching Workflow****


# The main branches 

![Git main branches](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/main_branches.PNG)



The central repo holds two main branches with an infinite lifetime:     
                                                                          
# 1. master                                                                  
# 2. develop                                                                
                                                                          
The **master branch** at origin should be familiar to every Git user.Parallel to the master branch, another branch exists called **develop**.    
                                                                          
We consider **origin/master** to be the main branch where the source code of HEAD always reflects a production-ready state.   
                                                                          
We consider **origin/develop** to be the main branch where the source code of HEAD always reflects a state with the latest delivered development changes for the next release.                       
                                                                          
When develop branch reaches a stable point and is ready to be released,all of the changes should be merged back into master somehow and then tagged with a release number.

[Branching detail workflow](https://nvie.com/files/Git-branching-model.pdf)

# Supporting branches

Next to the main branches master and develop, our development model uses a variety of supporting branches to aid parallel development between team members, ease tracking of features, prepare for production releases and to assist in quickly fixing live production problems. Unlike the main branches, these branches always have a limited life time, since they will be removed eventually.

The different types of branches we may use are:

1. Feature branches
2. Release branches
3. Hotfix branches

Each of these branches have a specific purpose and are bound to strict rules as to which branches may be their originating branch and which branches must be their merge targets. We will walk through them in a minute.

By no means are these branches “special” from a technical perspective. The branch types are categorized by how we use them. They are of course plain old Git branches. 

# 1. Feature branches

May branch off from:
develop

Must merge back into:
develop

Branch naming convention:
anything except master, develop, release-*, or hotfix-*    

As name suggest,feature branches are use to create a new feature.These branches typically exist on develop repository.

# 2. Release branches

May branch off from:
develop

Must merge back into:
develop and master

Branch naming convention:
release-*  

Release branches support preparation of a new production release.They allow minor but fixes and prepares data for release.By doing all of this work on a release branch, the develop branch is cleared to receive features for the next big release.

# 3. Hotfix branches

![Hotfix branches](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/Hotfix_branches.PNG)

May branch off from:
master

Must merge back into:
develop and master

Branch naming convention:
hotfix-*      

Hotfix branch arise from the necessity to act immediately upon an undesired state of a live production version. When a critical bug in a production version must be resolved immediately, a hotfix branch may be branched off from the corresponding tag on the master branch that marks the production version.

The essence is that work of team members (on the develop branch) can continue, while another person is preparing a quick production fix.                      