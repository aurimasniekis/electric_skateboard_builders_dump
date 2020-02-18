# A little confused

### Replies: 15 Views: 669

## \#1 Posted by: Jayallday Posted at: 2017-07-29T23:55:47.583Z Reads: 101

```
Hi everyone! So I have done quite a bit of reading but I am not confident enough to pull the trigger so to speak. 

Basically I have various "scrap" components laying around from Chinese brand ewheelin. I've enclosed a pic of the battery because my question is can I run 2 of them in series to a 500 watt hub? Will that increase the power to the board?<img src="/uploads/db1493/original/3X/4/d/4dd1e801cf318e9c741e2b234b44d2db86499967.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/b/8/b8e396222fc4440b93ce85ec80d11ffdda14031d.jpg" width="375" height="500">
```

---
## \#2 Posted by: Guacamoleface Posted at: 2017-07-30T00:00:31.321Z Reads: 89

```
the one thing I'd guess that would be concerning is the Amp rate the batteries are able to put out. I know the e-bike battery I have has very low discharge rate. I doubt this but Is there not any information on what kind of cells are used in it?

also just checking -  do you mean in serial or paralell? I assume u want the parallel as the serial connection would double the voltage instead.
```

---
## \#3 Posted by: MrHappy Posted at: 2017-07-30T00:30:59.240Z Reads: 81

```
That is a 7s battery i believe, Do not do series. 25.2/3.7 =(ish) 6.9
Wire them up with both positive/negative terminals together to make a parallel pack.
7s2p
```

---
## \#4 Posted by: Cobber Posted at: 2017-07-30T00:33:23.654Z Reads: 77

```
Series will go faster, Parallel will go for longer.
I think OP wants to go faster.
I don't know what will happen, from the experience of others on the board increasing voltage often the (v)esc can be the limiting factor so you will need to also understand the specs of that as well to make a informed judgement. Finally a circuit designed for 25.2v run at 50.4v will need the appropriate wiring and connections...
So keep learning bro before you bbq your scoot.
```

---
## \#5 Posted by: MrHappy Posted at: 2017-07-30T00:36:40.950Z Reads: 71

```
Please link me to a 50.4V (14s) ESC. 
Do not put them in series, you will explode your speed controller.
```

---
## \#6 Posted by: Cobber Posted at: 2017-07-30T00:41:58.446Z Reads: 60

```
I have a pair of Scorpion Commanders that are rated at 59v or 14s, why so @MrHappy I do not think the OP wants to spring for new hardware.
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2017-07-30T00:48:21.735Z Reads: 57

```
[quote="Cobber, post:6, topic:29084"]
Scorpion Commanders
[/quote]

those scorpion commanders are sikkkkkk just checked em out!
```

---
## \#8 Posted by: Cobber Posted at: 2017-07-30T00:59:08.242Z Reads: 55

```
Yeah @trancejunkiexxl I think they are pretty sweet. They have a YGE cap bank on the front and come wired with a extra anti-spark wire on the positive. 
We shouldn't de-rail @Jayallday's thread though. I'm not really sure why or how we ended up here? Maybe @MrHappy will pull it all together for us :smiley:
```

---
## \#9 Posted by: trancejunkiexxl Posted at: 2017-07-30T01:00:47.205Z Reads: 55

```
wow just realized that,, im sorry dudes i get a little excited
```

---
## \#10 Posted by: MrHappy Posted at: 2017-07-30T01:55:01.004Z Reads: 52

```
You won't be getting any more speed, but you'll get quite a bit more range by hooking them in parallel.
```

---
## \#11 Posted by: Jayallday Posted at: 2017-07-30T02:11:12.557Z Reads: 46

```
I can definitely spring for new hardware. I'm just a tinkerer by nature. These parts all came from some shenzen specials...😂 I wanted to see how fast I could make the board go
```

---
## \#12 Posted by: Jayallday Posted at: 2017-07-30T02:15:03.552Z Reads: 43

```
Thanks for the replies yall. The parts that cropped out with the quickness. Funny thing is that no single one stopped working because of the same reason I figure ill play Dr Frankenstein or...🤔.. Dr. Skatinstein ba dum dum chhhhh!!!
```

---
## \#13 Posted by: Cobber Posted at: 2017-07-30T03:04:34.328Z Reads: 36

```
Hi @Jayallday, Having a quick look at your history: you bought a eSk8 from ebay, then one from target? The first one cooked, the second is one of those AT boards with a heap of lead acid batteries in them that weigh >30kg?
The batteries you bought are good if what it says on the outside is on the inside: 18650 battery cells. The difficult thing is they are in what appears to be a 7s configuration. How many do you have? If you put 4-6 together in parallel you will have a half decent battery pack. How many depends on the rest of your drive system.
Going in series isn't impossible but there are not many 14s options out there for your esc and you will be more on your own and spending a lot more coin on hardware.

The obvious thing I think would be to ditch the lead acid batteries in your X cross for the 18650 cells you have. The problem then is the X cross is 36v (? need to check that) and your 18650 packs are 29.4. So if you dont change the gearing or the motor it will be slower. So there is no easy answer unfortunately.
It is likely you could have built a good diy board with what you have spent.

A solution to use what you have could be to pull apart your scooter packs and re-configure the cells to say 10s to use in your border cross. Search out building [18650 battery pack](http://www.electric-skateboard.builders/search?q=18650%20battery%20pack) on the forum.
Or you could use them as is to build a 7s board, there are lots of cheap reliable esc's at that voltage.
```

---
## \#14 Posted by: Jayallday Posted at: 2017-07-30T03:19:00.320Z Reads: 35

```
Yes you would be correct. The first "electric skateboard I bought was a blitzart from EBay. This was before I realized what kind of quality products where available. Lol. That one just apparently stopped connecting via Bluetooth. In between this time I ordered 2 Maverix border cross boards. They both currently work perfectly, but they weigh like 70 pounds each. I received a replacement for the Blitzart. Garbage as well. Then I bought a similar one for $22.I was just learning about this forum at that time and almost obsessively lurked in various threads. Unfortunately I am not very mechanically inclined so it's taking some time to get a full grasp of the DIY options. In the meantime I purchased a EMTB and a Koowheel to ride. I realize that this was a foolish decision as I could have possibly built an eskate of my own that is completely tailored to what I am looking for in a board.
```

---
## \#15 Posted by: Jayallday Posted at: 2017-07-30T03:22:01.369Z Reads: 29

```
in my ramblings I didn't answer your question. I have 3 of those batteries
```

---
