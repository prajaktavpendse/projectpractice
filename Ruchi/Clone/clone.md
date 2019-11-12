# **DEFINING GIT CLONE**

## git clone is a Git command line utility which is used to target an existing repository and create a clone, or copy of the target repository.

# **USAGE**

### git clone is primarily used to point to an existing repo and make a clone or copy of that repo at in a new directory, at another location. The original repository can be located on the local filesystem or on remote machine accessible supported protocols. The git clone command copies an existing Git repository. This is sort of like SVN checkout, except the â€œworking copyâ€ is a full-fledged Git repositoryâ€”it has its own history, manages its own files, and is a completely isolated environment from the original repository.

### As a convenience, cloning automatically creates a remote connection called "origin" pointing back to the original repository. This makes it very easy to interact with a central repository. This automatic connection is established by creating Git refs to the remote branch heads under refs/remotes/origin and by initializing remote.origin.url and remote.origin.fetch configuration variables.

### An example demonstrating using git clone can be found on the setting up a repository guide. The example below demonstrates how to obtain a local copy of a central repository stored on a server accessible at example.com using the SSH username john:

`git clone ssh://john@example.com/path/to/my-project.git 
cd my-project
Start working on the project`

*The first command initializes a new Git repository in the my-project folder on your local machine and populates it with the contents of the central repository. Then, you can cd into the project and start editing files, committing snapshots, and interacting with other repositories. Also note that the .git extension is omitted from the cloned repository. This reflects the non-bare status of the local copy.*

### Cloning to a specific folder

`git clone <repo> <directory>`

### Clone the repository located at <repo> into the folder called ~<directory>! on the local machine.

### Cloning a specific tag

`Git clone --branch <tag> <repo>`

Clone the repository located at <repo> and only clone the ref for <tag>.

### Shallow clone

`git clone -depth=1 <repo>`

