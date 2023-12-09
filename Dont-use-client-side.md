# Dont-use-client-side

### Challenge Description
Can you break into this super secure portal? https://jupiter.challenges.picoctf.org/problem/17682/ or http://jupiter.challenges.picoctf.org:17682

### My Solution Flowchart

1. I visited the webpage and there was a input field for entering password to verify.
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/73278366-3d9d-48dc-8c26-93a95f8532f9)

2. Then I opened the network tab and found a HTML file. There was a verify function written inside the script tag. Inside that function, there was nested if conditions.
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/259826b2-4f8d-44eb-b19a-a4cda2a595e5)

4. Then I just read the verify function attentively and understand all the conditions. I wrote the flag manually and put it in the input and clicked verify button to check and it worked.
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/dcadd62d-bfc5-4dac-a415-3438c15b148e)
