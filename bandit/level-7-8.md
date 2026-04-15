# LEVEL 7->8 : Find the key for the next level

**Location**:Stored in a file **data.txt**  next to the word millionth

**Commands for this level**: man, grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd


## How to solve this level ?


=> Log into the game using ssh with **bandit7** as username and the password found in the previous level;  
=> Use **ls** for listing directory contents and find the file;
=> Once the directory located, we will use **grep millionth data.txt** to search every line in data.txt and show us only the lines that contain the word millionth;

=> Log out with **CTRL + D** or **exit**.

## Observations 
- First, I have used the command **man grep** to understand how it works. At first, I was quite lost, did more research and used Claude to explain to me, really how to use **grep**
- Second, **grep** principally searches through  file line by line and displays only the lines containing the word you are looking for ( e.g. **grep [search word] [file's name]**
- the **man command** is the manual page, it is a system reference manual for every commands
