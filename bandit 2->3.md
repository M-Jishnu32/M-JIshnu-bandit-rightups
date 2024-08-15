#Bandit level 2->3
##Objective: Find the password for the next level in a file 'spaces in this filename' located in the home directory
##Steps taken
1. Connecting to the server
   Command: ssh bandit2@bandit.labs.overthewire.org -p2220
   loged in using the password from level 2
2. Finding the file 'spaces in this filename'
   command: ls
3.opening the file 'spaces in this filename'
   command: cat "spaces in this filename"
   using the command opened the fie and found the password for the next level
