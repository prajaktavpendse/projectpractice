(1) What is git?
Git is a tool for version source control. It works in distributed fashion.

(2) Why to use git?
In real life, there are many instances where we cannot do without source control. Sample these:
(a) Multiple developers making changes to a common set of files (aka repository). Here, synchronization is very important since all these changes are being made to a common set of files. 
(b) Reverting certain changes. Because of the "source control" nature of git, it becomes very easy to get rid of problematic changes and revert the code to a stable version. 
(c) Making simultaneous independent changes to the same code that should not interact with each other aka git branching

As a common person, git is simply the (more powerful) equivalent of Google docs. Just as Google docs allowsmultiple participants to view, edit and revert to previous revisions a document, git allows the same thing (with more features) for entire repos. 

(3) What about the distributed nature of git?
Yes, git is highly distributed, in the sense that all changes are first made locally (by cloning the repo) and then pushed to the common repository (remote). Quoting from Wikipedia, "every Git directory on every computer is a full-fledged repository with complete history and full version-tracking abilities, independent of network access or a central server."

(4) What is continuous integration
Lets say 5 developers are working on a shared set of files. Continous integration would mean perioidically consolidating their changes on a shared resource (machine). This is usually done at least once a day (several times a day is best). 

(5) Ok, why continous integration?
This is to make sure that all developers work with the latest available changes that their peers have made. If they don't then it could lead to issues consolidating the same changes at a later time, or even reduplication of efforts. 

(6) How does git allow continous integration?
git remote is a centralized shared repository that contains the merged changes from all the contributors. Periodically pushing to (and pulling) changes from remote ensures continous integration. 