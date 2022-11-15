|Linux Commands|What does it do? |
|:-------:|:-------|
|pwd|This command is used to find out the path of the current directory(folder).This command will return an absolute path, which is a path of all directories that starts with a forward slash(/).An example of an absolute path is:-  /home/username .|
|cd|This command is used to navigate through linux files and directories.  It either requires a full path or name of the directory depending on the current directory you are in. Let’s say you’re in /home/username/Documents and you want to go to Photos, a subdirectory of Documents. To do so, simply type the following command: cd Photos. Now if you want to switch to a completely new directory, say /home/username/Books.In this case, you have to type cd followed by the directory’s absolute path: cd /home/username/Books.<br>Some shortcuts:- <ul><li> cd.. (with two dots) to move one directory up.</li><li>cd to go straight to the home folder.</li><li>cd- (with hypen) to move to your previous directory.</li></ul>NOTE:- You have to type the directories' names exactly as it is becouse Linux's shell is case sensitive.|
|ls|This command is used to list contents os a directory. By default, this will display content of your current working directory. If you want to view contents of other directories, type ls and then the directory's path.<br>For example:- /homes/username/Movies to view contents of Movies.<br> Variations in this command:--<ul><li>ls -R will list all the files in teh sub-directories as well.</li><li>ls -a will show all the hidden files.</li><li>ls al will list the files and directories with detailed information like owner, size etc.</li><li>`ll and ls al are almost the same, but what's the difference?`</li></ul>|
|cat|The cat command is a multi-purpose utility in the Linux system. It can be used to create a file, display content of the file, copy the content of one file to another file, and more.This command is the most frequently used command in linux.To run this command, type cat followed by the file's name and its extension. For Example:- cat file.txt<br>Other ways to use cat command:-<ul><li>cat > filename creates a new file.</li><li>cat filename1 filename2>filename3 joins two files (1 and 2) and stores the output of them in a new file (3).</li><li>to convert a file to upper or lower case use, cat filename tr a-z A-Z >output.txt</li></ul>|
|cp|This command is used copy files from your current directory to a different directory. For example:- the command cp blackhole.jpg /home/username/Pictures would create a copy of blackhole.jpg (from your current directory) into the Pictures directory.|
|mv|The primary use of this command is to move files, although it can be used to rename files.For example:- mv neutronstar.txt /home/username/Universe. To rename files, mv oldname.txt newname.txt|
|mkdir|Is used to make a new directory. mkdir Music will create directory called Music.<br>Other uses:-<ul><li>to create a directory inside an other directory: mkdir Music/newfile-</li><li> to create multiple folders type mkdir abc def</li><li> You can create nested folders by adding the -p option. Refer to screenshot no. 163 to know it better.</li></ul>|
|rmdir|This command is used to delete a directory. However rmdir only allows you to delete empty directories.Syntax: rmdir <directory name>| 
|rm|This command is used to delete a file and its contents within them. Caution:- Always be sure which directory you are in as this command will delete everything and there is no going back.<ul><li>rm <filename> to delete a file</li><li>rm file1 file2 file3.. to delete multiple files at once.</li><li>`rm* to delete all files` (Be very careful with this)</li><li>rm -r directory_name to delete a non-empty directory.</li><li>rm -r directory's name to delete a empty directory.</li><li>Usually we have to type ls and check whether the file/directory is deleted or not, so to avoid that use rm -v <file></li><li>rm -ri will ask you to check the directory once and its contents before you delete them.</li></ul> |
|touch|Used to create, change and modify timestamps of a file. If a file already exists and then you type touch abc.txt, it will update the timestamp of the file.|
|locate|This command locates a file. Using -i along with this command makes it case-insensitive, therefore you can search for a file even if you don't know its exact name.Use an asterik(*) to search for a file which contains two or more names. For example:- locate -i maths*notes command will search for any file that contains the words "maths" and "notes".|
|find|Similar to **locate** command, find also searches for files and directories. But it finds command within a given directory. For example:- find /home/ -name notes.txt command will search for a file called notes.txt within the home directory and its sub-directories.To find files in current directory use, find. -name notes.txt and to look for directories use, / -type d -name notes. txt |
|grep|This command lets you search through all the text in a given file. Basically it searches for words. For example, grep math classnotes.txt will search for the word math in the file classnotes.|
|df|Use this command to get a report on system's disc space usage, shown in percentage and KBs. To get the report in megabytes, type df -m|
|du|Use this command to chech how much space does a file or a directory use. But this will show disk block numbers instead of usual size format.Add -h aargument to view in bytes,KBs and MBs.|
|sudo|sudo is a ahortform of "SuperUser Do". This command enables you to perform tasks that require administrative or root permissions.|
|head|This command is used to view first lines of any file. By default it is 10 lines, although you can change it. type head -n 5 record.txt to show first 5 lines.|
|tail|This command will display the last ten lines of a text file. For example, tail -n record.txt|
|cal|Used to display the current month's calendar with the current date highlighted.|
|date|Used to display date, time, time zone and more.|
|man|This command shows instructions about other commands.For example, man tail will show the manual instruction for tail command.|
|diff|This command compares contents of two files line by line. After analyzing the files, it will output the lines which do not match.Programmers often use this command when they need to make program alterations instead of rewriting the entire source code. Simplest form of this command:- diff file1.txt file2.txt|
|history| Displays the command you had entered before on that day.|
|useradd|Since Linux is a multi-user system, this means more than one person can interact with the same system at the same time. useradd is used to create a new user, while passwd is adding a password to that user’s account. To add a new person named John type, useradd John and then to add his password type, passwd 123456789.|
|userdel| Similarly to delete the users accout type, userdel username.|
|wget|You can download files from the internet using this command. To do so, simply type wget followed by download link.|
|rename|Used to rename files. Syntax:- rename 's/old-name/new-name/' files  Example:- 's/\.txt$/\.pdf/' *.txt|
|tac|It is the reverse of cat command. It displays the file content in reverse order(from last line).Syntax:- tac <file name> |
|su| This command provides administrative access to another user. Basically, it allows access of the Linux Shell to another user.Syntax:- su <user name>|
|passwd|Used to create and change password for a user. Syntax:- passwd <username> |
|groupadd|Used to create a user group. Syntax:- groupadd <group name> |
|wc| Used to count the lines, words and characters in a file.|
|sort|Used to sort contents of a file in an alphabetical order. Syntax:- sort <filename>|
|sleep|Used to hold the terminal by the specified amount of time. By default, it takes time in seconds.Syntax :- sleep <time> |
|exit|Used to exit from the current shell. Type exit and hit enter.|
|clear|Used to clear the terminal screen. Type clear and hit enter.|
|mail|Is used to send emails from the command line.Syntax: mail -s "Subject" <recipient address>  For example:- mail -s "Hey there!" xyz123@gmail.com|
|zcat|Used to display the compressed files. Syntax:- zcat <filename>|
|mount| Used to connect an external device file system to the system's file system.Syntax:mount -t type <device> <directory>|
|ip|Used to assign an IP address, initialze an interface, disable an interface.|
|ssh|Used to create a remote connection through the ssh protocol.Syntax:  ssh user_name@host(IP/Domain_name)</p>|
|ping|Short form for "Packet Internet Groper" . Used to check connectivity between two nodes (whether the server is connected. Syntax:- ping <destination>.|
|host|Used to display the IP address for a given domain name and vice versa.  It performs the DNS lookups for the DNS Query.Syntax:host <domain name> or <ip address>|
|gzip| Used to truncate the file size. It is a compressing tool. It replaces the original file by the compressed file having '.gz' extension.Syntax: gzip <file1> <file2> <file3>...  For example:- gzip file.txt file1.txt |
|gunzip|Used to decompress a file. It is reverse of gzip command.Syntax: gunzip <file1> <file2> <file3>. . |
|od|Used to display the content of a file in different format, such as hexadecimal, octal, and ASCII characters.<br>Syntax:<ul><li>od -b <fileName>      // Octal format</li><li> od -t x1 <fileName>   // Hexa decimal format</li><li> od -c <fileName>     // ASCII character format</li></ul>|
|tr|Used to translate file content. For example:- Convert lowercase to uppercase, braces to paranthesis etc. Syntax:- command | tr <'old'> <'new'>|
|sed| The sed command is also known as stream editor. It is used to edit files using a regular expression. It does not permanently edit files; instead, the edited content remains only on display. It does not affect the actual file.Syntax:  command | sed 's/<oldWord>/<newWord>/' |
|more| The more command is quite similar to the cat command, as it is used to display the file content in the same way that the cat command does. The only difference between both commands is that, in case of larger files, the more command displays screenful output at a time.Syntax: more <file name>|
|less|The less command is similar to the more command. It also includes some extra features such as 'adjustment in width and height of the terminal.Comparatively, the more command cuts the output in the width of the terminal.Syntax: less <file name>|

  
# What is a Path?
  A path is a unique location to a file or a folder in a file system of an OS. A path to a file is a combination of / and alphanumeric characters. 
  
## What is an Absolute Path?
  An absolute path is defined as the specifying the location of a file or a directory from the root directory(/). In other words, we can say that absolute path is a complete path from start of actual file system.
### Examples:- 

 /etc/samba.smb.conf

  /boot/grub/grub.conf

  `If you see all these paths started from "/" directory which is a root directory for every Linux/Unix machines.`
  
  
# What is a Relative Path? 
  Relative path is defined as a path related to the present working directory. 
  
  Suppose I am located in /var/log and I want to change directory to /var/log/kernel. I can use relative path concept to change directory to kernel.
  
  Changing directory to /var/log/kernel by using relative path concept:- 
   
  pwd/var/logcd kernel

  `Note: If you observe there is no "/" before kernel which indicates it’s a relative directory to present working directory.`

Changing directory to /var/log/kernel using absolute path concept:- 
  
  cd /var/log/kernel

  `Note: We can use an absolute path from any location where as if you want to use relative path we should be present in a directory where we are going to specify relative to that present working directory.`
