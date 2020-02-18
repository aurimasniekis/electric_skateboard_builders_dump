# Chinese remote with LCD

### Replies: 23 Views: 790

## \#1 Posted by: Marksmoura Posted at: 2019-01-28T10:22:44.790Z Reads: 226

```
Hello guys, so I am currently working in China for 1 year already and built my own skateboard with a really low end remote.

Last week I saw for sale a new remote for the Chinese vesc the one like meepo has and I decided to try to hack it and make it work with arduino with an rf module or Bluetooth. 

I am not entirely sure what module they use for comunication but I would guess that it is the RF module. I just unpack it as I write this post. I will open it and try to Frankenstein it for the following days. 

Has anyone seen this remote already? Does anyone have it? For 12€ (92 rmb) I got a great deal for it.

Here pics:

![IMG_20190128_181754|375x500](upload://zJFrvQwOcWBSvex93FxEuoQZ2Qc.jpeg) 
![IMG_20190128_181828|375x500](upload://AdH7cetGMhiYHPIsmXW26vLzvF4.jpeg)
```

---
## \#2 Posted by: Marksmoura Posted at: 2019-01-28T10:38:30.815Z Reads: 221

```
![IMG_20190128_183712|613x500](upload://2Ky6k9Px3zX0paAfyVRlF2RgfxG.jpeg) ![IMG_20190128_183536|375x500](upload://7i30Te6UA4Z6PYXhKPhIynVnpO4.jpeg) ![IMG_20190128_183555|666x500](upload://uenh3DF7VFhd6hIJbMKd7a5UN2W.jpeg)![IMG_20190128_185518|454x344](upload://qwfuVkSoRm3slgjAOeNlESRv7pZ.jpeg)
```

---
## \#3 Posted by: Superflim Posted at: 2019-01-28T10:53:18.413Z Reads: 209

```
looks cool and that price! 😍
```

---
## \#4 Posted by: LukePL Posted at: 2019-01-28T10:54:04.033Z Reads: 209

```
Looks nice and if you could make it work with Vesc you are going to be a hero :smiley:
```

---
## \#5 Posted by: Marksmoura Posted at: 2019-01-28T10:58:44.991Z Reads: 206

```
Basiy they have a Chinese micro controller I've never heard about. At the moment I just know how to program an arduino. I could solder it out and integrate an arduino mini inside and use the LCD and communication module it already has or try to figure out how to program this micro.

Someone? I don't want to start from scratch :D
```

---
## \#6 Posted by: DavidBanner Posted at: 2019-01-28T10:59:41.749Z Reads: 204

```
it's using NRF for comms, why not try and use an NRF RX with this remote ?
```

---
## \#7 Posted by: Marksmoura Posted at: 2019-01-28T11:44:04.815Z Reads: 192

```
I have one I can connect to an arduino and try to establish a connection. I'm not sure if they encript the communication but I will soon find out :D hopefully
```

---
## \#8 Posted by: Marksmoura Posted at: 2019-01-29T16:18:47.059Z Reads: 134

```
After searching about the Nrf I found they have an address or pipe which is used to communicate. If I don't know which Address it is then I will also never be able to read the packets from the remote
```

---
## \#9 Posted by: pat.speed Posted at: 2019-01-29T19:52:44.918Z Reads: 105

```
Are you able to find out the address? I’m sure there would be a way to do it
```

---
## \#10 Posted by: Mich21050 Posted at: 2019-01-29T19:53:54.296Z Reads: 99

```
Are you able to get me one shipped to Austria? :slight_smile:
```

---
## \#11 Posted by: pat.speed Posted at: 2019-01-29T19:55:48.212Z Reads: 95

```
May I ask are you an ee? I’ve just seen you designing lots of cool shit recently
```

---
## \#12 Posted by: brenternet Posted at: 2019-01-29T19:56:01.264Z Reads: 97

```
Thought about contacting the maker and just outright asking for a receiver? Might be receptive and a WHOLE lot easier.

Tell them there's a huge market here for them
```

