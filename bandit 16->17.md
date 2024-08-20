#Bandit level 16->17
##Objective: The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL/TLS and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.
##Steps taken
1. Connecting to the server
   Command: ssh bandit16@bandit.labs.overthewire.org -p2220
   logged in using password from previous level
3. listing out the localhost
   command: nmap -p 31000-32000 localhost
   we get 5 potential local host
5. listing out the required localhost
  command: nmap -p 31046,31518,31691,31790,31960 -A localhost
  localhost 31790 is the required localhost
6. Connecting to localhost
   command: ncat --ssl localhost 31790
8. enter the password for the current level and we get the credentials for the next level .
