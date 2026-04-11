LEVEL 1->2 : Find the key for the next level

Location: Home directory
Stored: In a file called " ** - ** "
Commands for this level: ls, cd, cat, file, find
Mission: find the key for next level.


How to solve this level ?
=> Log into game using ssh with ** bandit1 ** as user
=> Use ** ls** for listing the directory contents
=> Once the file is identified. We will use ** "cat" ** + ** "./" ** + ** "-" ** for print the key on the screen 
=> Log out with ** ctrl + D ** or ** exit **


** Why did we use " cat ./- instead of cat - " ? **
Because adding " ./ " before a ** filename ** tells the terminal to treat it as a path to a file, not as a special symbol.
** A filename ** is simply the name of a file.
