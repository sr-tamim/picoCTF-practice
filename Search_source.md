# Search source

### Challenge Description
The developer of this website mistakenly left an important artifact in the website source, can you find it?
The website is [here](http://saturn.picoctf.net:65086/)

### My Solution Flowchart
1. I opened the website and it was a yoga website. I right clicked on the page and clicked on `View page source`
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/cc1a9ffb-294e-48b3-a109-39a573ac22c6)

2. I was scrolling through the page source text and searching for any clue. Suddenly I saw something.
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/96e802ec-3137-440a-b0b6-6ba56ea47fda)

3. It said there is nothing but still I scrolled through the end of the source text and found nothing.
4. Then I started going through all the linked files mentioned in the header section.
5. First I visited `css/owl.carousel.min.css` and got nothing
6. Then I went to `css/style.css` and there was a pretty big css file.
7. I scrolled from up to bottom of the file but couldn't find anything.
8. Then I opened text search in the browser and searched for `pico` and got the flag
   ![image](https://github.com/sr-tamim/picoCTF-practice/assets/86656406/b01f73b8-90ba-49dd-912c-b37152b5911d)
