## Challenge Description
Kishor Balan tipped us off that the following code may need inspection:
https://jupiter.challenges.picoctf.org/problem/9670/ or http://jupiter.challenges.picoctf.org:9670

## My Solution Flowchart
1. First I visited the [webpage](https://jupiter.challenges.picoctf.org/problem/9670/) and there is a simple html page. There is two buttons, one is `What` and other one is `How`, Nothing special.
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/88a95b71-3b2f-434b-9312-2bc2d920d1b3)
2. Then I opened network tab and tried to get some clues.
3. I found something inside the html file. There is the first part of the flag.
   > Html is neat. Anyways have 1/3 of the flag: picoCTF{****
4. Then I was pretty sure that I am gonna find something in css and js files also.
5. So, I looked at the css file and found second part of the flag.
   > You need CSS to make pretty pages. Here's part 2/3 of the flag: t3****
6. After that I opened js file in network tab and found last part of the flag
   > Javascript sure is neat. Anyways part 3/3 of the flag: _luc*****}
7. Thus I solved this challenge
