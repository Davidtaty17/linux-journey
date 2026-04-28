# LEVEL 1->2 : Find the key for the next level

**Location**: Stored in a file named **-** on *home directory*
**Useful commands**: ls, cd, cat, file, find

## How to solve this level?
=> Log into game using ssh with **bandit1** as user

=> Use **ls** for listing the directory contents

=> Use **cat ./-** to print the content on the screen 

=> Log out with **CTRL + D** or **exit**

## Observations
- Why did I use **cat ./-** instead of **cat -** ? 
Because adding " ./ " before a **filename** tells the terminal to treat it as a *path to a file*, not as a special symbol.
- A **filename** is simply the name of a file.
