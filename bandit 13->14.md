#Bandit level 13->14
##Objective: Find The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level we get a private SSH key that can be used to log into the next level instead of password.
##Steps taken
1. Connecting to the server
   Command: ssh bandit13@bandit.labs.overthewire.org -p2220
   loged in using the password from level 12
2. Finding the file 
   command: ls
3. opening the file
   command: cat sshkay.private
   using the command opened the fie and find the private ssh key
4. copying the content of file to local host
   command: cat 'content of ssh key' > private14.keys
5. changing the mode of private14.keys
   command: chmod 700 private14.keys
6. loggin to bandit14
   command: ssh bandit14@bandit.labs.overthewire.org -p2220 -i private14.keys
   logged in retrived the password for the next level .
