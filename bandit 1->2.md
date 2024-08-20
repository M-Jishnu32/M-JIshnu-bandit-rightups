#Bandit level 1->2
##Objective: Find the password for the next level in a file '-' located in the home directory
##Steps taken
1. Connecting to the server
   Command: ssh bandit2@bandit.labs.overthewire.org -p2220
   loged in using the password from previous level
2. Finding the file '-'
   command: ls
3.opening the file '-'
   command: cat ./-
   using the command opened the fie and found the password for the next level
