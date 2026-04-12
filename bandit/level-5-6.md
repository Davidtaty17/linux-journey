LEVEL 5->6 : Find the key for the next level 

Location:Stored in a file somewhere under the inhere directory and all of the following properties:human-readable, 1033 bytes in size & not executable.
Commands for this level: ls, cd, cat, file, du, find


How to solve this level ?
=> Log into the game using ssh with < bandit5 > as username and the password found in the previous level.
=> Use < ls > for listing directory contents and find the directory 
=> Once the directory located, we will use < cd inhere > to changing the current directory 
=> Then, we will type < ls > to see is in this directory 
=> Once taped you will see several directories. In this time we will use the command < find > + < ./ > + < -size 1033 > to know in which directory our file is.
=> Then, we will go these directory and open the file with < cat ./[file's name] >
=> Log out with < CTRL + D > or type < exit > on the terminal 


Observations
