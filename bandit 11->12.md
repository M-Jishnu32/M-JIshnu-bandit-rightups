#Bandit level 11->12
##Objective: Find the password for the next level in data.txt which where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions
##Steps taken
1. Connecting to the server
   Command: ssh bandit11@bandit.labs.overthewire.org -p2220
   loged in using the password from level 10
2. Finding the file 
   command: ls
3. opening the file
   command: cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
   using the command opened the fie and found the password for the next level
