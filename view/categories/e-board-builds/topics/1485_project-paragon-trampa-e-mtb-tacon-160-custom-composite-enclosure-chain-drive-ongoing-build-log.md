# Project Paragon &#124; Trampa E-MTB &#124; Tacon 160 &#124; Custom Composite Enclosure &#124; Chain Drive &#124; Ongoing Build Log

### Replies: 30 Views: 5347

## \#1 Posted by: paragon Posted at: 2016-02-21T07:00:20.988Z Reads: 344

```
Hello,

After completing a pintail build and riding around, I nearly fell a few times due to going over small rocks. I have also experienced speed wobble at around 25mph. To kill two birds with one stone; I decided on a mountainboard build. Most electric mountain boards that I have seen looked extremely heavy and ugly (with the exception of E-Toxx builds), and I didn't like the idea of having a box of lithium under my legs :stuck_out_tongue_winking_eye: . Here is my shot at a sleek electric mountain board:

<img src="/uploads/db1493/original/2X/3/3c1a4acf5ba9579855c6b1ed537ede10f39f729d.JPG" width="667" height="500">

My enclosure is made from G10 (CF blocks my GT2B signal) and Aluminum), and there is still a couple of inches of ground clearance below it. I have designed it for dual drive, but for now I will only use one motor. There is plenty of space in the box for lipos, escs, motors, wiring, etc. I am also working on V2 which will work with channel/spring trucks. My custom enclosure is extremely sturdy so far, and I may even sell some kits, if there is interest.

Current Setup:
Tacon 160
FVT120a esc
6s 5.2ah Multistar Lipo
10T motor sprocket
55T electric scooter sprocket (mounted using my G10 adapter)
25 chain
Cool looking voltmeter, light-up switch, and loop key
```

---
## \#2 Posted by: lox897 Posted at: 2016-02-21T09:11:34.133Z Reads: 317

```
Awesome! Could you post some more pics of the whole board and maybe inside the enclosure? Good job.
```

---
## \#3 Posted by: paragon Posted at: 2016-02-21T18:22:46.720Z Reads: 315

```
<img src="/uploads/db1493/original/2X/e/ed4b3bbcdd9611539352b07d3fdfecea578d5b3c.jpeg" width="666" height="500"><img src="/uploads/db1493/original/2X/b/ba4e14a3a3c7b4d95b50de599553ea894aac9798.jpeg" width="375" height="500">
```

---
## \#4 Posted by: paragon Posted at: 2016-02-25T05:05:59.020Z Reads: 297

```
So I finally figured out my 5 pin 12v switch, sort of.
Here is a picture of the switch:
<img src='/uploads/db1493/original/2X/2/229eab21f59cd6578b940c40d5aab14d32cb2403.jpeg'>
I installed it in place of the switch on my FVT120a esc (same as diyesk8's 6s esc) and matched up the wire colors to the chart above; everything worked, but when I powered the esc, it wouldn't exit programming mode.

Next I tried powering the switch from my receiver. I bridged the "+" and "NO1" pins and soldered the positive wire from my rx, then soldered the negative rx wire to the "-" pin. I soldered the white wire from the esc's old switch to "C1" This time it worked perfectly, on 3s. When I plugged in my 6s battery, the positive wire vaporized and my receiver died.

I'll be trying the following configuration next (if anyone knows the correct combination, feel free to help a temporarily multimeter-less fellow like me): 
+ and NO1 powered from a 12v bec
- also connected to the 12v bec
C1 connected to the white wire from the esc's old switch.
```

---
## \#5 Posted by: onloop Posted at: 2016-02-25T05:10:53.439Z Reads: 269

```
sweet build mate, i like the wire braiding!

will you be using foot straps?
```

---
## \#6 Posted by: paragon Posted at: 2016-02-25T05:11:35.260Z Reads: 265

```
Or would white wire (from the old esc switch) to "C1," black wire (from old esc switch) to "-" ,and "+" and "NO1" bridged and connected to my 12v bec work?
```

---
## \#7 Posted by: paragon Posted at: 2016-02-25T05:12:49.546Z Reads: 265

```
Thanks Onloop!
I'll be getting matching white and black bindings as my reward when I finally get my switch working :joy:
```

---
## \#8 Posted by: onloop Posted at: 2016-02-25T05:14:13.518Z Reads: 259

```

sorta looks cool without bindings
```

---
## \#9 Posted by: paragon Posted at: 2016-02-25T05:23:42.786Z Reads: 250

```
@onloop 
Yeah,
I'll probably keep this one as a cruiser, and build a matching 2 wheel drive Trampa with channel trucks and bindings.

On another note, can you help me with the switch? :wink:
```

---
## \#10 Posted by: paragon Posted at: 2016-02-25T15:58:32.371Z Reads: 240

```
So no one knows how to wire this switch?
```

---
## \#11 Posted by: Iceni Posted at: 2016-02-25T16:30:11.123Z Reads: 261

```
I have switch with similar pin layout, though i havn't plugged in the lighting on it.
I had to use a multimeter to figure out which pole did what since the schematic wasn't correct.


This is what i ended up with for on/off operation
<img src="/uploads/db1493/original/2X/d/d4e47eb48d4ba04cefaad63fdb9329a5018bfcbc.jpg" width="656" height="497">
Yes, it looks terrible, I need to get a new soldering iron :P
```

---
## \#12 Posted by: paragon Posted at: 2016-02-25T16:49:45.611Z Reads: 241

