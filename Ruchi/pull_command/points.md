# OPTIONS
## `-q`
 
### --quiet

*This is passed to both underlying git-fetch to squelch reporting of during transfer, and underlying git-merge to squelch output during merging.*

## -v
### --verbose

*Pass --verbose to git-fetch and git-merge.*

## --[no-]recurse-submodules[=yes|on-demand|no]

*This option controls if new commits of all populated submodules should be fetched and updated, too (see git-config[1] and gitmodules[5]).*

### If the checkout is done via rebase, local submodule commits are rebased as well.

### If the update is done via merge, the submodule conflicts are resolved and checked out.

## **EXAMPLES:**

Update the remote-tracking branches for the repository you cloned from, then merge one of them into your current branch:


`$ git pull

$ git pull origin`

Normally the branch merged in is the HEAD of the remote repository, but the choice is determined by the branch.<name>.remote and branch.<name>
.merge options; see git-config[1] for details.

Merge into the current branch the remote branch next:


$ git pull origin next

This leaves a copy of next temporarily in FETCH_HEAD, but does not update any remote-tracking branches. Using remote-tracking branches, the same can be done by invoking fetch and merge:


$ git fetch origin

$ git merge origin/next

If you tried a pull which resulted in complex conflicts and would want to start over, you can recover with git reset.
