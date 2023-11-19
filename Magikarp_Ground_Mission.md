# Magikarp Ground Mission

## Challenge Description
Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin. Login via `ssh` as `ctf-player` with the password, `6****`

## My Solution Flowchart
1. It was so easy. I opened the webshell in picoCTF web and ssh into the server.
2. There was 2 text files when I `ls` in the folder. One file contains the first part of the flag and other one says what to do next.
   ```bash
     cat 1of3.txt
     cat instructions-to-2of3.txt
   ```
3. Then I changed the directory to root as instructed in previous txt file.
   ```bash
     cd /
     ls
     cat 2of3.txt
     cat instructions-to-3of3.txt
   ```
4. Then I went to home directory as instructed in previous file.
   ```bash
     cd ~
     ls
     cat 3of3.txt
   ```
5. Thus I got all the parts of the flag and done. Then just pressed `Ctrl + D` to logout.

