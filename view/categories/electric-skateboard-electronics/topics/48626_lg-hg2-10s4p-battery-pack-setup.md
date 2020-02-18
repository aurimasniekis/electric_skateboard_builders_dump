# LG HG2 10S4P Battery pack setup?

### Replies: 26 Views: 1271

## \#1 Posted by: nikoli280 Posted at: 2018-03-09T18:29:21.183Z Reads: 180

```
Hi Everyone. I have made this schematic to show how i plan to wire up my batteries. 

The pack will be used to draw a absolut max of 60A. Its made into a 10S4P config, So each parrellel pack needs to draw 15A at most

I have bought some 10mm x 0.1mm Nickel wire. and i found through the linked video that the strip could supply around 3.5a-4A at optimal settings. So i thought that if i made the pack with 4 strips on top of each other in a pyramid shape i would get a max draw of 3.5 * 4 = 14-16A 

So my question is does this schematic seem right? i plan on connecting the series connection through a 14AWG silicone wire

 ![lg-h2_1_1|509x500](upload://azaMw4gt6wrCvGeCOS4AYVyAYeF.jpg)
https://www.youtube.com/watch?v=wdZ_Ca_sAZE
```

---
## \#2 Posted by: ZackoryCramer Posted at: 2018-03-09T18:34:09.500Z Reads: 170

```
I would use 12 or 10 guage wires to be sure. 60 is massive amount of current if you can’t tell.
Where are you using the nickel strips anyways? I would use 10mm x .15mm to be sure.
```

---
## \#3 Posted by: nikoli280 Posted at: 2018-03-09T18:49:53.247Z Reads: 164

```
No you are wrong 14AWG is more than enough for 60A. 14Awg can hold up to 55A at a standard 20C temperature. The wire can handle 105C so 20-25C is no problem at all.

I would also use .15mm strips but my spot welder can better handle 0.1
```

---
## \#5 Posted by: ZackoryCramer Posted at: 2018-03-09T20:11:52.718Z Reads: 151

```
@GrecoMan have some 🌶‘s 😃

The schematic seems right if that’s all you are looking for. What’s more important is how you actually layout the cells in a pack. 
You wouldn’t want to lowball your electrical components. In addition, I wouldn’t recommend the pyramid layout on the sides since nickel on nickel doesn’t go so well and they can easily snap if the pack were to bend. 🗿
```

---
## \#6 Posted by: nikoli280 Posted at: 2018-03-09T20:52:26.805Z Reads: 129

```
Hi Im sorry you feel pissed of by my topics. I make topics to gain knowledge, which is a forums main objective in my book.

I just want to correct what you are saying. I will very much like to take advice from you all. But many times people comment on other things that i ask about. Yesterday i asked about which longboard deck to choose, it quickly changed to be about my ABS 3d printed motor mount.
i did not ask for advice on that, so  of courses i will deny it. If people could stay on the asked topic i would have gained the information i needed faster.
```

---
## \#7 Posted by: Lumaci Posted at: 2018-03-10T00:10:03.987Z Reads: 118

```
But you didnt ask about the deck, it says "I would like to hear your thoughts on my second ESK8 build. I have a last decision to make which you can read about in the end"

They gave you feedback on your mount, since you asked for thoughts about the built.
```

---
## \#8 Posted by: PXSS Posted at: 2018-03-10T07:33:09.205Z Reads: 109

```
[quote="nikoli280, post:3, topic:48626"]
No you are wrong 14AWG is more than enough for 60A. 14Awg can hold up to 55A at a standard 20C temperature.
[/quote]
NO. YOU ARE WRONG. 
Go do some real testing and come back after.

[quote="nikoli280, post:1, topic:48626"]
So my question is does this schematic seem right?
[/quote]
No.
```

---
## \#9 Posted by: nikoli280 Posted at: 2018-03-10T08:34:15.553Z Reads: 105

```
60a ratting is what I got from the web, the seller hobbyking and Wikipedia. So why is it wrong? 

And if the schematic is wrong then don't just answer no that does not help me at all
```

---
## \#10 Posted by: pat.speed Posted at: 2018-03-10T10:12:29.985Z Reads: 104

```
That schematic is correct, but the orientation is a little bit wierd
```

---
## \#11 Posted by: nikoli280 Posted at: 2018-03-10T10:16:56.713Z Reads: 97

