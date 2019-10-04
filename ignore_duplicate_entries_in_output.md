####>Q.8 How to make history ignore duplicate entries in output?

This can be done by setting HISTCONTROL variable to 'ignoreboth' and 'erasedups'.You can do it in following way:

>echo HISTCONTROL=ignoreboth:erasedups
