# LEVEL 5->6 : Find the key for the next level

**Location**:Stored in a file somewhere under the inhere directory and all of the following properties:human-readable, 1033 bytes in size & not executable.
**Commands for this level**: ls, cd, cat, file, du, find


## How to solve this level ?

=> Log into the game using ssh with **bandit5** as username and the password found in the previous level.
=> Use **ls** for listing directory contents and find the directory 
=> Once the directory located, we will use **cd inhere** to change the current directory 
=> Then, we will type **ls** to see the content of this directory 
=> Once typed you will see several directories. This time we will use the command **find  +  ./  +   -size 1033c** to know in which directory our file is.
=> We will notice that our file was an hidden file because there is a dot **.** at the beginning of the filename.
=> Then, we will navigate to that directory and open the file with **cat ./[file's name].**
=> Log out with **CTRL + D** or **exit**.

## Observations 
- **find -size** helps us to find a size of a file. We added **c** means bytes specifically.
