# Logon

### Challenge Description
The factory is hiding things from all of its users. Can you login as Joe and find what they've been looking at? https://jupiter.challenges.picoctf.org/problem/44573/ or http://jupiter.challenges.picoctf.org:44573

### My Solution Flowchart
1. I opened the webpage and there is two input fields which takes username and password as login credentials.

2. I tried to login with `username=Joe` and a random password and failed
![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/1269dd41-b265-4fc2-a219-fbcea8dda81d)

3. Then I just tried again with some random username and password. It worked
`username=kpabyt` and `password=kpabyt`
![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/14b1c81b-2cc1-4c87-855f-6843405b540f)

4. Then I thought there can be something in session storage or local storage or cookies because we have logged in and there must be some kind of auth key saved somewhere.

5. I looked around and found one cookie named admin which has False value
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/87acfd4a-2155-4827-9671-3dd3ce19acc0)

7. I modified the value of admin to True and reload the page and the flag is here..
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/59808cdd-ab0a-4d5d-a722-3561f26e2892)

