# Who are you?

# Challenge Description
Let me in. Let me iiiiiiinnnnnnnnnnnnnnnnnnnn 

http://mercury.picoctf.net:34588/

# My Solution Flowchart
1. This challenge is pretty interesting one and it has 200 points in return. I visited the URL on browser and there is a GIF saying "Who are you?" and above that there is a clue sentence:
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/b7046a68-7ca0-4230-b021-f6bddfff5681)

2. I understood the thing here, I need to change the user agent. So, I opened postman client and hit the URL again setting the `User-Agent=PicoBrowser` in the header part of the request.
   > I don't trust users visiting from another site.
3. So now it says that I am not trusted. **Referer** header can make me trusted to the website but Referer value must be same as the host website, in this case it's `http://mercury.picoctf.net:34588/` I need to setup `Referer=http://mercury.picoctf.net:34588/` in the request header with previous user-agent config.
   > Sorry, this site only worked in 2018.
4. Now I need to time travel back to the year 2018 when Iron Man was alive. I just set `Date=2018` in header and boom, it worked.
   > I don't trust users who can be tracked.
5. So, now I have to make me untrackable. Okay, I am gonna do it by sending **Do not track** request in the header. I set `DNT=1` in the header config and hit the URL again and got response:
   > This website is only for people from Sweden.
6. How can I go to Sweden now only to visit one webpage! That doesn't makes sense. Well there is another way we can pretend to be in Sweden modifying headers. I just set the value of `X-Forwarded-For` property to an ip address of sweden. I got an swedish ip address searching in Google.
   > You're in Sweden but you don't speak Swedish?
7. Let's setup language in the header. `Accept-Language=sv`
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/812ef26a-9bc2-4554-a452-46bd5c114f07)
8. Hurray! I got the flag...

*Throught the full process [MDN docs](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers) helped me a lot*
