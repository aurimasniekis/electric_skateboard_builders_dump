# Some lights on the board?

### Replies: 14 Views: 1532

## \#1 Posted by: Bloop Posted at: 2017-08-01T16:30:56.607Z Reads: 217

```
Id like to add some lights on my board. i have a strip of 5m of white leds but i dont really know how to power them up. 

Do i have any spot on the vesc from where i can get 12V 5A ? Or do i need to get a stepdown regulator for this ? 

I dont want to connect my lights directly to the battery since they will drain just some cells and my battery will get unbalanced .. 

Thank you.
```

---
## \#2 Posted by: themegak Posted at: 2017-08-01T16:40:26.213Z Reads: 214

```
I use a step down regulator after the power switch to power some 12v lights.  I also added another switch so that i can turn on/off the lights when the board is on.  I used something like the link below and it works great.  You can get this in various size profiles if you search on ebay and amazon.  5amps is a bit high, I am not sure you will find anything that is small that will give you 5 amps but you should be able to find something that can support 2 - 3 amps out at a good size.

https://www.amazon.com/eBoot-LM2596-Converter-3-0-40V-1-5-35V/dp/B01GJ0SC2C/ref=sr_1_9?ie=UTF8&qid=1501605403&sr=8-9&keywords=step+down+voltage+converter
```

---
## \#3 Posted by: Bloop Posted at: 2017-08-01T16:45:51.114Z Reads: 197

```
yeah you are right i dont need 5A out of it cause i wont use 5m of leds... i only need the 12V tho
```

---
## \#4 Posted by: melchiorvester Posted at: 2017-08-01T16:52:01.867Z Reads: 192

```
Yeah that step down converter is very useful and has a pot on it so you can change to voltage to how ever much you need. Just make sure to test the voltage before you put anything on the receiving end
```

---
## \#5 Posted by: SilentException Posted at: 2017-08-01T19:50:02.294Z Reads: 174

```
If using step down converter, make sure you get the switching type with the regulated output. Otherwise, you will have heat problems and/or your output voltage will drop as input voltage (battery voltage) drops.

I would use a BEC instead. Similar thing but it has all the above requirements and then some. This one is nice, very wide input range and two outputs (5V / 12V) with much amps.

https://hobbyking.com/en_us/turnigy-multistar-twin-output-5-10-amp-6-50v-sbec-for-lipoly.html

After the step down module or BEC, you'll have a nice 5V or 12V output which you can connect LEDs to. But, if you have a two channel received, you could push it further :) Get (or make) a trigger relay circuit, something like this:

http://www.ebay.com/itm/DC12V-Signal-Trigger-Delay-Turn-Off-Adjustable-Timer-Control-Switch-Relay-Module-/192260589813?hash=item2cc39fc8f5:g:s-wAAOSwTA9X9yho

You connect this after the BEC and use second channel of the receiver as a trigger so you can turn the lights on and off with the remote.

I've been planning this for my board and even had the whole thing running on the bench but at the end I scrapped the idea because it was too many wires and stuff. I just wanted a board and thought: "meh, ShredLights will do" :)
```

---
## \#6 Posted by: sl33py Posted at: 2017-08-01T20:17:21.929Z Reads: 167

```
i've measured some 5050 SMD LEDs and the whole 300 light 5m roll took just shy of 2a.  So for a few feet i think your current draw will be minimal.

Your options are to convert your battery voltage (you don't mention - let's assume 8s) so 33.6v -> 12v stepdown dc to dc needed.  OR  you can get a small 3s lipo to power them and only plug in when you want light?

Your VESC would not be a good solution - besides it providing around 5v not 12v i would not try to pull 1-2A current through it.  A dead VESC for this seems bad.

I went with some blitzu bike lights front/rear on my board when riding at night - work pretty well.  I prefer the brake light blinking for visibility, and a headlamp on my helmet for better visibility of the path in front of me.  i found even the newer 168 lumen (claimed but still) white headlight didn't illuminate far enough ahead to be super useful.  The rubber strap works perfect around the truck hanger between the bushing seat and pivot cup - just wish it would adjust a smidge more "up" to further point in front vs down at the ground.

HTH - GL!
```

---
## \#7 Posted by: Bloop Posted at: 2017-08-01T20:21:49.015Z Reads: 149

```
Yes i think the separate battery would be the perfect solution. But i was wondering if i can get something kinda easier. 

Thank you for the answers.
```

