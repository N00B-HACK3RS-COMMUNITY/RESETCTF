# RESTCON CTF Writeup
---
Organised by _Resethackers_ 
Date: _28 August 2020 10:30AM - 12:00 AM (IST)_
***
## Basic Challenges:

# Basic : 1
---
![](https://samaritan106.files.wordpress.com/2020/08/cb964-1fqwawqxwejkmhpqg9enqxw.png)
***
flag submitted by [_@hacker_oneness](https://www.instagram.com/hack3r_oneness/)_ , **Captain**

This flag was very simple but when i first looked at this i was quite confused. I thought it is ROT13, by the time i figured it out what it was my teammate already submitted the flag

It was quite simple the text was reversed. I used [Cyberchef](http://icyberchef.com/) tool to get the flag, whereas you can do it manually too.

---
![](https://samaritan106.files.wordpress.com/2020/08/base.png?w=1024)
***
After reversing this **“`}GALF_NOCTSER{NOCTSER`”** and flag is **“RESTCON{RESTCON_FLAG}“**

# Base: 2:-
---
![](https://samaritan106.files.wordpress.com/2020/08/1.png)
***
flag submitted by [_@106_Sam_](https://www.instagram.com/106_sam/) , **CTF Team member** 

A hacker can guess at a glance that it is encoded in BASE64 **`“UkVTVENPTntSRVNUQ09OXzJORF9CQVNJQ19GTEFHfQ==“`**

> _Note:- Base64 has “==” at the end of their strings_

In CyberChef, search “Base64” in search box drag and drop it in Recipe column and paste the above text in input column 

---
![](https://samaritan106.files.wordpress.com/2020/08/2.png?w=1024)
***

Flag: **RESTCON{RESTCON_2ND_BASIC_FLAG}**

# Base: 3
---
![](https://samaritan106.files.wordpress.com/2020/08/1-1.png)
***
flag submitted by [_@JayaLakshmi_](https://www.instagram.com/jayalakshmi7599/) , **CTF Team member**

In this Challenge they gave file named “Chal.txt”. We can download the file by clicking on the ” Chal file ” . But i used Linux Command “wget <file-URL>” and downloaded in specific folder through my terminal 
  
When i opened this file i saw this text **```“ ;FOM6VgI(;FOM6VgHa5u(3T84?E`6:”OA6XN;V5t?> “```**

---
![](https://samaritan106.files.wordpress.com/2020/08/2-1.png)
***
Got to know that it is ASCII85 by searching on [cryptii](https://cryptii.com/) website after decoding i got the flag.

---
![](https://samaritan106.files.wordpress.com/2020/08/3.png?w=1024)
***
Flag: **RESTCON{RESTCON_ANOTHER_BASIC_FLAG}**

# Broken 
---
![](https://samaritan106.files.wordpress.com/2020/08/1-2.png)
***
flag submitted by [_@106_Sam_](https://www.instagram.com/106_sam/) , **CTF Team member**

This flag took me only 25 seconds to capture. As in above image “Your Flag is hear” and a undefined image link. Simply i did a **right click > copy Image location** and created new tab and paste the image link
---
![](https://samaritan106.files.wordpress.com/2020/08/2-2.png?w=1024)
***
It was showing **“404 error”** with **“File not found, Sorry about that”** Then i looked at the URL there i saw **“https://ctf.resethacker/`RESTCON{HIDD3N}`“**

---
![](https://samaritan106.files.wordpress.com/2020/08/3-1.png?w=1024)
***
Flag: RESTCON{HIDD3N}
> _Note: "HIDD3N" is a Basic form of leetspeak language

# Garbage

---
![](https://samaritan106.files.wordpress.com/2020/08/1-4.png)
***
flag submitted by [_@106_Sam_](https://www.instagram.com/106_sam/) , **CTF Team member**

This challenge gave us a file named “garbage.txt” which was corrupted. As this file got corrupted the file got itself converted into binary data.

So first step i did when i downloaded this file using linux command **“wget”** is i used Command **“file (file-name)”** to check what type of Data is inside the file **garbage.txt**

Second step : i used command **“cat garbage.txt | grep RESTCON ”** to know if the flag is there in it or not. I got to know that **“Binary input(standard input) matches"**

> _Note : command ‘cat’ is used to list whats inside the file , symbol ‘|’ this is called ‘Pipe’ it is used to divided the command , command ‘grep’ it is used to search the specific text from the given file and shows us._
---
![](https://samaritan106.files.wordpress.com/2020/08/2-3.png)
***
Third step : i just simply used ‘cat garbage.txt’ to list the text inside the file. The file was filled with the binary data…but at the end there was the flag **“RESTCON{GR3P_7HE_FL4GS}“**.

there is another way of finding the flag just use command **“strings (file-name)”**

---
![](https://samaritan106.files.wordpress.com/2020/08/3-2.png?w=1024)
***
Flag : **RESTCON{GR3P_7HE_FL4G}**

# Weirdo: 1
---
![](https://samaritan106.files.wordpress.com/2020/08/1-5.png)
***
flag submitted by [_@106_Sam_](https://www.instagram.com/106_sam/) , **CTF Team member**

When i clicked **“File”** a file named **“weirdo1.txt”** was download. When i **“cat weirdo1.txt"**. There was lot of symbols, alphabets, and etc. It took so much time to figure out what can this message be i tried reversing and i was checking for metadata of the file etc. Then i thought it might be some other type of morse code(but it wan’t). After doing much research got to know that it is **“Malbolge Programming Language”**.

---
[](https://samaritan106.files.wordpress.com/2020/08/2-4.png?w=1024)
***
>_Note: Malbolge, invented by Ben Olmstead in 1998, is an esoteric programming language designed to be as difficult to program in as possible. And so it is 🙂 _

I used a online interpreter to compile and capturing the flag [Malbolge](http://malbolge.doleczek.pl/)

---
![](https://samaritan106.files.wordpress.com/2020/08/3-3.png?w=1024)
***
Flag: **RESTCON{Malb0lg3_is_cool}**

# In Plain Sight
---
![](https://miro.medium.com/max/487/1*X9vBfiYzOYtM1xDLo2Ix2g.png)
***
