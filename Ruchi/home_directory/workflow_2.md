# **How do I change the default location for Git Bash on Windows?**

## Type git bash in search

## Right click on it and choose open file location

## Right click on it and choose properties

## At target remove --cd-to-home from "C:\Program Files\Git\git-bash.exe" --cd-to-home

## At start in put the path of the directory you want it to start at for example Start in: C:\xampp\htdocs

# **OR**

## Hit windows key and type: env; then click Edit environment variables for your account (control panel)

## Under "User variables for ...."; hit New button

## Variable Name: HOME

## Variable value: path where you would like `~/` to be in git bash

## Open a git bash session and test it by typing: pwd and double check by doing `cd ~/` && `pwd`


