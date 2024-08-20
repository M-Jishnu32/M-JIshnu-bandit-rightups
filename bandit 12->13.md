#Bandit level 12->13
##Objective: Find the password for the next level in data.txt which is a hexdump of a file that has been repeatedly compressed
##Steps taken
1. Connecting to the server
   Command: ssh bandit12@bandit.labs.overthewire.org -p2220
   loged in using the password from previous level
2. Finding the file 
   command: ls
3. creating a new directory 'dirt' under /tmp directory
   command: mkdit dirt
4. copying file data.txt to dirt directory
   command: cp data.txt /tmp/dirt
5. uncompressing the file data.txt to get the password
   command: xxd -r data.txt data2.txt
   command: mv data1.txt data2.bin.gz
   command: gunzip data2.bin.zip
   command: mv data1.bin.gz data2.binbz2
   command: bunzip2 data2.bin.bz2
   command: mv data2.bin data4.bin.gz
   command: gunzip data4.bin.gz
7. using tar command to furthur decompress
   command: mv data4.bin.gz data5.bim.tar
   command: tar -xf data5.bin.tar
   command: mv data5.bin data5.bin.tar
   command: tar -xf data5.bin.tar
   command: mv data6.bin data7.bin.bz2
   command: bunzip2 data7.bin.bz2
   command: mv data8.bin data9.bin.gz
   command: gunzip data9.bin.gz => data9.bin ASCII text
7. opening the file data9.bin
   command: cat data9.bin
   using the command opened the fie and found the password for the next level
