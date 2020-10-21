# FORENSICS

# CAPTURED MEMORIES

![captured memories](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Forensics/images/captured%20memories.PNG)

For memory forensics, I used volatility in linux. It can be installed using the command - apt install volatility.
We can also use the python version of the tool - https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjb36mbl8XsAhWAyzgGHU2RCf0QFjAAegQICxAD&url=https%3A%2F%2Fgithub.com%2Fvolatilityfoundation%2Fvolatility&usg=AOvVaw1_vBpA3qj3hVAAoPRS0Ta4

To get all the possible profiles for this dump, the command is - volatility -f [filename] imageinfo

![imageinfo](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Forensics/images/imageinfo.PNG)

Here we can see there are 6 profiles. The first one worked for me and I used 'pslist' to further get the running processes and their IDs. 
volatility -f [filename] --profile=Win10x64_17134 pslist

![pslist](https://github.com/gautiii/CTF-Writeups/blob/main/HacktoberCTF%202020/Forensics/images/pslist.PNG)

The actual list is quite long. The last process in the list is 'winpmem_v3.3.r' , which could most probably be the process that captured the memory dump, given that its name has a 'mem' in it. The flag is the PID of this process

Flag - flag{3348}
