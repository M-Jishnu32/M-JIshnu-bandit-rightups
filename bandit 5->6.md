#Bandit level 5->6
##Objective: Find the password for the next level in a file located somewhere in inhere directory
##Steps taken
1. Connecting to the server
   Command: ssh bandit3@bandit.labs.overthewire.org -p2220
   loged in using the password from level 5
2. entering the inhere directory
   command: cd inhere
3. enetering maybehere07 directory
   command cd maybehere07
4. Finding the file 
   command: ls find -type f -size 1033c -readable ! -executable
5. opening the file
   command: cat .file2
   using the command opened the fie and found the password for the next level
