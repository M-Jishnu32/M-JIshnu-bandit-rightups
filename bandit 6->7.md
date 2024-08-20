#Bandit level 6->7
##Objective: Find the password for the next level in a file located somewhere in inhere directory
##Steps taken
1. Connecting to the server
   Command: ssh bandit6@bandit.labs.overthewire.org -p2220
   loged in using the password from previous level
2. Finding the file 
   command: find/ -size 33c -group bandit6 -user bandit7
3. opening the file
   command: cat ./var/lib/dpkg/info/bandit7.password
   using the command opened the fie and found the password for the next level
