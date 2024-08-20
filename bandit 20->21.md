#Bandit level 20->21
##Objective:There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level. If the password is correct, it will transmit the password for the next level.
##Steps taken
1. Connecting to the server
   Command: ssh bandit20@bandit.labs.overthewire.org -p2220
   logged in using password from previous level
2. finding the file
   command: ls 
   we see the file bandit20-do
4. listing the bandit20-do
   command: ls -l bandit20-do
5. retrieving the password
   command: ./bandit20-do cat /etc/bandit_pass/bandit20
   retrived the password for next level
