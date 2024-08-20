#Bandit level 10->11
##Objective: Find the password for the next level in data.txt which contain base64 coded data
##Steps taken
1. Connecting to the server
   Command: ssh bandit10@bandit.labs.overthewire.org -p2220
   loged in using the password from previous level
2. Finding the file 
   command: ls
3. opening the file
   command: cat data.txt| base64 -d
   using the command opened the fie and found the password for the next level
