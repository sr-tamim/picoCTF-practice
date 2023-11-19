# strings it
## Challenge Description
Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings) without running it?

## My Solution Flowchart
1. It's easy. The solution is in the name of the challenge.
2. I have to find the flag in the string output of the file.
3. So, I opened the bash terminal in the folder where I have downloaded the given file.
4. Then I ran below command in the terminal 
   ```bash
     strings ./strings | grep pico
   ```   
   Here I have used the `strings` command to get the string version of the file. Here the filename is also "strings" so the next part is `./strings` and then I used `grep` command after pipe character to search through the output. I searched for the word "pico" because I knew that the flag is gonna start with the word `picoCTF`
5. And as soon as I pressed `Enter` key, the flag showed up 😃
