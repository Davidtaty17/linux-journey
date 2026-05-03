# LEVEL 5->6 : Find the key for the next level

**Location**:Stored in a file somewhere under the inhere directory and all of the following properties:human-readable, 1033 bytes in size & not executable.

**Useful commands**: ls, cd, cat, file, du, find


## How to solve this level ?

=> Log into the game using ssh with **bandit5** as username and the password found in the previous level;  

=> Use **ls** for listing directory contents and find the directory;

=> Once the directory is located, use **cd inhere** to change the current directory;

=> Then, type **ls** to see the content of this directory;

=> Once typed you will see several directories. This time, use the command **find ./ -size 1033c** to know in which directory our file is;

=> Then, navigate to that directory and open the file with **cat ./filename**;

=> Log out with **CTRL + D** or **exit**.

## Observations 
- You will notice that our file is a hidden file because there is a *dot* at the beginning of the filename.
- The **-size** flag filters files by their size. The *suffix* *c* specifies **bytes**.
- **./** has been used specifically for the current directory
