# MASTER BRANCHING

>A **branch** is essentially is a unique set of code changes with a 
>unique name. Each repository can have one or more branches. The main 
>branch — the one where all changes eventually get merged back into, and 
>is called master.

>In Git, **master** is a naming convention for a branch. After cloning
>a project from a remote server, the resulting local repository has a 
>single local branch: the so-called **master** branch. This means that 
>**master** can be seen as a repository's **default** branch.

- In the GitHub Desktop client, switch to the branch you want to merge the development branch into. From the branch selector, select the master branch.
- Go to Branch > Merge into Current Branch.
- In the merge window, select the development branch, and then click Merge development into master.

>If we want to merge two branches, we have to be in the destination 
>branch. So if we want to merge doc1 to master, we need to be in the 
>master branch. If you want to know on which branch are you, you can use 
>git status. Then the only thing run is the git merge <name-of-branch>. 
>So, because we want to merge the doc1 branch, we are going to execute 
>git merge doc1.


![master](https://user-images.githubusercontent.com/54865970/66374832-ded00480-e979-11e9-916f-ca7f53cce558.png)
