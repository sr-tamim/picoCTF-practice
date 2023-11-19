# Wave a flag

## Challenge Description
Can you invoke help flags for a tool or binary? [This program](https://mercury.picoctf.net/static/fc1d77192c544314efece5dd309092e3/warm) has extraordinarily helpful information...

## My Solution Flowchart
1. After downloading I tried to run the file in bash terminal but I failed
2. Oops, I forgot the make the file executable after downloading
3. So, I made it executable and ran in in bash terminal. Here the filename is `warm`
   ```bash
     ./warm
   ```
   Output:
   > Hello user! Pass me a -h to learn what I can do!
4. Then I have passed `-h` flag with the previous command
   ```bash
     ./warm -h
   ```
   Output:
   > Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1******4}
   
5. So, this is how I got the flag...

