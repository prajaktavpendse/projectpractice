# Forking Vs Cloning

*What is forking?*

A **fork** is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.

The Forking Workflow is fundamentally different than other popular Git workflows. Instead of using a single server-side repository to act as the “central” codebase, it gives every developer their own server-side repository.This means that each contributor has not one, but two Git repositories: a private local one and a public server-side one. The Forking Workflow is most often seen in public open source projects.

Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.

Steps to use forking feature :

1. Fork the repository.

![Where is this forking option in the github?](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/Forking.PNG)


2. Make the fix.

3. Submit a pull request to the project owner.








When you are Forking a repository you are creating a copy of repository under the GitHub Id. Any changes made to the original original repository will be reflected back to your forked repository. However, if you make any changes to your forked repository you will have to explicitly create a pull request to the original repository. When your pull request is approved by the administrator of the original repository, then your changes will be merged with the existing original code-base. Until then, your changes will be reflected only in the copy you forked.

A Clone is where you have proper duplication, and separation between, two versions of a repository. When one repository is amended, the new content must be actively copied to the other repository using a push command. And changes in the other repository are fetched.