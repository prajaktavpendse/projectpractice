# **DEFINITION**

## A home directory is a special directory designated for your own personal usage. It may contain a variety of content including, scripts, symlinks, raw data, configuration files, and the publich_html folder. The home directory contains your cPanel username on the server.

# **DIFFERENCE BETWEEN CURRENT DIRECTORY AND WORKING DIRECTORY**

## Home directory is the default working directory when a user logs in. On the other hand, working directory is the user's current directory. Working directory can be changed. ... Home directory in Linux contains user's personal data, configuration files, settings of a software etc.

# IMPORTANT POINT TO REMEMBER:

### `HOME` isn’t usually considered customizable (too many other things depend on it), but it’s where Git looks for the global configuration file. If you want a truly portable Git installation, complete with global configuration, you can override HOME in the portable Git’s shell profile. 

### Git uses several environment variables to determine how it interfaces with the current repository.

### `GIT_DIR` is the location of the .git folder. If this isn’t specified, Git walks up the directory tree until it gets to ~ or /, looking for a .git directory at every step.

### `GIT_CEILING_DIRECTORIES` controls the behavior of searching for a .git directory. If you access directories that are slow to load (such as those on a tape drive, or across a slow network connection), you may want to have Git stop trying earlier than it might otherwise, especially if Git is invoked when building your shell prompt.

### `GIT_OBJECT_DIRECTORY` can be used to specify the location of the directory that usually resides at .git/objects.

### `GIT_ALTERNATE_OBJECT_DIRECTORIES` is a colon-separated list (formatted like /dir/one:/dir/two:…) which tells Git where to check for objects if they aren’t in GIT_OBJECT_DIRECTORY. If you happen to have a lot of projects with large files that have the exact same contents, this can be used to avoid storing too many copies of them.

