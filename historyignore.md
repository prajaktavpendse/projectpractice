>Q.5 How to make history not record a single command?

#This can be done by setting the HISTCONTROL variable to 'ignorespace.' This you can do in the following way:
 >export HISTCONTROL=ignorespace

Now whenever you run a command that you don't want to be recorded in history, just execute it with a leading space.
