# What VESC to get?

### Replies: 15 Views: 2676

## \#1 Posted by: Thanorak Posted at: 2018-04-20T18:11:32.554Z Reads: 195

```
So I have most of the parts to my eboard picked out, except for one very important part: the VESC.  My board will be running a 10s4p from 30q, with a single 190kv motor, which according to [this esk8 calculator](http://calc.esk8.today/config/?type=3.6&scells=10&pcells=4&cc=3&da=50&mda=100&kv=190&poles=14&eff=85&wheel=97&mp=13&wp=35&wpm=18), should give me roughly 50k eRPM, which I thought would be fine on a 4.12 VESC, so I decided to get the Torqueboards VESC.  However, after some more research, I saw that there were a lot of people who blew their TB VESC while running a pretty similar setup to me.  I am a college student, and I'm trying to keep costs pretty low.  Do you guys think the TB 4.12 would be sufficient, or would I have to get a different 4.12 or step it up to a FOCBOX or VESC 6?  Or could I just deal with a decent quality ESC.  Any help is appreciated
```

---
## \#2 Posted by: rey8801 Posted at: 2018-04-20T18:18:26.283Z Reads: 190

```
Do you wanna run it in FOC?
```

---
## \#3 Posted by: Thanorak Posted at: 2018-04-20T18:21:46.768Z Reads: 180

```
Most likely BLDC, since I've heard its easier on 4.12.  However I could be wrong about this as I have no experience.
```

---
## \#4 Posted by: rey8801 Posted at: 2018-04-20T18:32:25.421Z Reads: 171

```
It's correct. If you are not interested in FOC then you can also look to Torqueboard vesc, meytech and save some money. Also hobbyKing's vesc will work. Although I see you are going with a 10s 4p 30q which cost you money and can deliver 80A continuously. With the previous mentioned vesc you better set the battery max to 30A and you can understand that it's way lower your real potential. So to me either you move to dual and then two TV, meytech vesc will use 60A.pr you stick with one and you set it to 30A still powerful and great range with 4p or you invest a little more money and go with Focbox or even better vesc6 and use more of your board potential.
```

---
## \#5 Posted by: Namasaki Posted at: 2018-04-20T18:32:38.797Z Reads: 159

```
Running BLDC will reduce the risk of problems. 
And simplify the setup if your using BLDC tool to set it up
```

---
## \#6 Posted by: Thanorak Posted at: 2018-04-20T18:39:57.032Z Reads: 152

```
The TB VESC is rated for 50A continuous, are you saying to limit it to 30 to reduce risk of damaginf the VESC?  Also, If I understand how this works correctly, limiting the current through the motor would affect only my acceleration (but not braking?), not top speed, and will probably slightly increase range
```

---
## \#7 Posted by: PredatorBoards Posted at: 2018-04-20T18:52:10.191Z Reads: 143

```
I feel like everyone completely forgot about Vanda...

https://www.electric-skateboard.builders/t/new-vesc-from-china-seems-like-not-only-maytech-is-making-vescs-now/5207/42?u=predatorboards
```

---
## \#8 Posted by: Thanorak Posted at: 2018-04-20T18:56:54.655Z Reads: 130

```
Wow, thanks!  I've only looked into it for about 5 minutes, but from what I've seen so far that looks pretty nice, I'm surprised I haven't seen it before.  If I do end up going with 4.12, I'll definitely look more into that
```

---
## \#9 Posted by: PredatorBoards Posted at: 2018-04-20T19:02:07.556Z Reads: 126

```
Cool. Just remember the Vanda was built to Vedder's original 4.12 specifications. This means it won't  run FOC reliably.
```

---
## \#10 Posted by: Thanorak Posted at: 2018-04-20T19:06:04.331Z Reads: 126

```
Fine with me, I think I'll be perfectly ok with  BLDC
```

---
## \#11 Posted by: rey8801 Posted at: 2018-04-20T19:21:01.789Z Reads: 117

```
You right. And yes I forgot about it :joy: the thing that we still need the brave guy that tries it for the science.
```

---
## \#12 Posted by: rey8801 Posted at: 2018-04-20T19:22:22.226Z Reads: 114

```
Yes they are rated 50A but for instance for Maytech it way easier to burn it at that Amp.
```

---
## \#13 Posted by: Thanorak Posted at: 2018-04-20T20:01:52.663Z Reads: 106

```
Ok, I'll keep that in mind if I do end up going with the 4.12
```

---
## \#14 Posted by: zeno Posted at: 2018-04-20T20:57:41.915Z Reads: 100

```
I just received my vanda vesc last week.. from the looks of it it is really high quality work! :) Hope it will prove to be as reliable as it looks :)
```

---
## \#15 Posted by: trampa Posted at: 2018-04-20T21:38:51.620Z Reads: 98

```
A HW 4.12 is rated 30A continuous without additional cooling of the PCB. Benjamin has a video on his YouTube channel, comparing the VESC 6 to a VESC 4. 

https://www.youtube.com/watch?v=1iwN5LGGM80

If you run low KV motors, keeping the erpm quite low, FOC should work reasonable well on a good quality HW 4.12 made to original spec, BOM and pcb manufacturing to top level standards.
The slower the motor spins, the easier it is to track the rotor position. HW4 is a bit limited in precision tracking the rotor position, since it uses 2 shunts only. All HW 4 based ESCs lack ultimate precision when it comes to FOC, especially on speedy motors. This is a design limitation which was leading Benjamin to re-think the entire ESC layout. Unfortunately a lot of coding was needed to allow VESC 6 hitting the market.

Voltage would be best at 12S, limiting the Amp flow as much as possible. 

@PredatorBoards: THX for sharing the link with the microscope images. Very enlightening... 2x "Same" product but obviously worlds apart in quality. Gives people an idea how much PCB/Product quality can vary and why newbies still need a good portion of luck to get a reliable device deliver when they buy from a random source. The spread in quality is astronomic!

https://www.electric-skateboard.builders/t/new-vesc-from-china-seems-like-not-only-maytech-is-making-vescs-now/5207/42?u=trampa  

A good sign is always buying from a source offering a full product warranty. If you get no proper warranty or you have to pay extra for a standard term warranty something is funny...  If you trust the products you sell, you can give full warranty, knowing that you won't see the same device twice in your life anyway.
```

---
