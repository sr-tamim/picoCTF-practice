# Login

### Challenge Description
My dog-sitter's brother made this website but I can't get in; can you help?

https://login.mars.picoctf.net


### My Solution Flowchart
1. There is two input fields (username and password) for login. I have tried to login something random but it didn’t work.

2. I visited the page and opened network tab to see all files. HTML and CSS files contained nothing special but there is something interesting in JS file.
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/9cfff2d0-da57-454e-b69d-5c4dc723063a)

3. Seems like the code compare the input after converting to Base64 string. So, I have to just decode the comparison text to normal string.
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/f2ff8af3-1ed7-4d3d-ad10-ae21f5330f11)

4. I copied the base64 string from the condition part and used atob function to decode it.
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/1ce581e5-b29c-445b-ab8b-ddf0bacf59ce)
