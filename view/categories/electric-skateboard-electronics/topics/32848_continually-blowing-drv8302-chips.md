# Continually blowing DRV8302 Chips

### Replies: 17 Views: 950

## \#1 Posted by: dkornfeld Posted at: 2017-09-11T07:29:38.935Z Reads: 208

```
Hey everyone, 

I have had issues with VESCs bought from torqueboards. For whatever reason, I keep seeming to blow the DRV8302 chip within hours of opening the bags. I am using a custom built lithium ion 10S 6P pack and it seems to be outputting nominal voltage the whole time. I use torqueboards 6355 190KV Motors, so I wouldn't imagine that backEMF is what could be killing the chip. 

Luckily, Dexter seems to have been understanding and has agreed to replace these VESCs, but three have already been killed, and the settings have all been well within the safe operating limits. 50A motor current, 50k ERPM limits, current ramp is properly set to 0.04. 

This issue has happened both in FOC and BLDC mode. I have been using BLDC tool instead of VESC tool, so maybe that's causing issues? There are no burn marks or holes in or around the DRV8302 chip, so I have no idea what actually went wrong. 

I am receiving my replacements from Dexter later this week, and I do not want them to blow again. Any help from anyone would be appreciated, as this board just seems to suck more and more money. 

Thanks!
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-09-11T09:11:42.614Z Reads: 201

```
tell us what setup you have, which motor and so on.
Then post screenshots or your vesc settings.

Sometimes it´s just a faulty motor, sometimes it´s a bad setting somewhere hidden in the bldc tool ;)
```

---
## \#3 Posted by: Deckoz Posted at: 2017-09-11T14:06:47.054Z Reads: 170

```
Well atleast dexter is replacing them for you

I've gone through three and they've made no such offer, and dont allow warranty purchases afterwards.

Two of mine have gone in FOC and one in Hybrid on his 6355 motors

I'm running 10s, and my settings are very moderate, 

30a motor max 
-30motor min
30 battery max
-12battery min.

Again atleast he's offering to replace yours. My first one died after 293 miles, the second one died after 26 miles(repurchased one to replace the first), third one(one of the original pair) died 157 miles after that. I would have been happy if they replaced them, or even allowed warranty purchase as this has all happened since august 2nd. Yea that's right 3 vesc in less then a month. $360 in paper weights. Lol

@torqueboards what say you for keeping your PCBs from dying? Because I'm obviously not the only one, and I run more modest settings then the OP.
```

---
## \#4 Posted by: dkornfeld Posted at: 2017-09-11T17:08:37.448Z Reads: 142

```
I have already explained the full setup. Additionally, I have had this happen with multiple motors, so I don't think it's a defective motor problem. What "bad setting" would you be looking out for in BLDC tool?
```

---
## \#5 Posted by: dkornfeld Posted at: 2017-09-11T17:09:49.325Z Reads: 139

```
All of mine have died in one mile or less, one didn't even make it off the testbench.
```

---
## \#6 Posted by: Deckoz Posted at: 2017-09-11T17:29:33.248Z Reads: 134

```
One mile...or 26 miles(that's one charge on my board). There's something wrong with them. I'd like to know why as well, because as I stated my settings are even more moderate then yours, and they all have gone poof. Especially since you have the same motors I do, are on 10s like me and using the same vescs
```

---
## \#7 Posted by: Alanhunt123 Posted at: 2017-09-11T19:59:54.033Z Reads: 123

```
Make sure you are taping over each of your bullet connectors to the motors. I had a board running solidly for a few months, and as soon as I took the tape off, my board was fried within a few hours of riding.

Good luck!
```

---
## \#8 Posted by: dkornfeld Posted at: 2017-09-11T20:16:28.083Z Reads: 116

```
All my connectors were taped.
```

---
## \#9 Posted by: TarzanHBK Posted at: 2017-09-11T21:22:58.982Z Reads: 107

```
Sorry didn´t see that.
Could be a lot to mess up ;)
Just post some screenshots and let me or other people take a look
```

---
## \#10 Posted by: danielz Posted at: 2017-09-11T22:20:47.435Z Reads: 100

```
Maybe try using addition low esr caps on top of the ones already there? How long are your battery to vesc cables?
```

---
## \#11 Posted by: dkornfeld Posted at: 2017-09-11T22:53:27.305Z Reads: 97

```
Probably 10" or shorter. They're in the same compartment, not separated. My battery goes through a fuse into a solid-state relay into the VESC.
```

---
## \#12 Posted by: danielz Posted at: 2017-09-12T00:12:15.305Z Reads: 97

```
That is quite long, are they cable tied together? There doesn't seem to be a conclusive answer to why some ppl burn so many out, and others none. I assume it must be something to do with individual setups, otherwise the seller would of had to stop selling them by now. 

I know of only one guys who failed whilst hooked up to an oscilloscope. He noticed a lot of noise, which overwhelmed some diode, with killed the buck then the in turn the drv. But that might not necessarily be the same problem as you are having.
http://vedder.se/forums/viewtopic.php?f=7&t=145&start=30
```

---
## \#13 Posted by: dkornfeld Posted at: 2017-09-12T03:17:04.871Z Reads: 90

```
My DRV doesn't look like that though. It hardly looks touched. It looks completely normal. Also, do you mean noise on the power line?
```

---
## \#14 Posted by: Deckoz Posted at: 2017-09-12T03:22:19.416Z Reads: 90

```
@danielz thats how my first one blew, D4 and D5 and L1, went first
 <img src="/uploads/db1493/original/3X/7/5/75b4dca80c0a4a39e63c68d02896442003ac02d7.jpg" width="374" height="499">
```

---
## \#15 Posted by: dkornfeld Posted at: 2017-09-12T03:51:45.359Z Reads: 84

```
I plan on shortening my battery cables once I get my new VESCs in. What other fixes have people said helped? Do the VESCs from @torqueboards come with the C18 mod?
```

---
## \#16 Posted by: crustyxpunk Posted at: 2017-09-12T09:58:26.369Z Reads: 73

```
I had one Torque Boards VESC blow out after less than a mile as well. It was my first build and could definitely have been something I did wrong. I sent a message to the guys at Torque Boards with some screen shots of my settings in BLDC tool. Dexter sent me an email back saying to send them my old VESC and they would send me a new one. Which is really nice IMO! 

I can see them not replacing your VESC after more than a 100 miles. They do offer a warranty that you should have purchased after the first one blew. 

I can post my settings if you guys would like.
```

---
## \#17 Posted by: Saikdog Posted at: 2017-11-02T16:49:40.932Z Reads: 49

```
Internal motor shorts?
```

---
