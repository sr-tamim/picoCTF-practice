# Who are you?

# Challenge Description
Let me in. Let me iiiiiiinnnnnnnnnnnnnnnnnnnn 

http://mercury.picoctf.net:34588/

# My Solution Flowchart
1. This challenge is pretty interesting one and it has 200 points in return. I visited the URL on browser and there is a GIF saying "Who are you?" and above that there is a clue sentence:
   > Only people who use the official PicoBrowser are allowed on this site!
2. I understood the thing here, I need to change the user agent. So, I opened postman client and hit the URL again setting the `User-Agent=PicoBrowser` in the header part of the request.
   > I don't trust users visiting from another site.
3. So now it says that I am not trusted. **Referer** header can make me trusted to the website but Referer value must be same as the host website, in this case it's `http://mercury.picoctf.net:34588/` I need to setup `Referer=http://mercury.picoctf.net:34588/` in the request header with previous user-agent config.
   > Sorry, this site only worked in 2018.
4. Now I need to time travel back to the year 2018 when Iron Man was alive. I just set `Date=2018` in header and boom, it worked.
   > I don't trust users who can be tracked.
5. So, now I have to make me untrackable. Okay, I am gonna do it by sending **Do not track** request in the header. I set `DNT=1` in the header config and hit the URL again and got response:
   > This website is only for people from Sweden.
