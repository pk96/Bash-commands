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
  $ rm Example\Directory
  $ rm script.py
  
