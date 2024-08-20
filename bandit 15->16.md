#Bandit level 15->16
##Objective: Find The password for the next level by submitting the password of the current level to port 30001 on localhost using SSL/TLS encryption.
##Steps taken
1. Connecting to the server
   Command: ssh bandit15@bandit.labs.overthewire.org -p2220
   logged in using password from previous level
2. connecting to localhost 30001
   command: openssl s_client -connect localhost:30001
3. enter the password for the current level and we get the password for the next level .
