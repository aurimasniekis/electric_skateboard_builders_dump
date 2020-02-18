# Another Truncated Tesseract build

### Replies: 19 Views: 2850

## \#1 Posted by: kortho Posted at: 2016-10-17T00:55:47.780Z Reads: 362

```
Well let me start off by saying I’ve been lurking around here for a little while gathering information and ow I believe it’s time to contribute. 

First a little background.  I have a Master’s degree in Mechanical Engineering so it would be a fair statement to say I’m a bit nerdy.  I’ve always been interested in building pretty much anything and spend the majority of my spare time in my wood shop making furniture.  A few months ago I was introduced to electric skateboards by Casey Neistat and the Boosted Board. While I found the idea to be a novel one I found the board to be lacking.  So after a few short minutes of googling I found that it wouldn’t be very hard to build my own to the way I wanted it.  
Now there seems to be two thoughts to this process, build from scratch and assemble from parts.  With my first born daughter still an infant I have more money than time so I chose the latter approach while fabricating what I could.  
To start off here is my BOM with associated prices and comments for those that are interested.  
Deck:
Loaded Truncated Tesseract			        $230

Trucks – Bears – wheels - risers:
	Callibur 2’s 					        $54
	Reds bone swiss				        $50
	Orangatang Kegels 83a			        $60
	Luxe 0.5 inch					        $4

Motor & mount:
        Alien 6355 HEV 190 kv x2                      $73 ea
	Alien drive longboard diy 63mm kit x2		$145 ea

Electronics:
	Nyko Kama remote				        $15
	DIY Electric skateboard VESC x2 		$90
	Parallel XT90 connector 			        $9
	CAN bus connector				        $7

Battery:
	Battery Bro Samsung 25R5 x50			$3.68 ea
	Dxsoul diy 4 slot 18650 battery holder x10	$32
	Mean Well HLG-150H-42A Power supply	$62

MISC:
	Wire, nuts, screws, ect. 				$50

Needless to say this project coming in at a total of $1373 was way more than my expectations in the beginning.  But everything always costs more and takes longer than one would think, and I still came in under the price of a Boosted Board.  
A few comments on why I chose certain items, to start off with the deck was for the simple reason that it is a tried and true deck that is compact and can handle speed.  I went with Alien’s mounting kits because of all the others I looked at these appeared to be the better engineered, with minimal stress concentrators and well machined.  I went with DIY’s VESCs because after scouring the forum they had the least complaints for the best price.  Battery Bro was able to get me a decent price for a bulk buy of 50 cells, however I will say that shipping was a nightmare. It took well over a month to get the cells despite the fact that I paid extra to have 3-5 day air shipping and when I received them I was missing some additional items I had ordered, so it took another 2 weeks for them to fix it.  I will say they refunded me for the items that were missing in the first package but it was still a disaster and I don’t think I would use them again.  The battery charger I chose is not actually a charger, it’s an LED power supply.  However it has a customizable output voltage from 37 to 47 volts and a max amperage setting up to 150 watts total output.  So I set the voltage to 41.5v and 3.6A, I don’t use a BMS for reasons that WhitePony has outlined and the charger works quite well.  It won’t charge the cells to fast due to the max amperage setting and as battery voltage approaches supply the current draw tappers off to zero. 
But enough words let’s get to some pictures.  
First up are the Alien parts, and while the quality is good I found the finish to be a little lacking, there were a number of burs on the Kegel adapters that had to be filed for proper fit. 
<img src="/uploads/db1493/original/3X/a/1/a1a113a119c2f32fda0180fac8de8e31a17ed308.jpg" width="374" height="500">

Next is the 32T HTD5 pullley and as you can see more burs from manufacturing 
<img src="/uploads/db1493/original/3X/c/1/c1c3b80dd8f528c6169deadc8d9b9e76d51715ba.jpg" width="374" height="500">
and along with that the diameter of the pulley is not quite right for the 32 teeth and the HTD5 pitch so as you can see when there is tension of the belt there is a bit of slack in a portion of the belt.  this will cause premature belt failure and eventually the teeth of the pulley will begin to wear away due to the concentrated stress at the enterance and exit of contact. 
<img src="/uploads/db1493/original/3X/9/c/9c2fb18576c9905e5c5aab91ed7ed7fefd121624.jpg" width="374" height="500">
The next part are the truck adapters and while I like water jet manufacturing I would not consider it an acceptable as milled surface finish so again a file was needed to finish the part to get it to fit in the motor mounts. 
<img src="/uploads/db1493/original/3X/b/8/b870caed05dc8fe0f7733c144011a80de8f5c71d.jpg" width="374" height="500">
These nest two images shows the galling on the adapters from an extremely tight mount fitting and the non perpendicular circumference to the sides. 
<img src="/uploads/db1493/original/3X/e/1/e17ba078334dafea573c29cbdf7e3b4e5ade947f.jpg" width="374" height="500">
<img src="/uploads/db1493/original/3X/3/b/3bb0385b90452485587758cae5a947a771626ee7.jpg" width="374" height="500">
However that all being said, with a bit of work everything went together well and I am please with the finished product.  
Next up came the battery build, I decided to go with these 18650 sleds that were only $3.20 a piece and modify them.  starting with the removal of the leads and parallel connections.  
<img src="/uploads/db1493/original/3X/2/6/2682185e41a79977140f828179ff3591dcc5b54e.jpg" width="374" height="500">
Then I added 14 awg solid copper bus wire in a configuration to make a 10S4P battery.  It's not show but I doubled up on the 14 awg wire for an equivalent 12 awg which is more than enough to handle the amperage and when checking the resistance of the connections it was below the tolerance of the meter so about .00002 ohms. 
<img src="/uploads/db1493/original/3X/d/7/d794023ea8c3043382019329bea51e7cbf232ac9.jpg" width="374" height="500">
Next I added braided protectors to the motor wires and heat shrank then ends. 
<img src="/uploads/db1493/original/3X/2/0/20f4112e5575b7035bfc6404605d9ad74bb3b7ca.jpg" width="375" height="500">
The heat output of the fets on the VESC gave me a bit of concern so more for peace of mind than anything else I added these little RAM heat sinks to each fet.  
<img src="/uploads/db1493/original/3X/8/0/80ed193059f378261ef029e6fe7dc16bbcd536fe.jpg" width="375" height="500">
Next came modifying the deck to accommodate the battery, electronics, and case.  I had to make a router sled so I could accurately route out a max 5 mil deep uniform surface to which everything would be mounted to. 
<img src="/uploads/db1493/original/3X/2/c/2c0d7ec6747c46cfc1ca873f3a068549ff5526ea.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/6/8/680ff0cefd6eb6eea37a9744705907af1fe0bd26.jpg" width="374" height="500">
<img src="/uploads/db1493/original/3X/b/b/bb79f52f9f3f1f7e90807d1fc28eed38327c78ff.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/2/6/2603bb3e22fd3f58da85d2fbbc076dbb596a795a.jpg" width="375" height="500">
Once all that was done I tried my hand for the first time at vacuum formed carbon fiber molding.  I'm not particularly pleased with the way it came out so in the next week or two I plan on doing it over and adding reinforcement in high stress areas such as fastener pass thoughs due to deck flexing. 
<img src="/uploads/db1493/original/3X/0/e/0ea02c952cd89163d50abf905ec7e6e7adcb9d1f.jpg" width="375" height="500">
With the major fabrication done it came time to assemble the electronics, I added an additional lead to the Kama receiver antenna so it could be routed outside the case.  
<img src="/uploads/db1493/original/3X/0/0/00213f6652e0fdab43ed42f12a9e0ab790319162.jpg" width="375" height="500">
I then did an initial assembly of the electronics pack for a test fit and run to identify any potential problems.  
<img src="/uploads/db1493/original/3X/3/b/3b1170e76f25d38820f6bae01e931f2810b5c2be.jpg" width="375" height="500">
After the first ride it became quite obvious that I was going to have to take greater steps toward vibration management.  I noticed that due to the orientation of the battery cells, constant vibration could cause them to lower to the point of intermittent contact.  I'm not ready to glue them all in place because as I mentioned before I'm not using a BMS so I want to maintain the ability to monitor and if necessary replace individual cells if I notice a problem.  so I added carbon fiber panels and metal straps to keep everything in place.  also notice I'm using an XT90 anti-spark switch and I've placed the Kama receiver away from high frequency switching amperage sources to minimize interference.  
<img src="/uploads/db1493/original/3X/d/9/d9c2af2b81c3fbfafdc4be6326c16671ac274f06.jpg" width="375" height="500">
After all the here is the final result.  
<img src="/uploads/db1493/original/3X/4/5/459becc1f81c96b39e65664e744af404e283c0f0.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/9/b/9b7464c80f22c9a1a90e01fb9b31f977b33f9df0.jpg" width="666" height="500"> 
As I mentioned before I intend to redo the enclosure and I'm also thinking of switching to abec 11's 
Thanks for reading and I hope this helps some as I have found help from the forums.
```

