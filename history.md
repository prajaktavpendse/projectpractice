#                       'history' command

==========================================================================

Table of Contents:
1. Linux history command
2. How does history command work?
3. How to make history display date and time as well?
4. How to make history stop recording commands?
5. How to make history not record a single command?
6. How to perform quick history search?
7. How to run the previous command?
8. How to make history ignore duplicate entries in output?
9. How to clear history?
![*Wanna know more about history command!*](https://linux.die.net/man/3/history)




>Q.1Linux history command .
If you know how to effectively utilize your command line history, you can save a lot of time on daily basis.
history command - that gives you a list of commands you've executed earlier.

>Q.2How does history command work?
Usage of history command is simple- just execute the 'history' command
![History command](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/history.PNG)

You can also use 'history|more' command to get more details about history.

> Q.3 How to make history display date and time as well?
If you want the history command to display the date and time of execution for each command, you can do this by exporting the HISTTIMEFORMAT variable in the following way:

`export HISTTIMEFORMAT="%F %T: "`

That's it. Now when you'll run the 'history' command, you'll see the date and time info in the output.
![History date time](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/historydatetime.PNG)

>Q.4 How to make history stop recording commands?
If a situation arises wherein you do not want the system to save your commands history, then you can do this using the HISTSIZE variable. Just export it with zero as its value, and you're good.

Please refer below image:
![Clear history](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/historyclear.PNG)

>Q.5 How to make history not record a single command?
This can be done by setting the HISTCONTROL variable to 'ignorespace.' This you can do in the following way:
 >export HISTCONTROL=ignorespace

Now whenever you run a command that you don't want to be recorded in history, just execute it with a leading space.

>Q.6 How to perform quick history search?
You can perform quick history search by *'reverse-i-search'* method.This method is quite easy.

Steps to be followed for quick search:
1. Press Ctrl +R and you see command prompt turning into something like this:
![Quick history search step 1](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/Quicksearch1.PNG)
2. Now type the keyword you want to search, and you'll see matching suggestions from history on the right.
Like here I entered word 'added'
![Quick history search step 2](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/Quickhistorysearch2.PNG)
3. If this is not what you are looking for, you can get the next matching result by pressing CTRL+R again.

You can run this command and get result quickly.

>Q.7 How to run the previous command?
There are two easy ways to run previous command.
1. Press Ctrl +P
2. OR you can run below command on command prompt:
>!!
3. In case you need second last command then you can do that in following way:
>!-1
So on and so forth.

>Q.8 How to make history ignore duplicate entries in output?
This can be done by setting HISTCONTROL variable to 'ignoreboth' and 'erasedups'.You can do it in following way:
>echo HISTCONTROL=ignoreboth:erasedups

> Q.9 How to clear history?
Existing history can be cleare by following way:
>history -c

![Wanna know more about 'history' command?]||(https://linux.die.net/man/3/history)||
