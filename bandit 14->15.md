#Bandit level 14->15
##Objective: Find The password for the next level password can be retrieved by submitting the password of the current level to port 30000 on localhost.
##Steps taken
1. Connecting to the server
   Command: ssh bandit14@bandit.labs.overthewire.org -p2220
2. connectinf to localhost 30000
   command: nc localhost 30000
3. enter the password for the current level and we get the password for the next level.
