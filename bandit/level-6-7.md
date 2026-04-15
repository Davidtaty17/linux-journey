# LEVEL 6->7 : Find the key for the next level

**Location**: stored somewhere on **the server** and has all of the following properties:
owned by user bandit7
owned by group bandit6
33 bytes in size

**Commands for this level**: ls , cd , cat , file , du , find , grep

## How to solve this level ?
=> Log into the game using ssh with **bandit6** as username and the password found in the previous level;  
=> We will follow the instruction as they have said. At this time, our command would be **find / -user bandit7 -group bandit6 -size 33c** 
=>Once our file found, we will print the content on the display with **cat [the root where our key is located]**
=> Log out with **CTRL + D** or **exit**.

## Observations 
- **Find**: helps us to simply find a file in a directory or a server
- **./**: is for the current directory and there we have used **/**, that was for the root of the entire **server**
- We accompanied *find* not only with the server but also arguments and options for this case. We have; *-user*, *-group* and *-size*
- When I ran **find /**, the terminal printed many "Permision denied" erros. It was noraml beacuse **bandit6** does not have permission to access folders belonging to other users or system. The **find** command continued searching until it found the correct file
