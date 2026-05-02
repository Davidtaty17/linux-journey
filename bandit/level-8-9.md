# LEVEL 8->9 : Find the key for the next level

**Location**:Stored in a file **data.txt** and is the only line of text that occurs only once

**Useful commands**: grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## How to solve this level?
=> Log into the game using ssh with **bandit8** as username and the password found in the previous level;  

=> Use **ls** to list directory content and find the file;

=> Once the file is located, use **sort data.txt | uniq -u** to search find our key;

=> Log out with **CTRL + D** or **exit**.

## Observations 
- Our key is located in a file which contents several lines of data and we must find our key in this data.
- Let me break this command down:
-> **sort**: helped me to group contents file together;
-> **|** or **a pipe**: had a main purpose to send the output of one command to directly into another one;
  Instead of running two separate commands, I wrote: **sort data.txt | uniq -u**;
->**uniq -u**: *uniq* just removes consecutive duplicates but still shows them once while the option *-u* filters the only one data that is not duplicated and print it on display.
-That was a great level. It shows the various commands used to navigate directories and files, and how they can simplify our tasks.
