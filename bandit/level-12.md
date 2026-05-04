# LEVEL 11->12 : Find the key for the next level

**Location**:Stored in a file **data.txt**, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

**Useful commands**: grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

*ROT13*

## How to solve this level?
=> Log into the game using ssh with **bandit12** as username and the password found in the previous level;  

=> Use **ls** to list directory content and find the file;

=>Once the file is located, use **cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'**, to read the content file decoded;

=> Log out with **CTRL + D** or **exit**.

## Observations 
-  The concept **ROT13** is encoding which all letters will be replace by 13 positions forward in the alphabet.
In this case, I decryption the content of *data.txt*. **Encoding** has no key and anyone can reverse it.
-  **How did I decode the file?**
  -> I use the command *tr* that mainly does the translation and works with two arguments; the input group ( A-Za-z) which contents all lowercase and uppercase letters of alphabet, and
   the output group ( N-ZA-Mn-za-m ) that will be replaced with.
   -> If you have noticed, we wrote **N-ZA-M** because we must provide a full 26 letter mapping: N-Z handles A-M and A-M handles N-Z.

*This level was the most difficult one that I have done so far*
