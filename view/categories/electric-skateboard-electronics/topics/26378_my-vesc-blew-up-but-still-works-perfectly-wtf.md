# My vesc blew up but still works perfectly. WTF?

### Replies: 22 Views: 1892

## \#1 Posted by: NAF Posted at: 2017-06-29T06:03:49.569Z Reads: 261

```
Ok so a I ve noticed that from time to time i ve started loosing connection and I thought it was my remote. It happened maybe like twice in the past five days. Today i've taken off shrink foil from my vesc and I saw that c51 blew up comletely. 

<img src="/uploads/db1493/original/3X/5/4/5400e4f2d1745e7660c94c210c46442bb6321f60.JPG" width="375" height="500">



Whats really weird is that the vesc is still full functinal:

- drv chip is ok and intact
- bldc tool gives no errors
- the lights on the bootup blink three times and show no error
- motor detection works
- motor spins

Big question is what should I do. The vesc is under the warranty but Ill have to send it back to US. I was just wondering if I could just replace C51 with new one ? will that be enough to get fully functional vesc?

From what I know the capacitor on this vesc is the upgraded 22uf 100v cap.

http://pl.mouser.com/Search/ProductDetail.aspx?R=CKG57NX7S2A226M500JJvirtualkey52130000virtualkey810-CKG57NX7S2A226JJ
```

---
## \#2 Posted by: wmj259 Posted at: 2017-06-29T06:39:28.871Z Reads: 251

```
I would first ask your vendor if you do this repair yourself if it will void the warranty. 

Next check it you still see the silver solder patch on both ends of the spot on the VESC itself or if that's ripped off. If it's ripped off I would send it back for warranty. If it's still there then you can proceed with replacing it. 
You will need a soldering iron and Flux and solder. 

What version VESC is that? If you flip it over in the board it will say Vedder.se with a 4.##
```

---
## \#3 Posted by: NAF Posted at: 2017-06-29T06:43:25.805Z Reads: 243

```
This is 4.12 version.
```

---
## \#4 Posted by: wmj259 Posted at: 2017-06-29T06:44:42.206Z Reads: 236

```
Also if this is using hardware 4.12 then c51 capacitor is a 15 microfarad. 
<img src="/uploads/db1493/original/3X/0/6/0627898389c39d4ef6cf18370463cb6808e2fea9.png" width="690" height="388">

If someone else can chime in. From. What I read, replacing a capacitor with a slightly larger one won't make a difference, neither with voltage but never go down. Also size maybe a factor to be careful of.
```

---
## \#5 Posted by: NAF Posted at: 2017-06-29T07:16:47.884Z Reads: 214

```
Yes usually it is 15uf 100v but this vesc had upgraded components and they have used 22uf 100v which is double stacked capacitor.
```

---
## \#6 Posted by: NAF Posted at: 2017-06-29T09:05:46.050Z Reads: 196

```
Damn I just have noticed that L1 cap seems to be broken.

<img src="/uploads/db1493/original/3X/c/7/c73884f1bfb861138bc21445eee1fcfde085eced.JPG" width="375" height="500">

@wmj259 can you tell me whats the part number for L1 component?
```

---
## \#7 Posted by: NAF Posted at: 2017-06-29T11:00:16.894Z Reads: 180

```
Guys can anyone tell me what's the difference between: CKG57NX7S2A226M500JJ and CKG57NX7S2A226M500JH and which one should I get ? They are both 22uh 100v and have exactly the same specs. Maybe @onloop @chaka @zmoney or especially @JTAG as it is his upgrade could chime in.


<img src="/uploads/db1493/original/2X/8/812dbf61563b957bc14c68a34029d0ad3c53f14a.jpg" width="690" height="442"><img src="/uploads/db1493/original/3X/e/a/ea056488cadbeb437f7a3846a0f229439466015a.png" width="690" height="277"><img src="/uploads/db1493/original/3X/0/d/0de2f673b57ecdb3112ff29c71ca61d02e545681.png" width="690" height="291">
```

---
## \#8 Posted by: JTAG Posted at: 2017-06-29T11:24:05.772Z Reads: 165

```
Both are just fine. The last letter stands for: "Special reserved code" probably some batch or source identification, nothing we should care about :smile:.
```

---
## \#9 Posted by: NAF Posted at: 2017-06-29T11:27:59.260Z Reads: 164

```
@JTAG THanks a lot !!! Do you think I should be fine if I replace C51 considering the fact that the VESC is still fully functional ??? Also do you think I should replace L1 as it has chipped off a little bit ??
```

---
## \#10 Posted by: wmj259 Posted at: 2017-06-29T15:40:39.005Z Reads: 143

```
L1 is a power inductor. 
<img src="/uploads/db1493/original/3X/4/e/4e1cf1c2b2a0694924b2d2a7c6601d2b16f85fea.png" width="690" height="388">
It's seems like your vesc has been rattling around.
```

---
## \#11 Posted by: NAF Posted at: 2017-06-29T15:43:08.313Z Reads: 135

