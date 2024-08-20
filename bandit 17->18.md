#Bandit level 17->18
##Objective: There are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new
##Steps taken
1. Connecting to the server
   Command: ssh bandit17@bandit.labs.overthewire.org -p2220
   loged in using the password from previous level 
2. Finding the file 
   command: ls
3. retriving password
   command: diff password.new passwords.old
   retrived the password for the next level .