```
Please tell me what you think  is wierd about the orientation :slight_smile:
```

---
## \#12 Posted by: pat.speed Posted at: 2018-03-10T10:35:05.298Z Reads: 96

```
Just the 4th parallel pack, maybe you are not going to have them connected in that configuration
```

---
## \#13 Posted by: nikoli280 Posted at: 2018-03-10T10:38:18.074Z Reads: 94

```
Ahh okay, yeah i really dont know why i drew it that way but it will not be connected that way, it will be connected in 2 lines across the board.
```

---
## \#14 Posted by: PXSS Posted at: 2018-03-10T13:32:56.139Z Reads: 92

```
[quote="nikoli280, post:9, topic:48626"]
the seller hobbyking
[/quote]
Yes because hobbyking doesn't exaggerate their numbers. EVER. 

[quote="nikoli280, post:9, topic:48626"]
Wikipedia
[/quote]
Did no-one ever teach you not to use Wikipedia as a source if you want to be taken seriously?

[quote="nikoli280, post:9, topic:48626"]
that does not help me at all
[/quote]
I am giving you the same courtesy, you gave others.
```

---
## \#15 Posted by: nikoli280 Posted at: 2018-03-10T13:45:41.109Z Reads: 87

```
Tell me why should i trust you and not 2 independent sources?
```

---
## \#17 Posted by: PXSS Posted at: 2018-03-10T13:49:54.384Z Reads: 93

```
I'm not. 
I said:

[quote="PXSS, post:8, topic:48626"]
Go do some real testing and come back after.
[/quote]

[quote="nikoli280, post:15, topic:48626"]
2 independent sources?
[/quote]
Bahaha.
```

---
## \#18 Posted by: PXSS Posted at: 2018-03-10T13:57:50.849Z Reads: 91

```
Let me teach you how to use proper sources...

![image|357x500](upload://eykGfSMkby250Q8bpxCyNorGCQP.jpeg)
Source: Santa Clause. 

Jk. Source: Handbook of Electronic Tables and Formulas for American Wire Gauge.

---
![image|690x368](upload://mKPsJdxZdBpjsg5nZ5mgpFHp2ow.jpeg)
Source: Mil-Spec ETFE Insulated Electric Wire (MIL-W-22759/16)
```

---
## \#20 Posted by: PXSS Posted at: 2018-03-10T14:18:40.216Z Reads: 82

```
Not even a thank you? Oh well. I proved my point. You figure out the rest. 😂
```

---
## \#21 Posted by: nikoli280 Posted at: 2018-03-10T14:22:57.067Z Reads: 83

```
Im still unsure its correct the internet seems to be filled with loads of diffrent opinions on the amp ratting. So i honerstly dont know anymore
```

---
## \#22 Posted by: GrecoMan Posted at: 2018-03-10T14:27:31.705Z Reads: 85

```
dude @PXSS is speaking from REAL LIFE EXPERIENCE, not random wikipedia pages
```

---
## \#23 Posted by: PXSS Posted at: 2018-03-10T14:27:54.722Z Reads: 85

```
Loooool. 
These are standards for engineering. Not something xXxBrony553 on 4chan/reddit came up with.
```

---
## \#24 Posted by: GrecoMan Posted at: 2018-03-10T16:25:06.557Z Reads: 79

```
lol i guess flagging that is kinda appropriate 🤣
```

---
## \#25 Posted by: ATLesk8 Posted at: 2018-03-11T21:05:32.802Z Reads: 67

```
You're a flag
```

---
## \#27 Posted by: nikoli280 Posted at: 2018-03-11T21:41:13.436Z Reads: 66

```
This thread is out of hands i simply wanted some help, i will flag this for admins to decide.
```

---
## \#28 Posted by: Namasaki Posted at: 2018-03-11T21:44:27.190Z Reads: 65

```
[quote="nikoli280, post:27, topic:48626, full:true"]
This thread is out of hands i simply wanted some help, i will flag this for admins to decide.
[/quote]

I can close it down right now if you like.
```

---
## \#29 Posted by: nikoli280 Posted at: 2018-03-11T21:45:52.628Z Reads: 64

```
I guess that would be better, i dont think i will gain any better advice from this. Just a shame.
```

---
## \#31 Posted by: Namasaki Posted at: 2018-03-11T21:48:31.066Z Reads: 64

```

```

---
