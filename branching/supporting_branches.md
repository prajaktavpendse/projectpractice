# Supporting branches

Next to the main branches master and develop, our development model uses a variety of supporting branches to aid parallel development between team members, ease tracking of features, prepare for production releases and to assist in quickly fixing live production problems. Unlike the main branches, these branches always have a limited life time, since they will be removed eventually.

The different types of branches we may use are:

1. Feature branches
2. Release branches
3. Hotfix branches

Each of these branches have a specific purpose and are bound to strict rules as to which branches may be their originating branch and which branches must be their merge targets. We will walk through them in a minute.

By no means are these branches “special” from a technical perspective. The branch types are categorized by how we use them. They are of course plain old Git branches. 

# 1. Feature branches

![Feature branching diagram](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/Feature_branches.PNG)

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
