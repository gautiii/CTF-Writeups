# CRYPTOGRAPHY

# HAIL CAESAR!

![hail caesar](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Cryptography/images/hail%20caesar.PNG)

An image and an encoded message was given in the challenge - TGG KUSJWV QGM

![crypto01](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Cryptography/images/crypto01.png)

This was the easiest of all the challenges. The challenge name is hail caesar which gives away the cipher type. The image too was quite revealing with the alphabets. 
The message can be decoded using caesar cipher on https://www.dcode.fr/chiffre-cesar . 

![c1](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Cryptography/images/c1.PNG)

One of the deciphered lines makes sense - BOO SCARED YOU
Flag - flag{BOO SCARED YOU)


# DOWN THE WRONG PATH

![down the wrong path](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Cryptography/images/down%20the%20wrong%20path.PNG)

The given image:

![crytpo02](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Cryptography/images/crypto02.png)

The four encoded lines when read from top to bottom column-wise made sense. Also, the name of the challenge is 'Down the wrong path'. 
The deciphered message is - REMEMBERTOTELLSPOOKYBOIABOUTTHENEWTARGETSOFOURNEXTATTACK
                            REMEMBER TO TELL SPOOKYBOI ABOUT THE NEW TARGETS OF OUR NEXT ATTACK
The message is intended for spookyboi(an member of the deadface hacker group).
Flag - flag{spookyboi}


# COVER YOUR BASES

![cover your bases](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Cryptography/images/cover%20your%20bases.PNG)

Encoded message - ZmxhZ3tzaG91bGRhX21hZGVfdGhpc19vbmVfaGFyZGVyfQ==

I could figure out that this message was a base64 encoded message with the '==' at the end of the message and for the obvious reason that the name of the challenge is 'Cover your bases'. 

Base64 can be encoded easily on any online tool. I personally prefer CyberChef (https://gchq.github.io/CyberChef/) which is very handy and user friendly. 
Decoded message - flag{shoulda_made_this_one_harder}

Flag - flag{shoulda_made_this_one_harder}


# BONE TO PICK

![bone to pick](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Cryptography/images/bone%20to%20pick.PNG)

Link to encoded message - https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Cryptography/images/bone%20to%20pick

The message is a very very long encoded string which seemed scary at first. After trying multiple encoding formats on cyberchef, I came across this format called magic. Actually, its not an encoding format but it attempts to detect various properties of the input data and suggests which operations could help to make more sense of it.

![magic1](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Cryptography/images/magic1.PNG)

Here, the first link under output shows us that it is in a jpeg format. After clicking this link (https://gchq.github.io/CyberChef/#recipe=From_Base64('A-Za-z0-9-_',true)Render_Image('Raw')) the page is automatically set to decode a message of Base64('A-Za-z0-9-_',true) format.

![magic2](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Cryptography/images/magic2.PNG)

The decoded message is in fact an image with the flag.

Flag - flag{angrybones}
