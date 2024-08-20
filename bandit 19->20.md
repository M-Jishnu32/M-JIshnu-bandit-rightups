#Bandit level 19->20
##Objective:To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary
##Steps taken
1. Connecting to the server
   Command: ssh bandit19@bandit.labs.overthewire.org -p2220
   logged in using password from previous level
2. finding the file
   command: ls 
   we see the file bandit20-do
4. listing the bandit20-do
   command: ls -l bandit20-do
5. retrieving the password
   command: ./bandit20-do cat /etc/bandit_pass/bandit20
   retrived the password for next level
