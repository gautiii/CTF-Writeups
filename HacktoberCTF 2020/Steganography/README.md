# STEGANOGRAPHY

# GHOST HUNTER

![ghost hunter](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Steganography/images/ghost%20hunter.PNG)

The image:

![ghost01](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Steganography/images/ghost_01.png)

First I tried - strings [filename] , to get all the characters from the raw file but this didn't reveal anything. Binwalk and stegoveritas too didn't find any flag. Finally, zsteg worked!

![zsteg](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Steganography/images/zsteg.PNG)

One of the lines from the output had the flag.

Flag - flag{8862a805a3140996343da91bdcbda79e}


# YOU BELIEVE IN GHOSTS?

![you believe in ghosts](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Steganography/images/you%20believe%20in%20ghosts.PNG)

The given image:

![steg01](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Steganography/images/steg01.png)

I tried tools like zsteg, binwalk, stegoveritias, but nothing was useful. There are 'almost invisible' ghosts in the image. Probably stegsolve could get us something good. Stegsolve applies many filters on the image. 

![stegsolve](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Steganography/images/stegsolve.PNG)

And yes it did give us the flag!

Flag - flag{ghosts_everywhere}

# BLASPHEMY

![blasphemy](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Steganography/images/blasphemy.PNG)

The given image:

![witches](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Steganography/images/witches.jpg)

Given that its a jpg image, the first tool I tried was steghide. The command is - steghide extract -sf [filename]. Since no passphrase was given, I used a blank passphrase for extracting from this image.

![steghide](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Steganography/images/steghide.PNG)

The extracted data was written to a file named secret.txt.o which contained the flag.

Flag - flag{950634ccc97ca3ef03e22c759a356973}


