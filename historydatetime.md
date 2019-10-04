####Q.3 How to make history display date and time as well?

If you want the history command to display the date and time of execution for each command, you can do this by exporting the HISTTIMEFORMAT variable in the following way:

`export HISTTIMEFORMAT="%F %T: "`

That's it. Now when you'll run the 'history' command, you'll see the date and time info in the output.
![History date time](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/historydatetime.PNG)