```
Thanks! So outermost pins are probably for powering the led and the remaining pin stays untouched?
```

---
## \#13 Posted by: Iceni Posted at: 2016-02-25T16:55:50.420Z Reads: 234

```
Yes, should be if i read the schematic correctly.
```

---
## \#14 Posted by: Iceni Posted at: 2016-02-25T17:00:57.939Z Reads: 241

```
This is the schematic for my switch, might help you figure it out if with the lighting.
Though it assumes you're using 12 volts through the switch as well, so if it's not powered by 12 volts i don't think it can be wired the same way.
<img src="/uploads/db1493/original/2X/d/daf7a1e2d7bf44a18c5950f4b4697b27c1b227e3.jpg" width="690" height="477">
```

---
## \#15 Posted by: paragon Posted at: 2016-02-26T05:07:51.002Z Reads: 240

```
More complications: 
After frying my rx, I decided to power the esc with a different rx to see if it still functioned. My esc fried immediately, but hopefully it is not beyond repair. I have attached a picture of the burnt piece of the esc, and I'm wondering if anyone has access to the schematics (or is willing to take apart their fvt120a) so that I could find out the part that I need to replace.<img src="/uploads/db1493/original/2X/c/cdd6a6891d4a1c87ab4acf5050a6cdba07bebae8.JPG" width="666" height="500">
```

---
## \#16 Posted by: paragon Posted at: 2016-03-09T05:44:51.660Z Reads: 230

```
SUCCESS! Here is the correct wiring for anyone else who may have had similar issues with this switch.
<img src="/uploads/db1493/original/2X/d/de923b9bf913edee07560f545d7fffb9ca66263f.JPG" width="375" height="500">

<img src="/uploads/db1493/original/2X/1/1edbf6128ee85a9f02cdeb145f92137023648532.JPG" width="375" height="500">
```

---
## \#17 Posted by: paragon Posted at: 2016-03-09T05:46:03.680Z Reads: 215

```
By the way, the newest batch of FVT120a escs comes with a third cap externally installed.
```

---
## \#18 Posted by: trampa Posted at: 2016-03-31T19:06:29.162Z Reads: 207

```
Nice little project! Congratualtions from Trampa. If you want to build a spring truck version, feel free to give me a buzz. Frank

frank@trampaboards.com
```

---
## \#19 Posted by: Ulfberht Posted at: 2016-04-01T06:12:40.127Z Reads: 197

```
Dude that mountainboard is sweet!!! Damn!! :open_mouth:
```

---
## \#20 Posted by: Karmannghiagirl Posted at: 2016-04-04T04:00:51.824Z Reads: 190

```
Hey, i am looking at getting a set of those wheels for my build. How did you mount the sprocket to them?
```

---
## \#21 Posted by: paragon Posted at: 2016-04-04T04:18:48.056Z Reads: 164

```
You can get a set here: http://m.ebay.com/itm/Ground-Industries-Balistik-MAK-Tires-And-Silver-Terraintula-Hubs-qty-4-/201552445364?nav=SEARCH

I attached the sprocket using a 2mm thick g10 adapter.
It works pretty well. There isn't play in any direction, and it's very easy to center the sprocket.
```

---
## \#22 Posted by: Karmannghiagirl Posted at: 2016-04-04T04:23:19.285Z Reads: 163

```
[quote="paragon, post:21, topic:1485"]
2mm thick g10 adapter
[/quote]

what is this/where can i get it?
```

---
## \#23 Posted by: paragon Posted at: 2016-04-04T04:40:26.246Z Reads: 161

```
Its just a custom cut g10 (garolite/fiberglass/pcb material) piece. Carbon fiber, aluminum, or even wood could work.
```

---
## \#24 Posted by: Karmannghiagirl Posted at: 2016-04-04T04:44:10.530Z Reads: 163

```
<s>Sorry if this is obvious, but what do you mean g10? what is a g10?</s>

oh my god im an idiot :sweat_smile:
http://www.fingertechrobotics.com/proddetail.php?prod=garolite
im assuming this is what you are talking about?
```

---
## \#25 Posted by: paragon Posted at: 2016-04-04T04:55:45.786Z Reads: 158

```
You're assumption is correct :smile:
```

---
## \#26 Posted by: Ulfberht Posted at: 2016-04-08T13:16:09.608Z Reads: 156

```
[quote="paragon, post:21, topic:1485"]
You can get a set here: http://m.ebay.com/itm/Ground-Industries-Balistik-MAK-Tires-And-Silver-Terraintula-Hubs-qty-4-/201552445364?nav=SEARCH
[/quote]

That's a great deal on those wheels!!
```

---
## \#27 Posted by: paragon Posted at: 2016-04-08T13:56:30.941Z Reads: 153

```
Yeah, I bought 2 sets. They are carbon fiber and aluminum construction.
I was worried about the tires wearing too quickly, but they are holding up so far.
```

---
## \#28 Posted by: Ulfberht Posted at: 2016-04-08T13:58:32.149Z Reads: 151

```
BTW: Epic build dude!!! That thing is mean looking!
```

---
## \#29 Posted by: willpark16 Posted at: 2016-07-25T19:03:11.236Z Reads: 120

```
how loud is that chain drive?
```

---
## \#30 Posted by: paragon Posted at: 2016-07-26T16:45:07.802Z Reads: 111

```
not too loud, it doesn't strike me as extremely loud or annoying when I ride it, but it's not as quiet as belt drive.
```

---
