#Bandit level 7->8
##Objective: Find the password for the next level in data.txt next to the word millionth
##Steps taken
1. Connecting to the server
   Command: ssh bandit7@bandit.labs.overthewire.org -p2220
   loged in using the password from level 7
2. Finding the file 
   command: ls
3. opening the file
   command: grep "millionth" data.txt
   using the command opened the fie and found the password for the next level
