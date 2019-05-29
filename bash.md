**Important bash commands with a brief description and example**

1. df:
  Shows the available disk space in each of the disk partitions on the system. 'df -m' to see space in megabytes.
  ```shell
  $ df
  $ df -m
  ```
2. ls:
  Use this command to know what files exist in the directory you are currently in. 'ls -a' to see the hidden files as well.
  
  ```shell
  $ ls
  $ ls -a
  ```
3. cd:
  Use 'cd' command to go to any directory. For example, to go to the Downloads folder, 'cd Downloads'. Case sensitive command. 
  
  ```shell
  $ cd  --> to go to home directory
  $ cd Downloads --> go to downloads
  $ cd ..  --> go to previoud folder
  ```
4. mkdir:
  Command to create a new directory/folder within the current directory. To create a directory name with spaces use '\' (backslash) instead of giving a space.
  
  ```shell
  $ mkdir Example\Directory
  ```
5. rm:
  Command to delete files or directories. 'rm -r' to delete only the directory and not the files in that directory.
  
  ```shell
  $ rm -r Example\Directory
  $ rm script.py
  ```
6. touch:
  The touch command is used to create a new file. It can be any type of file, like a text file or a python script.
  
  ```shell
  $ touch newfile.txt
  ```
7. man:
  To know more about a certain command and how to use it, we use the man command. It shows the documentation of that command. 
  
  ```shell
  $ man cd --> shows documentation of cd command
  ```
8. cp:
  The command for copying files through the command line. Takes two arguments, first is the path of the file to be copied, and the second is where that file should be copied to.
  
  ```shell
  $ cp setup.exe /Downloads
  ```
9. mv:
  We can use 'mv' to move files throught the command line, or to rename a file. Takes two arguments just like the 'cp' command.
 
 ```shell
 $ mv newfile.txt new.txt --> renames newfile.txt to new.txt
 $ mv new.txt /Desktop --> moves new.txt to the desktop
 ```
10. locate:
  Use this command to find where exactly a file is located. Useful when we dont know or remember where a file is saved. Use the '-i' argument to ignore case. Use an asterisk to separate words if there is more than one word.
  
  ```shell
  $ locate -i script.py
  $ locate -i new*doc.txt
  ```
 11. echo: 
  The echo command helps us move data (usually text) into a file. 
  
  ```shell
  $ echo Hello World >> new.txt 
  ```
 12. cat:
  The cat command is used to display the contents of any file, for example scripts or text files.
  
  ```shell:
  $ cat script.py --> displays the python code
  ```
 13. 
