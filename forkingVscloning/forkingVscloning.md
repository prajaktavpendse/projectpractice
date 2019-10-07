# Forking Vs Cloning

-----------------------------------------------------------------------------------------------

When you are **Forking** a repository you are creating a copy of repository under the GitHub Id. Any changes made to the original original repository will be reflected back to your forked repository. However, if you make any changes to your forked repository you will have to explicitly create a pull request to the original repository. When your pull request is approved by the administrator of the original repository, then your changes will be merged with the existing original code-base. Until then, your changes will be reflected only in the copy you forked.

A **Clone** is where you have proper duplication, and separation between, two versions of a repository. When one repository is amended, the new content must be actively copied to the other repository using a push command. And changes in the other repository are fetched.

For example, if you want to make changes to any of its cookbooks, you will need to fork the repository, which creates an editable copy of the entire repository (including all of its branches and commits) in your own source control management (e.g. GitHub) account. Later, if you want to contribute back to the original project, you can make a pull request to the owner of the original cookbook repository so that your submitted changes can be merged into the main branch.