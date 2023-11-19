# Get aHEAD

## Challenge Descriptoin
Find the flag being held on this server to get ahead of the competition

http://mercury.picoctf.net:28916/

## My Solution Flowchart
1. First I visited the webpage from the browser and there is two buttons which changes the background color of the page.
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/b9578a7d-b226-4a66-bc65-ad6b81ca56c7)
2. I opened network tab and found nothing special.
3. So, I opened Postman client to play with the url.
4. After playing with request headers for awhile I got nothing and I was clueless.
5. Then I did some research and understood the mystery behind the challenge name.
6. The name is `Get aHEAD` and here the part `HEAD` is all uppercase. So, there is something to do with this word.
7. Then simply I just did a HEAD request instead of GET or POST request using Postman.
8. And thus I got the flags in response headers
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/ca338a6b-f4f9-4eae-802b-34498231f19b)
 
