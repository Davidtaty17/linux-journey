# LEVEL 6->7 : Find the key for the next level

**Location**: stored somewhere on **the server** and has all of the following properties:

owned by user bandit7

owned by group bandit6

33 bytes in size

**Useful commands**: ls , cd , cat , file , du , find , grep

## How to solve this level ?
=> Log into the game using ssh with **bandit6** as username and the password found in the previous level;  

=> Follow the instruction as described. At this time, the final command is **find / -user bandit7 -group bandit6 -size 33c**;

=> Once our file is found, print the content on screen with **cat /path/to/the/file**;

=> Log out with **CTRL + D** or **exit**.

## Observations 
- **Find**: helps us to simply find a file in a directory or a server.
- **./**: is for the current directory and here we used **/**, that was for **the root of the entire server**.
- We used find with the **root path** */* and several flags: -user, -group, and -size.
- When I ran the final command, the terminal printed many errors *"Permission denied"*. It was normal because **bandit6** does not have permission
  to access folders belonging to other users or system. The **find** command continued searching until it found the correct file.