---
## \#2 Posted by: JLabs Posted at: 2016-10-17T01:07:11.745Z Reads: 310

```
Great right up! I like all the pics and details! Beautiful board, keep up the good work!
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-10-17T01:39:51.245Z Reads: 294

```
Nice build... but from experience Kegel are way smoother than the Flywheels.
```

---
## \#4 Posted by: Pantologist Posted at: 2016-10-17T01:47:39.960Z Reads: 280

```
Smoother? I thought abecs would be smoother considering their lower durometer.
```

---
## \#5 Posted by: kortho Posted at: 2016-10-17T01:50:03.713Z Reads: 271

```
Its the combination of the lower durometer and larger diameter that has me interested, just looking for a way to smooth out the bumps a bit.
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-10-17T01:51:54.884Z Reads: 265

```
Sorry... yes the duro is lower on the abec a 78a, but in my personal taste the Kegel feel way smoother... I've try the two different type on previous setup and I prefer the Kegel
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-10-17T02:04:22.602Z Reads: 256

```
Are you looking at the 90mm or the 83mm ?
```

---
## \#8 Posted by: kortho Posted at: 2016-10-17T02:09:05.109Z Reads: 250

```
Sorry I should have been more spacific, I'm looking at either the 83 mm 75a, or the 90 mm 78a. With the larger diameter you won't feel small cracks as much but the higher durometer means small bumps and rocks will be felt more so I think it's a bit of a toss up between the two.
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2016-10-17T02:34:27.653Z Reads: 246

