 # ***Basic Linux Commands :-***

 ## 1. pwd Command :- 
   This command is used to find out the path of the current directory(folder). 
      This command will return an absolute path, which is a path of all directories that starts with a forward slash(/). 
       An example of an absolute path is:- 
       /home/username .
    
    
 ## 2. cd command :-
       This command is used to navigate through linux files and directories. 
       It either requires a full path or name of the directory depending on the current directory you are in.
       
       Let’s say you’re in /home/username/Documents and you want to go to Photos, a subdirectory of Documents. To do so, simply type the following command: cd Photos.
       Now if you want to switch to a completely new directory, say /home/username/Books. In this case, you have to type cd followed by the directory’s absolute path: cd /home/username/Books.

       Some shortcuts:- 
       -> cd.. (with two dots) to move one directory up.
       -> cd to go straight to the home folder.
       -> cd- (with hypen) to move to your previous directory.
  **NOTE:- You have to type the directories' names exactly as it is becouse Linux's shell is case sensitive.**


 ## 3. ls commmand:-
       This command is used to list contents os a directory. By default, this will display content of your current working directory.
       If you want to view contents of other directories, type ls and then the directory's path.
       For example:- /homes/username/Movies to view contents of Movies
       
       Variations in this command:-
       - ls -R will list all the files in teh sub-directories as well.
       - ls -a will show all the hidden files.
       - ls al will list the files and directories with detailed information like owner, size etc.
       
       
 ## 4. cat command:- 
       The cat command is a multi-purpose utility in the Linux system. 
       It can be used to create a file, display content of the file, copy the content of one file to another file, and more.
       This command is the most frequently used command in linux.
       To run this command, type cat followed by the file's name and its extension. For Example:- cat file.txt
       
       Other ways to use cat command:-
       - cat > filename creates a new file.
       - cat filename1 filename2>filename3 joins two files (1 and 2) and stores the output of them in a new file (3).
       - to convert a file to upper or lower case use, cat filename | tr a-z A-Z >output.txt
       
       
 ## 5. cp command:-
       This command is used copy files from your current directory to a different directory. 
       For example:- the command cp blackhole.jpg /home/username/Pictures would create a copy of blackhole.jpg (from your current directory) into the Pictures directory.
       

 ## 6. mv command:-
       The primary use of this command is to move files, although it can be used to rename files.
       For example:- mv neutronstar.txt /home/username/Universe
       To rename files, mv oldname.txt newname.txt
       
       
 ## 7. mkdir command:- 
       Is used to make a new directory. mkdir Music will create directory called Music.
       Other uses:- 
       - to create a directory inside an other directory: mkdir Music/newfile
       - use the p (parents) option to create a directory in between two existing directories. For example, mkdir -p Music/Charlie/Newfile will create the new “Charlie” file.
       
       
 ## 8. rmdir command:-
       This command is used to delete a directory. However rmdir only allows you to delete empty directories.
       Syntax: rmdir <directory name>    
       
 ## 9. rm command:-
       This command is used to delete directories and its contents within them. Use rm -r (as an alternative to rmdir) to delete a directory.
       Caution:- Always be sure which directory you are in as this command will delete everything and there is no going back.
 
 ## 10. touch command:-
        Used to create, change and modify timestamps of a file.
        
 ## 11. mv command:- 
        The mv command is used to move a file or a directory form one location to another location.
        Syntax: mv <filename><directory path>
        Example:- mv info.txt Directory
     
 ## 12. locate command:-
        This command locates a file. Using -i along with this command makes it case-insensitive, therefore you can search for a file even if you don't know its exact name.
        Use and asterik(*) to search for a file which contains two or more names. 
        For example:- locate -i maths*notes command will search for any file that contains the words "maths" and "notes".

 ## 13. find command:- 
        Similar to **locate** command, find also searches for files and directories. But it finds command within a given directory. 
        For example:- find /home/ -name notes.txt command will search for a file called notes.txt within the home directory and its sub-directories.
        To find files in current directory use, find. -name notes.txt and to look for directories use, / -type d -name notes. txt 
        
 ## 14. grep commmand:-
        This command lets you search through all the text in a given file. Basically it searches for words. 
        For example, grep math classnotes.txt will search for the word math in the file classnotes.

 ## 15. sudo command:- 
        sudo is a ahortform of "SuperUser Do". This command enables you to perform tasks that require administrative or root permissions.
        
 ## 16. df command:-
        Use this command to get a report on system's disc space usage, shown in percentage and KBs. To get the report in megabytes, type df -m
        
 ## 17. du command:- 
        Use this command to chech how much space does a file or a directory use. But this will show disk block numbers instead of usual size format.
        Add -h aargument to view in bytes,KBs and MBs. 
        
 ## 18. head command:-
        This command is used to view first lines of any file. By default it is 10 lines, although you can change it. type head -n 5 record.txt to show first 5 lines.
        
 ## 19. tail command:- 
        This command will display the last ten lines of a text file. For example, tail -n record.txt 
        
 ## 20. cal command:-
        Used to display the current month's calendar with the current date highlighted.
        
 ## 21. date command:- 
        Used to display date, time, time zone and more.
        
 ## 22. 
