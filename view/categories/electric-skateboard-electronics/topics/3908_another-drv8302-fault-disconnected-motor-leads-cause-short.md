# Another DRV8302 fault - Disconnected motor leads cause short

### Replies: 15 Views: 3455

## \#1 Posted by: treenutter Posted at: 2016-05-27T20:45:04.199Z Reads: 323

```
So I really love this silicone repair tape, has no adhesive on it, it just sorta grips to itself. This is great when I need to tape something up to prevent electrical shorts, but I don't want it to have gummy residue left behind when I remove it. Genius right?

<img src="/uploads/db1493/original/2X/4/425c08949f50016c3b6741a89022b2a08cbedbcf.jpeg" width="375" height="500">

I use this stuff all the time on my motor leads, to keep them connected to the ESC and to keep out grit. About a month ago I did some rewiring in my enclosure and in my haste to get on my board and ride, I taped all three of the motor connections together instead of wrapping each on individually.

We guess what happened? About 2 weeks later, I noticed that VESC was overheating on short rides. That had never happened before, but I chalked it up to some longish downhill rides and the rising outdoor temps. At this point, I had forgotten all about the DUMBEST TAPE JOB MANKIND HAS EVER KNOWN. 

I go for another ride, it's mostly OK but overheats once. I start to wonder if there is a problem with my battery or if VESC needs more cooling in the summer weather. Those FETS were getting really hot to the touch which is not good.

On the third ride I start to have a lot of strange problems. Weird motor noise, brakes are more aggressive than usual. Some shit is going down....

I put the board on the bench and connect VESC to BLDC tool. I do a tests and review the realtime data. two revs of the remote and BOOM - DRV8302 fault. GAH!

I start tinkering around and uncover the motor connections (which are covered in tech wrap so I didn't notice immediately.) Oh mother eff! The middle motor cable came loose (because no tape was holding it in place and it came into contact with the tiny lip of the other connector (which was also exposed because I wrapped all three with one piece of tape, LIKE A MORON!) Their intermittent contact caused the fault.

So now I have a dead VESC.

When I finally checked the motor connections, two of them were fused together! Look at the burn mark on the bullet connector:
<img src="/uploads/db1493/original/2X/6/640492461fcaad1ac01f8aa64817f96710a4d362.jpeg" width="383" height="500">

<img src="/uploads/db1493/original/2X/9/9838db26d7f4c715d4b658c203a5a408de960435.jpeg" width="360" height="500">

**Lesson learned**: Tape up your motor connectors individually. Check all physical connections before you test on the bench. Do not win the Darwin award!

Silver lining: I ordered a new VESC from @chaka and I know it will rock!

Once that's up and running, I've got a new DRV8302 chip on the way from Mouser and it's time to see if I can manage to remove and surface-mount a chip by hand.  
<img src="/uploads/db1493/original/2X/6/6d8cfe2d20e1715b9a49e2269efdc54b08d9f757.jpg" width="250" height="250">
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-05-27T21:04:28.704Z Reads: 294

```
This is looking like a good idea

http://www.electric-skateboard.builders/t/mt60-connector-how-do-you-feel-about-them/2819?u=michaelinvegas
```

---
## \#3 Posted by: Krudte Posted at: 2016-05-27T22:47:39.679Z Reads: 266

```
This is the exact reason, I'm about to pour me, some custom connecters ^^ <img src="/uploads/db1493/original/2X/e/e70f8c34e8bf96032da219bfe08e9725020e348c.jpg" width="375" height="500">
```

---
## \#4 Posted by: 1080-aerial Posted at: 2016-05-28T05:32:40.618Z Reads: 250

```
I use these on my builds, 5mm bullets and you can only connect them one way. Just need to make sure you've got the connections right for motor direction before soldering. 

https://www.ebay.co.uk/itm/111996201879
```

---
## \#5 Posted by: KMeyerson Posted at: 2016-05-28T17:02:12.637Z Reads: 235

```
I'm thinking of using the 3.5mm for motor/ESC and the 5mm to ESC battery.

Anyone find umbilical wraps they like?
```

---
## \#6 Posted by: racidon Posted at: 2016-08-09T02:56:30.513Z Reads: 179

```
I suspect this happened to mine. Although I think it was caused by the sharpness on the motor casing itself cutting into the wires and bridging connections. 
Is there not a way we could build in a circuit that would prevent this from frying the DRV?
```

---
## \#7 Posted by: Jinra Posted at: 2016-08-09T03:07:12.265Z Reads: 173

```
it has more to do with the drv being a sensitive and fragile chip, that's why it's not going to be used in 6.0
```

---
## \#8 Posted by: racidon Posted at: 2016-08-09T04:42:37.419Z Reads: 162

```
I thought Ben was talking about using this:
http://www.ti.com/product/DRV8301
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-09T04:46:34.147Z Reads: 160

```
Sorry, I should say the DRV8302 is a sensitive chip, which is being phased out and being replaced by the 8301 on the VESC 6.0
```

---
## \#10 Posted by: racidon Posted at: 2016-08-09T04:54:18.198Z Reads: 165

```
Ah that makes sense :slight_smile:
So it's likely to handle this kind of issue?
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-09T04:54:57.753Z Reads: 167

```
It's supposed to be more robust so my assumption is that it'll handle 12S and FOC much more reliably.
```

---
## \#12 Posted by: tim_felbinger Posted at: 2016-11-14T15:39:07.099Z Reads: 127

```
So just to be clear: 

I can use a DRV8301 chip to replace the current fried DRV8302 chip on my VESC 4.12
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2016-11-14T15:43:23.903Z Reads: 123

```
No it won't work... the circuit is made only for the drv8302
```

---
## \#14 Posted by: treenutter Posted at: 2016-11-14T16:40:17.558Z Reads: 126

```
@JohnnyMeduse is right, you should use the exact same chip in the replacement.
```

---
## \#15 Posted by: 2-alex-2 Posted at: 2016-11-15T11:09:14.556Z Reads: 116

```
I have just brought these for my motor wires 

https://www.ebay.co.uk/itm/262102769365
```

---
