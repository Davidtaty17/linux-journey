# LEVEL 10->11 : Find the key for the next level

**Location**:Stored in a file **data.txt**, which contains base64 encoded data.

**Useful commands**: grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## How to solve this level?
=> Log into the game using ssh with **bandit9** as username and the password found in the previous level;  

=> Use **ls** to list directory content and find the file;

=> Once the file is located, use **base64 -d data.txt** to decode data to standard output and print it;

=> Log out with **CTRL + D** or **exit**.

## Observations 
- I ran first *cat data.txt* to see what was inside and the terminal returned me a large mix of letters and numbers, ending with two *==*.
  Then, I ran **base64 data.txt* and the terminal returned me two lines of a mix of letters and numbers again but without the double *==*.
  
- All of that was a reflexe that I do habitually since I have stared with bandit. Observing details on the mission and following my instinct. That was not a good way to do.
  
- The right thing I generally do after my request declied, is using the command **man**(it explains me how to use a command) to understand the new command that I will use. Generally is next to the last one that I have learned in th eprevious level.
  In this case, It was **man base64**.
  *base64* encode/decode data and print to standard output. I used the options *-d* to decode data.
