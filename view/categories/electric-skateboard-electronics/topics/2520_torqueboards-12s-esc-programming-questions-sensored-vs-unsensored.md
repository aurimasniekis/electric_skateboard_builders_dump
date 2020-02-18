# Torqueboards 12s ESC Programming Questions - Sensored vs. Unsensored

### Replies: 19 Views: 2009

## \#1 Posted by: Mobutusan Posted at: 2016-04-22T20:42:24.340Z Reads: 202

```
I just picked up two used TB 12s ESC's, one sensored and one unsensored, from a fellow member, and I'm having trouble figuring out how to program the sensored one using the TB programming card. 

Is there some trick to programming the sensored esc, or get it to connect to the programming card? I was trying to use the bec from the non-sensored esc (powered by it's own batteries) to provide power to the programming card since the unsensored unit doesn't have its own BEC yet, but I can't seem to get the sensored esc to connect to the card and display the menus. I got the non-sensored esc to work with the programming card easily, using the same BEC, so I'm a little baffled by the sensored one. If it makes a difference, I don't have a sensored motor or sensor wires, so I'm just trying to get the sensored esc to run unsensored, and access the programming functions. Also, the sensored ESC works fine all wired up and using the BEC to provide power to the receiver, so I know it's functioning properly and the little LED lights work. I just can't program it.
```

---
## \#2 Posted by: torqueboards Posted at: 2016-04-22T21:55:28.755Z Reads: 191

```
@Mobutusan - You might need to flash it.. I'll post something a bit later.
```

---
## \#3 Posted by: Mobutusan Posted at: 2016-04-22T22:07:38.555Z Reads: 187

```
Awesome! Thanks for the help.
```

---
## \#4 Posted by: Mobutusan Posted at: 2016-04-23T15:05:06.803Z Reads: 163

```
Help me, TB-wan. You're my only hope...

:end transmission:
```

---
## \#5 Posted by: Mobutusan Posted at: 2016-04-25T20:28:19.112Z Reads: 148

```
So, @Namasaki was kind enough to link me to the esc software and help me figure out how to access the settings through the pc. So, I've confirmed that the sensored esc functions properly except for the fact that it won't display the settings on the programming card LCD display.

It looks like I have older firmware on both the sensored and uncensored esc's. 

@torqueboards Can you answer these questions for me? 
1. Is v1.00_150818 the current version of firmware and should I upgrade to this version?
2. Is this firmware compatible with both the sensored and unsensored esc's, or is there another version that is?

Thanks!
```

---
## \#6 Posted by: Mobutusan Posted at: 2016-04-27T01:56:41.669Z Reads: 133

```
Bump for confirmation?
```

---
## \#7 Posted by: Namasaki Posted at: 2016-04-30T02:39:29.022Z Reads: 126

```
Did you ever find out about firmware compatibility?
```

---
## \#8 Posted by: Mobutusan Posted at: 2016-04-30T03:28:53.382Z Reads: 127

```
Not yet. I emailed Dexter, and hope to hear back soon.
```

---
## \#9 Posted by: b-rad Posted at: 2016-06-13T04:39:37.959Z Reads: 100

```
Im having the same problem with my TB 12s esc. I am trying to program the esc with the programming card and it just gets stuck at one screen. Anyone know what to do?
```

---
## \#10 Posted by: c4Lvin Posted at: 2016-08-27T07:06:29.362Z Reads: 78

```
Any update on this subject? I can't get through the initial version screen on the program card. More electrical problems.
```

---
## \#11 Posted by: torqueboards Posted at: 2016-08-27T07:14:57.395Z Reads: 76

```
Which ones are you guys using? SBEC or OPTO?

SBEC - middle 3pin on the back of the esc card + power.
OPTO - middle 3pin for the short programming wire. right side 3pin is for UBEC power.

Short wire = programming wire
Long wire = esc signal wire
```

---
## \#12 Posted by: c4Lvin Posted at: 2016-08-27T07:57:32.486Z Reads: 71

```
maybe i'm too tired, but can you tell from this picture attached @torqueboards

<img src="/uploads/db1493/original/2X/b/b2be22cca197b8c6ebeb951bae1025e3d4e57165.jpg" width="281" height="500">
```

---
## \#13 Posted by: Mobutusan Posted at: 2016-08-27T08:04:25.033Z Reads: 67

```
Looks like the opto to me. Try flipping your esc programming wire plug and bec plug and then power it up. Here's a pic of my esc all plugged in.
<img src="/uploads/db1493/original/2X/0/0ce5c7b581e538ea836604b363a7361c7fedb07e.jpg" width="281" height="500">
```

---
## \#14 Posted by: torqueboards Posted at: 2016-08-27T08:06:29.700Z Reads: 64

```
Yeah @mobutusan is right. :grin:
```

---
## \#15 Posted by: c4Lvin Posted at: 2016-08-27T08:20:03.514Z Reads: 64

```
Will do it first thing in the morning guys. I think I tried the bec reverse way as well but there's just no power. Should I have my escs  power plug into my 10S pack?
```

---
## \#16 Posted by: Mobutusan Posted at: 2016-08-27T08:26:07.417Z Reads: 62

```
@c4Lvin Plug in the shorter programming wire and bec like in my picture and make sure the red wire on the bec is plugged into the middle pin. Leave the longer receiver wire unplugged and after it's all set up, then plug in the battery to the esc power cable. I think that's the magic combo. @torqueboards, do you agree?
```

---
## \#17 Posted by: c4Lvin Posted at: 2016-08-27T08:28:55.661Z Reads: 64

```
I'm getting out of bed just to try it out! Be back in a few
```

---
## \#18 Posted by: c4Lvin Posted at: 2016-08-27T08:44:10.451Z Reads: 64

```
Holy mother of all! It worked! I could have sworn that I had the program wire where the black is towards the left side looking from the top front view. As you can see I am just using 4 AAs to power it. <img src="/uploads/db1493/original/2X/c/cfaa31c9a990077c30083defad4b44cfc546ad44.jpg" width="690" height="388">

@Mobutusan is your BEC reversed?  You're display is on because your mini USB is plugged into your PC no?
```

---
## \#19 Posted by: Mobutusan Posted at: 2016-08-27T20:56:48.056Z Reads: 54

```
@c4Lvin Yay! Glad it worked for you. I think your bec plug is reversed/flipped since the color sequence of wires in the connector should go white, red, black from left to right when looking at the screen. The red is the power wire which is always on the middle pin, but I guess maybe it doesn't matter which side the black wire goes from the bec since you were able to power up the card anyway. The card is plugged into the pc in my pic, but it still needs power from the bec to turn the card on.
```

---
