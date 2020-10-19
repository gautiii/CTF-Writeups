# HACTOBER CTF 2020
![deadface](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/OSINT/images/deadface.png)

'DEADFACE is a notorious hacker group made up of largely of hacktivists that target businesses, government, universities, and individuals. While they're active year-round, they always increase their activity in October with the intent to wreak havoc and cause mayhem. They have no particular political or idealogical affiliation - they simply enjoy hacking whether it's breaking systems or stealing data.'

Link to CTF - http://ctf.cyberhacktics.com/intel
This Capture the flag event had an imaginary hacker group called 'DEADFACE'. All of the challenges were based around this group.


# OSINT
## CREEPING 1

![creeping 1](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/OSINT/images/creeping1.PNG)

The first link that came up on google when I searched for Ali Tevlin was his facebook page. The page had only a few posts so it was easy to get his job details.

![ali tevlin work](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/OSINT/images/aliv%20tevlin%20work.PNG)

Flag - flag{F. Kreuger Financial}


## CREEPING 2

The answer for this question is in the previous answer. 
Flag - flag{Senior Acquisitions Supervisor}


## CREEPING 3

![creeping 3](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/OSINT/images/creeping3.PNG)

This flag can be found just below his work details in his facebook page.

![ali tevlin dob](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/OSINT/images/ali%20tevlin%20dob.PNG)

Flag - flag{17 jun 1973}


## CREEPING 4

![creeping 4](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/OSINT/images/creeping4.PNG)

Going through his facebook page, I found 3 posts. One of them was posted on August 12 which could be the picture he took on his vacation.

![mothman](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/OSINT/images/mothman.PNG)

I did a reverse image search for this image on https://yandex.com/ (The best site for reverse image searches).
The first link gave away the answer to this question.

![mothman yandex](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/OSINT/images/mothman%20yandex.PNG)

Point Pleasant is the city name and West Virginia is the state. (The statue is called Mothman)

Flag - flag{Point Pleasant, WV}.


## PAST ATTACKS

![past attacks](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/OSINT/images/past%20attacks.PNG)

This challenge seemed vague when I read it. I had to use some hints given in the challenge to crack this. 
When I searched for 'attacks that has hit financial institutions', the first link gave lots of attacks that I tried as the flag. I had to try the second hint after hours of digging. The second hint revealed that the attack hit a Polish financial institution. 

![polish attack](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/OSINT/images/polish%20attack.PNG)

The first link gave away the answer - Watering hole attack. Watch this video for a basic understanding of this attack. https://www.youtube.com/watch?v=GUQw4R3QGJ8

Flag - flag{watering hole}
