Bandit level 21->22
##Objective: Find the password in a program running automatically at regular intervals from cron, the time-based job scheduler.
##Steps taken
1. Connecting to the server
   Command: ssh bandit21@bandit.labs.overthewire.org -p2220
   logged in using password from previous level
2. finding the file
   command: cd /etc/cron.d/
   command: ls
4. opening the file 
   command: cat cronjob_bandit22
   command: cat /usr/bin/cronjob_bandit22.sh
6. retrieving the password
   command: cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
   retrived the password for next level
