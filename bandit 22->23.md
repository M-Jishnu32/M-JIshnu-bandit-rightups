Bandit level 22->23
##Objective: Find the password a program is running automatically at regular intervals from cron, the time-based job scheduler
##Steps taken
1. Connecting to the server
   Command: ssh bandit22@bandit.labs.overthewire.org -p2220
   logged in using password from previous level
3. finding the file
   command: cd /etc/cron.d/
   command: ls
4. opening the file 
   command: cat cronjob_bandit23
   command: cat /usr/bin/cronjob_bandit23.sh
6. retrieving the password
   command: (echo I am user bandit23 | md5sum | cut -d ' ' -f 1)
   retrived the password for next level
