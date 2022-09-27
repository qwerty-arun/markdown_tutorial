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
       
