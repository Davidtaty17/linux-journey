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

- **ROT13** is encrypting by substitution. It *replaces each letter with the next 13th in the alphabet*, and mainly used to hide spoilers or texts in a reversible way (applying the algorithm twice restores the original text). And it offers no real security and is treated as encoding in practice.
In this case, I decoded the content of *data.txt*. 
- **How did I decode the file?**
  -> I started with the command **cat** which helped me to print the content of file on display;
  -> Following with te pipe **|** that permit the terminal to run the next command and avoid me to type again;
  -> I used the command **tr** that mainly does the translation of characters and works with two arguments; the *input group ( A-Za-z)** which content all lowercase and uppercase letters of alphabet, and he **output group ( N-ZA-Mn-za-m )* that will be replaced with.
   -> If you have noticed, we wrote **N-ZA-M** which seems quite confusing, the *ROT13** says that the first part of the alphabet (A-M goes at the second part (N-Z), and the same fo the second part that takes places of the first one. That become *( N-ZA-M )**. And one more thing you must write for all characters, I mean even the lowercase and uppercase letters. That is why we wrote *N-ZA-Mn-za-m*.
  The single quotes **'** are used to protect the content from the terminal interpreting it as something special.
   
*This level was the most difficult one that I have done so far*
