LEVEL 4->5 : Find the key for the next level 

Location:<inhere directory> / Stored in the only human-readable file

Commands for this level: ls, cd, cat, file, du, find


How to solve this level ?

=> Log into the game using ssh with < bandit4 > as username and the password found in the previous level.

=> Use < ls > for listing directory contents and find the directory 

=> Once the directory located, we will use < cd inhere > to changing the current directory 

=> Then, we will type < ls > to see our file on the list 

=> Once taped you will see several files. In this time we will use the command < file > + < ./* > for know the type of all files in this directory at once.

=> Then once the file is located, we type < cat ./[file's name] > fo printing the content on the screen.

=> Log out with < CTRL + D > or type < exit > on the terminal 


Observations

-  Human-readable file contains plain text that can be read directly by a human.
In Linux, the file command identifies the type of each file. Human-readable files appear as ASCII text, while non-readable files appear as data.

- < * > is a wildcard that matches all files in a directory. Using file < ./* > runs the file command on every file at once instead of typing each filename individually.
