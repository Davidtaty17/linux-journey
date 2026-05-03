# LEVEL 3->4 : Find the key for the next level 

**Location**:Stored in a hidden file in a directory named **inhere** 

**Useful commands**: ls, cd, cat, file, find

## How to solve this level ?

=> Log into the game using ssh with **bandit3** as username and the password found in the previous level;

=> Use **ls** to list the home directory contents and find our directory;

=> Once the directory located, use **cd inhere** to *change* the current *directory* to **inhere**; 

=> Type **ls -a** and it will list all the contents of this directory even the hidden ones;

=> Once our **hidden file** is located, use **cat ./...Hiding-From-You** to print the content on the screen.

=> Log out with **CTRL + D** or **exit** on the terminal 


## Observations

- In this level, you should make sure that you have written correctly the directory name and the ***hidden file** as you will see on the terminal. Just *revise* your writing
  
- Also, I used **ls -a** for listing all files, including the hidden one.
   I didn't know this flag beforehand, I have used one of *search-engine* that I learned. It was **man ls** to explain me how to use deeply this command. 
  
- And the last one, if you pay attention, you will see that I ran **cat ./...Hiding-From-You** instead of **cat "./...Hiding-From-You"**.
  **No worries**, both work in this case beacuse *the filename* has no spaces. When there are no spaces, *quotes are optional*. I did not know until I tried both.
