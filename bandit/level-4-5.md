# LEVEL 4->5 : Find the key for the next level 

**Location**: Stored in the only **human-readable file** in a directory named *inhere*
**Useful commands**: ls, cd, cat, file, du, find

## How to solve this level?
=> Log into the game using ssh with **bandit4** as username and the password found in the previous level;

=> Use **ls** to list directory contents and find our directory;

=> Once the directory is located, use **cd inhere** to change the current directory;

=> Then, type **ls** to list the directory's content;

=> You will see several files. This time, use the command **file ./*** to know the *type of all files in this directory*;

=> Then once the file is located, type **cat ./filename** to read the content on the screen;

=> Log out with **CTRL + D** or **exit** on the terminal.


## Observations

-  **Human-readable file** contains plain text that can be read directly by a human.
In Linux, the file command identifies the type of each file. **Human-readable files** appear as *ASCII text*, while **non-readable files** appear as *data*.

- ***** is a **Wildcard** that matches *all files* in a directory. Using **file./*** runs the file command on every file at once instead of typing each filename individually.
