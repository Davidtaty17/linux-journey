LEVEL 2->3 : Find the key for the next level
Location: Home directory / Stored In a file called: --spaces in this filename--
Commands for this level: ls, cd, cat, file, find

How to solve this level ?
=> Log into game using ssh with < bandit3 > as user and use the password found in the  previous level.
=> Use < ls > for listing the directory contents and find the file
=> Once the file is identified, we will use  < cat "./--spaces in this filename--" >  for printing the key on the screen.
=> Log out with < CTRL + D > or Type < exit> on terminal

In this case I found an issue when I was typing my command to open file. Using < cat ./ ...> was not enough, because terminal did not recognize < --spaces in this filename-- > as one single file. 
The question is : How can we open a filename or file with space? 
"We must wrap the entire filename in quotes so the terminal treats it as one single argument" 

the final command was: cat "./--spaces in this filename--"

