## **Important bash commands with a brief description and example**

1. df: (basic shell)

  Shows the available disk space in each of the disk partitions on the system. 'df -m' to see space in megabytes.
  ```shell
  $ df
  $ df -m
  ```
2. ls: (directories)

  Use this command to know what files exist in the directory you are currently in. 'ls -a' to see the hidden files as well.
  
  ```shell
  $ ls
  $ ls -a
  ```
3. cd: (directories)

  Use 'cd' command to go to any directory. For example, to go to the Downloads folder, 'cd Downloads'. Case sensitive command. 
  
  ```shell
  $ cd  --> to go to home directory
  $ cd Downloads --> go to downloads
  $ cd ..  --> go to previous folder
  ```
4. mkdir: (directories)

  Command to create a new directory/folder within the current directory. To create a directory name with spaces use '\' (backslash) instead of giving a space.
  
  ```shell
  $ mkdir Example\Directory
  ```
5. rm: (file operations)

  Command to delete files or directories. 'rm -r' to delete only the directory and not the files in that directory.
  
  ```shell
  $ rm -r Example\Directory
  $ rm script.py
  ```
6. touch: (file operations)

  The touch command is used to create a new file. It can be any type of file, like a text file or a python script.
  
  ```shell
  $ touch newfile.txt
  ```
7. man: (basic shell)

  To know more about a certain command and how to use it, we use the man command. It shows the documentation of that command. 
  
  ```shell
  $ man cd --> shows documentation of cd command
  ```
8. cp: (file operations)

  The command for copying files through the command line. Takes two arguments, first is the path of the file to be copied, and the second is where that file should be copied to.
  
  ```shell
  $ cp setup.exe /Downloads
  ```
9. mv: (file operations)

  We can use 'mv' to move files throught the command line, or to rename a file. Takes two arguments just like the 'cp' command.
 
 ```shell
 $ mv newfile.txt new.txt --> renames newfile.txt to new.txt
 $ mv new.txt /Desktop --> moves new.txt to the desktop
 ```
10. locate: (searching and sorting)

  Use this command to find where exactly a file is located. Useful when we dont know or remember where a file is saved. Use the '-i' argument to ignore case. Use an asterisk to separate words if there is more than one word.
  
  ```shell
  $ locate -i script.py
  $ locate -i new*doc.txt
  ```
11. echo: (shell scripting)
 
  The echo command helps us move data (usually text) into a file. 
  
  ```shell
  $ echo Hello World >> new.txt 
  ```
12. cat: (file examination)
 
  The cat command is used to display the contents of any file, for example scripts or text files.
  
  ```shell:
  $ cat script.py --> displays the python code
  ```
13. nano, vi: (Text editors)
 
  Nano and vi are built in text editors in the Unix terminal . The nano command is a good text editor that denotes keywords with color and can recognize most languages. And vi is simpler than nano. We can create a new file or modify existing files using nano.
  
  ```shell
  $ nano newtext.txt --> creates a new .txt file and opens the editor for us to make any necessary changes
  ```
14. sudo: (users and groups)
 
  Stand for 'SuperUser Do'. This command is used when we need to run any command with admin or root privileges. If we need root permissions to modify a file, we can run the following command
  
  ```shell
  $ sudo nano config.txt
  ```
15. du: (file examination)
 
  Similar to the df command, but 'du' shows disk usage of a particular file or folder in the system.
  
  ```shell
  $ du Downloads
  ```
16. zip, unzip: (compression)
 
  Use zip to compress files into a zip archive, and unzip to extract files from a zip archive.
 
17. ping: (network)
 
  Use 'ping' to check your connection to a server.
  
  ```shell:
  $ ping google.com
  ```
18. hostname: (multi-user environments)
 
  This command displays the name of the host machine, to view the host IP address instead we add the argument '-I'.
  
  ```shell:
  $ hostname -I
  ```
19. chmod: (file permissions)
 
  'chmod' is used to make a file executable and to change the permissions granted to it in Linux. Imagine you have a python code named numbers.py in your computer. You'll need to run “python numbers.py” every time you need to run it. Instead of that, when you make it executable, you'll just need to run “numbers.py” 
  
  ```shell
  $ chmod +x numbers.py
  ```
20. apt-get: (packages)
 
  'apt' is used when working with packages through the command line. 'apt-get' is used to install packages. We add the 'sudo' command when we require admin privileges to install a package.
  
  ```shell
  $ sudo apt-get install jed --> jed is another linux command line text editor
  ```
21. head, tail: (file examination)
 
  Output the beginning or the ending of a file.
  
  ```shell
  $ head data.csv
  $ tail data.csv
  ```
22. wc: (file examination)
 
  Output a count of the number of characters, lines, words, etc. in a file.
  
  ```shell
  $ wc -l --> displays number of lines in a file
  $ wc -w --> displays number of words in a file
  $ wc -c --> displays the count of bytes in a file
  $ wc -m --> displays the count of characters in a file
  $ wc -L --> prints the length of the longest line in a file
  ```
23. grep: (searching and sorting)
 
  The grep filter searches a file for a particular pattern of characters, and displays all lines that contain that pattern.
  
  ```shell
  $ grep 'word' file --> searches file for the expression 'word'
  $ grep -l 'word' file1 file2 file3 --> displays list of filenames that contain 'word'
  $ grep -i 'word' file --> case insensitive search
  $ grep -w 'word' file1 --> match whole expression
  ```
24. sort: (searching and sorting)
 
  Command line function for sorting lines of text files. It supports sorting alphabetically, in reverse order, by number, by month and can also remove duplicates.
  
  ```shell
  $ sort input.txt
  $ sort -r input.txt --> sort in reverse order
  $ sort -n inputnumbers.txt --> sort file numerically
  $ sort -nr inputnumbers.txt --> sort file numerically in reverse order
  $ sort -c input.txt --> checks if file is already sprted or not
  $ sort -u input.txt --> sorts and removes duplicates
  ```
25. time: (system information)
 
  Displays execution time of the command being run.
  
  ```shell
  $ time script.py
  ```
26. ps: (process management)
  
  Displays the currently running processes. Shows the PID (process id), TTY (name of console user is logged into), the CPU time the process has been running and the name of the command that launched the process.
  
  ```shell
  $ ps
  $ ps -e --> list all processes on the system
  ```
27. top: (process management) 

  This command displays processor activity of your Linux box and also displays tasks managed by kernel in real-time. It’ll show how processor and memory are being used and other information like running processes.
  
28. &: (process management)
  
  A special character. When '&' is places at the end of a command, that command is run in the background. i.e. Shell does not wait for the command to finish executing before returning to the input prompt.

29. if..else: (shell scripting) 

  If-else conditional statement in shell scripts.
  
  ```shell
  a=10
  b=20

  if [ $a == $b ]
  then
   echo "a is equal to b"
  else
   echo "a is not equal to b"
  fi
  ```
30. for, while: (shell scripting)