```
Thanks. I just have ordered both c51 and L1 and found a guy who can do the soldering. I am only wondering if I should replace L1 or I can leave it like that with that chipped off part.
```

---
## \#12 Posted by: wmj259 Posted at: 2017-06-29T15:48:29.911Z Reads: 137

```
While your at it, I would order some extra capacitors. In case anything breaks off in the future. Shipping is cheap but prices also decreases with more you order quite significantly.
```

---
## \#13 Posted by: NAF Posted at: 2017-07-03T15:01:37.805Z Reads: 104

```
Today all my missing parts just arrived C51 and L1 - I already gave them to the guy who is going to do the soldering for me. I'll let you guys know if it all works. But if works it will only show that repairing your VESC's without actually having any electronics/soldering skills is still possible ;) :slight_smile:
```

---
## \#14 Posted by: NAF Posted at: 2017-07-03T17:44:11.838Z Reads: 96

```
WOW that was quick. I just picked up my vesc. C51 and L1 nicly replaced.

<img src="/uploads/db1493/original/3X/b/6/b6fd699245ba2b56e04441eb966b22ba28ac691d.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/f/a/fa811cbb2b1041bb1b15f85ac350091fada5c11c.JPG" width="375" height="500">




So on the whole it took me three working days to order the parts and get them replaced. Nice!! Ive paid around 20usd for soldering and about 15usd for the parts with shipping. Not bad at all considering the fact it was all done in three days. 

By the way i ve talked to the guy about replacing DRV in the future just in case bad things happen. He said no biggie for him. So if anyone needs vesc repair services here in europe just let me know and i will contact you with this guy.

Now its time to test the vesc and see if it all works.
```

---
## \#15 Posted by: JdogAwesome Posted at: 2017-07-03T18:57:02.975Z Reads: 83

```
Thats a shockingly fast repair lol. Its great that you got it repaired in all, but just keep an eye out for what actually caused the problem in case it happens again. You dont just want to repair something if its going to keep breaking, kinda like if you replaced a bike wheel cause it popped riding on a bed of nails, then continued to ride on the same bed of nails.
```

---
## \#16 Posted by: NAF Posted at: 2017-07-03T19:09:27.310Z Reads: 84

```
Hey. It was the first failure that ever happened so it is not like I am repairing it every week. The thing is C51 blew up as well as L1. Of course it might have been caused by the FOC ..but I have really hard time believing it..as the battery is 10s and not 12s ..and the motor is 85kv only. So I really doubt it was that. And besides that the VESC was upgraded with components that can handle a lot more and I know other people are actually using this vesc for FOC without any issues. 
I suspect it might have been caused by my battery ...as I remember little PUFF when I was disconnecting my battery in the way I wasn't supposed to.
```

---
## \#17 Posted by: NAF Posted at: 2017-07-06T20:04:05.907Z Reads: 71

```
UPDATE: after my VESC repair I just had a chance to try everything on a longer distance. I did **7miles** hitting max **24mph**. All in FOC MODE. Everything was smooth so I assume that FOC is working fine. I didnt had chance to cut open the vesc to check if anything blew up but Id be surprised if it did. So all in all, my vesc repair mission seems to be successful!

<img src="/uploads/db1493/original/3X/9/c/9cfdce50381b43e1863ba3af5bc741d8742f7c4d.jpg" width="640" height="394"><img src="/uploads/db1493/original/3X/2/0/2021827cf7e86ff22e05eeb5742916fb90b1b1f3.PNG" width="281" height="500">
```

---
## \#18 Posted by: Maxid Posted at: 2017-07-06T20:05:37.439Z Reads: 64

```
you should make a post with his contacts in the VESC directory. People should know!
```

---
## \#19 Posted by: NAF Posted at: 2017-07-06T20:11:34.333Z Reads: 62

```
Sure I'll call him tomorrow and ask for his email. He is based in Poland so if anyone from EUROPE wants to repair something he can easily do it. The guy specializes in soldering precise electronics. Repairing DRV Chips is not a problem for him.
```

---
## \#20 Posted by: NAF Posted at: 2017-07-07T08:29:47.511Z Reads: 50

```
One thing I thought I would ask ...when I am riding ..I think sometimes I hear something ...like little sparks ..I might be wrong ..and maybe my hearing is not right ..but I think the sound is coming from the motor. Is it normal behaviour ? What do I actually hear ? Is it high current going through the motor ??? I dont think it's the vesc making that sound. 
@Maxid Maybe you could help me out here ?
```

---
## \#21 Posted by: Maxid Posted at: 2017-07-07T10:24:41.135Z Reads: 42

```
Without some audio this is hard to tell. No idea what you hear and if it is coming from the motor.
Might just be gravel for all I know
```

---
## \#22 Posted by: solidgeek Posted at: 2017-07-07T10:41:14.378Z Reads: 42

```
Doesn't look like anything actually "brew" up, instead it looks like your VESC isn't probably secured, and therefore has been rattling around in your enclosure as @wmj259 wrote. It looks like the components has been broken off, not blown up :P ?
```

---
