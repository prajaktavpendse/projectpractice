(1) What is VI?
VI stands for Visual, is an editor found on Unix like systems, (Linux for example). It can be used to create, open and edit files that contain text (non-binary). For example, we can create, open and edit .java files with VI

(2) How to create a new file with VI (or VIM)?
On the command line, type "vi filename.extension" without the quotes. 
For example, $ vi test_file.txt

(3) Could you please explain the different modes of vi?
Yes, vi has several modes, most important of them are:
(a) Visual: used to select, copy and paste text. type v to enter into visual mode (can vary on different systems)
(b) Text mode: Type i or <insert_key> to get into this mode. This is used to edit the file i.e. add, modify or delete contents. 
(c) Command mode: The default mode when vi starts. Here, we can enter different commands like :wq etc. Not used to change any file contents. 
(d) Note, I have clubbed command mode with "last line mode" here. 

(4) How would you create and save a text file in vi?
(a) Create a new file using the steps in (2) 
(b) Now you are in command mode. Type i or insert_key to enter insert mode. 
Add your file contents. 
(c) Once you are done, hit escape. You will get back to command mode. Then type :w <Enter>. This will "write" or save the contents of the file to disk, including creating the new file (if it previously didn't exist)
(d) Type q to exit (while in command mode). Alternatively, we can also type :wq to "write" and "quit" 

(5) Why use vim?
(a) On most Unix like distributions, it is the editor that comes by default. 
(b) So, learning it offers great advantage over others. 
(c) It is also highly customizable (vim plugins etc).