---
## \#8 Posted by: Bloop Posted at: 2017-08-01T20:22:24.770Z Reads: 140

```
Silent i agree with you.. with all of these would be too many cables all over the place.
```

---
## \#9 Posted by: sl33py Posted at: 2017-08-01T20:24:46.403Z Reads: 143

```
This is *easiest* and works REALLY REALLY well at night.

5000 lumens and bright as hell:
[img]https://goo.gl/A2vBep[/img]

Feel a bit like a coal miner... with the red light behind the board, and this to see where i'm going... G E N I U S ! ! !
```

---
## \#10 Posted by: Bloop Posted at: 2017-08-01T20:27:11.202Z Reads: 129

```
cannot see the picture
```

---
## \#11 Posted by: JdogAwesome Posted at: 2017-08-01T20:28:18.076Z Reads: 134

```
I just use one of the LM2596 converters @themegak recommended, though they only work upto around 40V so 10S and 12S won't work with it and then you'll want to use a UBEC. I also just use a pushbutton switch to control the lights cause I don't want them on 24/7. You can find some cheap headlights in eBay called 15W Eagle Headlights or something and there decently bright and I just have 2 of them on the front of my board. Then on the bottom I just have some cheap 10W led steps I also got on eBay. Also the wattage that most LED's on eBay are rated at is wayyyyyy higher than they actually are, they just do it to make them sound better and it confuses a lot of people. 
<img src="/uploads/db1493/original/3X/d/7/d73a70a9838cb2c87474637f6616e1afdc3cc6a3.jpg" width="690" height="389">
```

---
## \#12 Posted by: treenutter Posted at: 2017-08-01T20:46:33.459Z Reads: 131

```
http://www.electric-skateboard.builders/t/eskate-lights-thread/199/
```

---
## \#13 Posted by: wafflejock Posted at: 2017-08-01T20:59:37.360Z Reads: 130

```
Made my own version of these here:

<img src="/uploads/db1493/original/3X/9/4/94ee18ef3b918885f0a1a96974e847e997b30d8d.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/1/b/1bfe20a154c4a03691eb99f1e1369beb5a50cd96.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/e/a/ea86b80164a97700246d3f80cca820d163035648.jpg" width="375" height="500">

Pretty sure I had never seen the flux lights before but it's a very similar design in the end.  Only differences with mine are basically the LEDs are surface mount type and has a diffuser in front of it (had to pour those out of clear epoxy which takes forever to cure).  Was thinking of selling just the plastic housing (or a kit) and instructions to piece it together since I'm not sure I could really do full assembly and still make any sort of profit off of them (they are .5").  Used a TP4056 for charging and 350mAh LiPo in the riser for power, that was as big as I could find that would fit in a .5" riser (LEDs should be pulling about 40mA so should last close to 10 hrs still of on time, charges in about 30 min).  Considered doing the power off the main battery supply but also figured the wiring would be more mess than it's worth.

---

Also you can see there are some problems with my mold but was the first time I gave this a go so knew it wouldn't be perfect, ordered some more silicone since I'm going to tweak the design on the riser itself slightly still to make the switch easier to mount and access and to try and eliminate any remaining air pocket areas (give them runners for the fluid to flow up through.

<img src="/uploads/db1493/original/3X/a/1/a1fa4840de7cd11a2e4e2833cb52991fd64b5a81.jpg" width="375" height="500">

These also work as just 3D printed versions (ABS or Nylon, PLA will crack over time) but the molding plastic is more durable and has no chance of delamination like the 3D printed original.

https://cad.onshape.com/documents/7be8e5eec66596f68a989626/w/2c722dcc2ec89f5c71643bec/e/488c17c6f310d5c7be62da8a

^^ original model if you want to tweak it or print one for yourself, make sure to print 2D drawings at 1:1 scale first to be sure dimensions are correct before wasting time and plastic if anyone decides to do this.

---

If interested in trying out some of these imperfect molds for the price of shipping would be better than me throwing them in the bin so PM me a PO Box/Mailing address and will see what shipping costs (I'm at the edge of Chicago).  If you have a printer exported the STLs and uploaded to thingiverse here: https://www.thingiverse.com/thing:2397920
```

---
## \#14 Posted by: Bloop Posted at: 2017-08-02T07:50:32.536Z Reads: 98

```
Wow this looks really nice. Good job and yeah keep testing you will get there.

Thanks for suggestions.
```

---
