LEVEL 3->4 : Find the key for the next level 

Location:<inhere directory> / Stored in a hidden file
Commands for this level: ls, cd, cat, file, find


How to solve this level ?
=> Log into the game using ssh with < bandit3 > as username and the password found in the previous level.
=> Use < ls > for listing directory contents and find the directory 
=> Once the directory located, we will use < cd inhere > to change the current directory 
=> Then, we will type < ls -a > to see our file on the list 
=> Once the hidden file is located, we will use the command < cat ./...Hiding-From-You > for printing the content on the screen.
=> Log out with < CTRL + D > or type < exit > on the terminal 


Observations
- In this level, you should make sure that you are written correctly the directory name and the de hidden file as you will see on the terminal.
- Also, I have used < ls -a > for showing all files, including the hidden one. I have not used that just like that, I have used one of search-engine I learned. The command was < man ls >.
- And the last one, if you pay attention, you will see that I used : < cat ./...Hiding-From-You > instead of < cat "./...Hiding-From-You" >.
  No worries, both work in this case beacuse the filename has no spaces. When they are no spaces, quotes are optional. I did not know until I tried both ways.
