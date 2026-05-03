# LEVEL 2->3 : Find the key for the next level

**Location**: Stored in a file named **--spaces in this filename** on *home directory*

**Useful commands**: ls, cd, cat, file, find

## How to solve this level?
=> Log into game using ssh with **bandit3** as user and use the password found in the  previous level.

=> Use **ls** to list the directory content and you will see the file.

=> Once the file is identified, use **cat "./--spaces in this filename--"** to print the content of our file on the screen.

=> Log out with **CTRL + D** or **exit**

## Observations
- **How do we read a file whose name contains spaces?** 
I found an issue when I was typing my command to read the file.
I used *cat ./--spaces in this filename--* and *cat ./ --spaces in this filename--* were not enough,
because the terminal did not recognize **--spaces in this filename--** as one single file.

->We must wrap the entire filename in **quotes**, so the terminal treats it as *one single argument* 