---
## \#13 Posted by: Mich21050 Posted at: 2019-01-29T19:57:06.240Z Reads: 95

```
Currently learning to become one :slight_smile:. 

[quote="pat.speed, post:11, topic:82361, full:true"]
May I ask are you an ee? I’ve just seen you designing lots of cool shit recently
[/quote]
Thank you. :smile:
Hoping that I can do something cool with that remote
```

---
## \#14 Posted by: Mich21050 Posted at: 2019-01-29T20:33:47.801Z Reads: 90

```
![Inked33198391e0826e70388a3c5bb78400c3d5f409fc_LI|375x500](upload://1EbvPIYb3G1MPaROckDn8Itbt3f.jpeg) 
In my opinion, this could be some kind of programming/flashing port but I need to see the PCB to be sure and which pad is which pin :slight_smile:
```

---
## \#15 Posted by: pat.speed Posted at: 2019-01-29T20:49:42.154Z Reads: 83

```
The Chinese ESCs have similar things all over but aparrantly they are locked so we can’t assess it
```

---
## \#16 Posted by: Mich21050 Posted at: 2019-01-29T20:50:22.399Z Reads: 83

```
Ohh ok. I would still like to take a look at one :slightly_smiling_face:
```

---
## \#17 Posted by: sunnyD Posted at: 2019-01-29T20:53:00.104Z Reads: 81

```
How would one purchase this for themselves?
```

---
## \#18 Posted by: pat.speed Posted at: 2019-01-29T21:02:29.784Z Reads: 79

```
Hmm that chip on back is actually a voltage reg, idk if this even has a micro controller, I can’t see one
```

---
## \#19 Posted by: Mich21050 Posted at: 2019-01-29T21:30:21.244Z Reads: 76

```
Yeah but on the front it got something called spmc65sf112a which looks like a microcontroller to me but I can't really find a datasheet online :slight_smile:
```

---
## \#20 Posted by: pat.speed Posted at: 2019-01-29T21:49:40.976Z Reads: 74

```
I googled it and all I got were 72v regulators so idk 😐
```

---
## \#21 Posted by: Mich21050 Posted at: 2019-01-29T21:57:46.316Z Reads: 73

```
I just saw this and it's related to an esc so..
https://endless-sphere.com/forums/viewtopic.php?t=31519
@Marksmoura can you get me one? :slight_smile:
Or maybe ignore the existing cheap and fit an attiny or something like that inside
```

---
## \#22 Posted by: Marksmoura Posted at: 2019-01-30T09:58:21.063Z Reads: 62

```
The Chinese lock everything up so no one can use or copy it. They also make it so we use their Esc. My ideia, because the remote has lots of space would be to unsolder that microcontroller and try to fit an arduino Mini Pro inside, the remote has lots of space, I could just glue it and connect it with wires to the main pcb.

Two days ago I figure out that one P series from My battery died and it is at 0V so the following weeks I must work on repair it first so I can ride again and when I have time again I get back to the remote.

I don't speak Chinese and I'm not sure if that is the supplier, just a shopping selling the remote. 
If you guys want you can try to contact him. For the price and quality it seems that it could be the cheapest and best remote around. 
Here is the link guys:
【无线智能遥控电动滑板车遥控器 电动小鱼板遥控器 电动长板遥控器】https://m.tb.cn/h.3GxzgNe?sm=b77f3b 点击链接，再选择浏览器咑閞；或復·制这段描述￥jI0wbHXFBp8￥后到👉淘♂寳♀👈
```

---
## \#23 Posted by: linsus Posted at: 2019-01-30T10:16:49.076Z Reads: 54

```
I recognize the name of that NRF module. Vedder has been playing alot over the years with these chips, both fresh ones and china ones. Try check out his forums if you can find any help. Maybe you can use some of his code for his custom NRF remote, it uses an STM however, not arduino based.
```

---
