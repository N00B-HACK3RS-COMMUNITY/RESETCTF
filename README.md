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