```
If you are really looking to see a difference, I suggest to go with the 90mm they are bigger and will probably handle more thought road... You won't much difference from 83mm version.... But the best bet, If you have access to skateshop who has them in stock, is to physically compare them.
```

---
## \#10 Posted by: Eboostin Posted at: 2016-10-17T02:45:50.467Z Reads: 240

```
Definitely go with the flywheel 90mm or higher. The Kegels look cool, but are not ideal unless you have perfect pavemenf everywhere you skate.
```

---
## \#11 Posted by: Pantologist Posted at: 2016-10-17T02:58:59.613Z Reads: 224

```
90mm is just so freaking huge though. On a Truncated Tess you will probably need a 1inch riser. On my tesse I have angled 1/4 to 1/2 inch risers just stop wheel bite with my 83mm flywheels.
```

---
## \#12 Posted by: kyo Posted at: 2016-10-17T03:19:19.685Z Reads: 215

```
Hi great build, a lot to learn from. Quick question: what kind of lead that u use as antena?
```

---
## \#13 Posted by: kortho Posted at: 2016-10-17T04:19:53.847Z Reads: 216

```
It's just a standard 22 awg copper stranded unshielded wire.
```

---
## \#14 Posted by: kyo Posted at: 2016-10-17T04:40:41.879Z Reads: 220

```
Great thanks, how did u do it? Did u drill a hole? Or just solder it on?
```

---
## \#15 Posted by: kortho Posted at: 2016-10-17T05:08:17.401Z Reads: 224

```
It's soldered right to the antenna trace on the pcb
```

---
## \#16 Posted by: Jebe Posted at: 2016-10-17T06:35:02.666Z Reads: 233

```
Nice build. Can't go wrong with abecs.
I did see somewhere that kegel are working on a softer wheel but I can't for the life of me find it again
```

---
## \#17 Posted by: Deathjunior Posted at: 2016-10-17T14:29:39.199Z Reads: 265

```
<img src="/uploads/db1493/original/3X/0/0/00c8146fafd570b452936a430ff0c7f5871b8336.jpg" width="374" height="500">, 97mm's ftw
```

---
## \#18 Posted by: kortho Posted at: 2016-10-22T03:03:29.065Z Reads: 292

```
I may hold off on the flywheels for a while, I'm considering selling this board and starting over with a trampa build. Too much fun to tinker and build
```

---
## \#19 Posted by: kortho Posted at: 2016-11-03T02:49:43.256Z Reads: 274

```
As promised I have redone the enclosure and am much happier with it.  The original enclosure was only 2 plies of 1x 1 carbon. The new enclosure starts with  e-glass then 2 layers of carbon with a metal flange imbedded in to prevent tear out in the mounting hole from board flex. 

<img src="/uploads/db1493/original/3X/b/f/bf29768371119caced4091e34192ac89290f3400.jpeg" width="374" height="500">
<img src="/uploads/db1493/original/3X/4/9/49ca1d48690d8c24f7abbb4b165b30419931cc80.jpeg" width="374" height="500">
<img src="/uploads/db1493/original/3X/5/8/58a466515eaf2c74835f0183ad7900baf164ba3d.jpeg" width="374" height="500">
<img src="/uploads/db1493/original/3X/5/0/50ef1cb34def3dae955e8c4054dafd4174e6e9b9.jpeg" width="374" height="500">
<img src="/uploads/db1493/original/3X/4/0/40b1bc51abecb938e8e4f669b0cac82c59b48163.jpeg" width="374" height="500">
```

---
