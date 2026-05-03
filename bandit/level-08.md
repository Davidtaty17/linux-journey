# LEVEL 7->8 : Find the key for the next level

**Location**:Stored in a file **data.txt**  next to the word millionth

**Useful commands**: man, grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd


## How to solve this level ?


=> Log into the game using ssh with **bandit7** as username and the password found in the previous level;  

=> Use **ls** to list directory content and find the file;

=> Once the file is located, use **grep millionth data.txt** to search every line in data.txt and show only the lines that contain the word millionth;

=> Log out with **CTRL + D** or **exit**.

## Observations 
- I used the command **man grep** to understand how it works. I was quite lost, did more research and used Claude to explain to me how to use grep
- **grep** searches through a file line by line and displays only the lines containing the word you are looking for ( e.g. **grep [search word] [filename]**
grep is also a fundamental *security tool*. It lets you search through *log files* when something happens on a Linux system. For example, a login, an error, a service starting. All those records *are written in log files*
