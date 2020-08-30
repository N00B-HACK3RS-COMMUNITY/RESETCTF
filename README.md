# RESTCON CTF Writeup
---
Organised by _Resethackers_ 
Date: _28 August 2020 10:30AM - 12:00 AM (IST)_
***
writeup by [@106_Sam](https://www.instagram.com/106_sam/)
---
Team Name: Q_For_Quaratine ([@N00B_Hack3r_Community](https://www.instagram.com/noob_hack3rs_community/))
We secured 68th rank out of 380 teams
Congratulation to Top 10 teams (Just go grab the prizes)
---
[Click to see the video of RESTCON CTF](https://www.instagram.com/tv/CEcgeL3p3XS/?utm_source=ig_web_copy_link)
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
This was a difficult one as u can see only 29 Solves.

Thanks to _[m3ta_c1ph4r](https://medium.com/@ashutoshg547) A.k.a [Ashutosh Gupta](https://medium.com/@ashutoshg547)_ for solution

So if you will see it just says as a normal plain text. If you google this as you will see a song name. But it is nothing related to the this question. So I directly to the solution. If you notice **“bum bum, tam tam tam.”** the last **‘.’** if you click on that it is a hyperlink. It will download one file. When you open it you will see some strange sentences. So to solve this I made a python script.

---
```python

st = """ah, ah
(¡wuh!)
y que griten los que están presentes
hoY va a bailar sin precedentes (wooh)
estoy tan pegao' que no salgo de tu mente (salgo de tu mente)
quieren apagarme y yO no tengo fuente
pa' bailar no existen prueba' (prueba')
este funky si es candela (wooh)
de aquí nadie va pa' fuera (aye)
esto lo bailan en la favela(ooh)
izqUierda, derecha
pa' arriba, pa' abajo
izquierda, derecha
rompiendo (wooh)
é a flauta envolvente que mexe com a mente
de quem tá presente
as novinha saliente
fica loucona e se joGa pra gente
aí, eu falei assim pra ela, ó
(aí, eu falei assim pra ela)
vai, vai com O bum bum, tam tam
mueve ese bum bum, tam tam
mueve ese bum bum, tam tam tam
mueve ese bum bum, tam tam
mueve ese bum bum, Tam tam Tam
mueve ese bum bum, ese bum bum
ese bum bum bum bum bum bum bum bum bum
(bum bum bum bum bum bum bum bum)
don
back it up me man cock it and rev it (and rev it)
and not just any man can get it (can get it)
mi naH care if you have good credit
you betta can handle the ting whEn mi send it (wooh)
man a drop off (wooh), mama pop off (wooh)
gyal walk off (wooh), 'til it bruk off (wooh)
don't stop oFf (wooh), 'til it slop off (wooh)
good pussy make the whole dance Lack off
(woooooh)
boy, turn it, see me ting turn up
turn up the ting 'til the ting burn up ('til it burn up)
whine pon the gyal 'til the gyal mash up ('til it mash up)
back up the ting like a dumper truck
Ayo, my ting good (ting good) and my ting shocks (ting shock)
and the ting set (ting set), and it sittin' loud (sit loud)
and the gyal Good (gyal good), but my face bad
'cah me ting ting real, and it can't stop
don
é a Flauta envolvente que mexe com a mente
de quem tá pResente
as novinha saliente
fica loucona e se jOga pra gente
aí, eu falei assim pra ela, ó
(aí, eu falei assiM pra ela)
vai, vai com o bum bum, tam tam
vem com o bum bum, tam tam tam
vai, mexe o Bum bum, tam tam
vem, desce o bUm bum, tam tam tam
vai, mexe o buM bum, tam tam
vem, desce o bum bum
vai com o bum bum (e aê, fioti?)
rompiendo
i know that thing that you like
i know the way that you move
we makin' love the first night, bum bum pac pac bum
yeah, hey, big up my jeweler, big up my .45, big up my ruger
hey, big up the bad bih, call that chimmie like king of the bunda
yeah, i'm a savage, summon 21, summon the cougars
hey, automatic spazzin', jumping in the crowd just like uzi
yeah, black stallion, i'ma go flex and fly out to cuba
yeah, if you got good pussy, let me hear you say hallelujah
yeah
é a flauta envolvente que mexe com a mente
de quem tá presente
as novinha saliente
fica loucona e se joga pra gente
aí, eu falei assim pra ela, ó
(aí, eu falei assim pra ela)
vai, treme o bum bum, tam tam tam tam (vem)
tam tam tam tam tam tam tam tam (vai)
tam tam tam Tam tam tam tam tam (vem)
tam tam tam tam tam tam tam tam (vai)
tam tam tam tAm tam tam tam tam (vem)
tam tam tam (tipo vavazinho)
(vai, vai com o buM bum, Tam tam)
le toco la flauta y se pone pa' mi
(vai, mexe o bum bum)
yo prendo el Ambiente
yo tengo la malla, déjamela ahí
(vai, mexe o bum bum, tam tam)
y yo la toco así, y yo la toco así
y después de un Momento
ella se olvida de tí (bum bum, tam tam tam tam tam)
se olvida porque solo le hablan de joya, botella y dinero
nosotros le damos lo que a ella le gusta
por eso es que estamos primero
y yo la toco así, y yo la toco así
y después de un momento
ella se olvida de tí"""
for i in st:
    if ord(i) >= 65 and ord(i) <= 91:
        print(i, end="")

```
***
So in this script it will print those characters which are CAPITAL. So when you execute this script you will see this output **“YOUGOTTHEFLAGFROMBUMTAMTAM”**. So in the question you will see that they said **“Flag is in Leet Speak language”**. So I just google this and I found this on [dcode.fr](https://www.dcode.fr/leet-speak-1337) . And when you tap on the encode .

>_Note: dcode.fr is a french sites, it is one of the best site for encoding and decoding text_
---
![](https://samaritan106.files.wordpress.com/2020/08/e74ea-1ult97tjvigeyavajy7gg6a.png)
***
So firstly I tried that leet code but that didn’t work so I tried that above. And it worked.

Flag: **RESTCON{Y0U6077H3F146Fr0M8UM74M74M}**
----This is the end of “Basic challenges”----- other challenges coming soon...
