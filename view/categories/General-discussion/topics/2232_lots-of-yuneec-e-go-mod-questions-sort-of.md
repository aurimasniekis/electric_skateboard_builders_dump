# Lots of Yuneec E-Go mod questions - sort of

### Replies: 9 Views: 4366

## \#1 Posted by: ShannonDMV Posted at: 2016-04-08T20:07:44.715Z Reads: 153

```
Hello, my name is Armando and I'm new to the eSk8 forum. I recently purchased a Boosted Board deck with wiring still installed. I am also an owner of a Boosted Dual+. 

Anyway, I purchased the extra deck with the idea of using a Yuneec "ECU" (ESC- app controlled) and Yuneec rear truck assembly with drive train and motor installed that I had lying around to build another board. Sort of a Boosted-Yuneec Frankenstein. 

The only thing I need to get everything running is a LiPo, a gear for my drive wheel, and maybe a front truck. I'm getting pretty confused and would appreciate little guidance.

First issue: I am aware that the E-Go uses a 29.4v battery so I was looking into a 7s, 8s, or 9s lipo but I don't want to fry the esc. I saw another post on this forum talking about BMS built into the Yuneec battery with another, smaller connection to the esc, but I don't know what that means or if I need that to avoid frying the esc. I had a complete E-Go a while back and remember the smaller connection coming from the battery aside from the main thicker power cable, but the board would operate fine without it connected. Do I need any additional hardware if I purchase a 3rd party battery and connect it to the esc? Relate question- How many mah should the battery I purchase be, minimum?

Second issue: Gearing. I read somewhere that the E-Go wheel gear is 35 tooth. Would this gear:  http://goo.gl/lblX82 be compatable with the ego belt? I would drill through it and bolt it to the 71mm wheels which came in this truck/wheel kit I bought: http://goo.gl/F1aUz3 

Third issue: The 71mm wheels that come in the kit I bought, linked above. Are they going to be too small resulting in the Yuneec motor housing sitting too low and dragging on the ground? I can't test this because I haven't received the wheels yet. I can purchase a complete Yuneec wheel set for $100 but I'd rather use what I have first if I can. 

Fourth issue: Matching trucks. Do we know if the Yuneec trucks are larger/taller than the trucks that came with my kit? Again, I haven't received the kit yet so I can't compare. Since the Yuneec motor assembly I have is all built onto the Yuneec truck, I'll need a front truck and I'll need a solution if the trucks in my kit are smaller and cause the front of the board to be lower. Alternatively, I suppose I could transfer all the Yuneec components to one of my kit trucks if I modified it.


I appreciate all the help and I apologize if this post is a mess. I typed it on my phone and the site only shows me two lines of text at a time. Maybe I'll edit it later on my laptop. Let me know if you guys would like to see a YouTube video made on this project. 

Cheers :grin:
```

---
## \#2 Posted by: KMeyerson Posted at: 2016-04-10T18:48:23.845Z Reads: 124

```
Hello!

I've been fiddling with the Yuneec for a while now and have pretty much figured out all there is to the board. If you've got questions, I can answer most of them.

## Powering the Yuneec:

The battery is an 8s LiFePO4 (which means it is NOT actually 7s (29V) LiPo because LiFePO4 cells have lower votlages and thus need more cells for the same power). The connections to the ESC are an EC3 for power and a two pin cable to communicate battery temperature (which substitutes motor temperature on the PCB it would seem) and is not critical.  The stock Yuneec battery is 7.8Ah and gets you maybe 18 miles if you weigh ~120 lbs like me (1Ah = 1000mAh). You can buy more or less, it does not matter but make sure the battery can output a continuous current of at LEAST 20Amps (do not use greater than 7s LiPo).

Do **NOT** overvolt the stock Yuneec ESC - even if the FETs can handle it, the microcontroller's voltage regulation system is not capable of managing 10s for more than a few minutes. I've killed my stock ESC and am unable to get another one (hence my post about using a VESC instead).

## Wheels and Gears:
If you're going to use the original ESC, do not change the powered wheels or gearing - you're asking for trouble (ground clearance, motor power, etc).  You can try, but if you are going to swap the gear, use an abec flywheel. Do you have access to a lathe? You might have to shave the wheel to make it fit with the plastic belt cover.

The EGo trucks are pretty standard TBH, they're look like inexpensive, cast trucks so any of the cheap ones online will work. You might make sure your hangar length is the same, but 180mm is pretty standard.

- Rye
```

---
## \#3 Posted by: ShannonDMV Posted at: 2016-04-10T21:30:29.064Z Reads: 117

```
Thanks for the help man! Unfortunately, I do not have a Yuneec wheel set, incl. the driver wheel. My option is to purchase a gear/pulley and attach it to my 71mm wheels. I do have a lathe however I do not know which pulley to purchase. My other option is to buy the yuneec wheel set for $100.
```

---
## \#4 Posted by: KMeyerson Posted at: 2016-04-11T00:04:47.417Z Reads: 112

```
[quote="ShannonDMV, post:3, topic:2232"]
e a Yuneec wheel set, incl. the driver wheel. My option is to purchase a gear/pulley and attach it to my 71mm wheels. I do have a lathe however I do not know which pulley to purchase. My other option is to buy the yuneec wheel set for $100.
[/quote]

Correct me if I am wrong, but you do have the battery, ESC, and truck/plastic cover (sans wheels).

The 90mm Yuneec wheels lift the plastic motor cover about 20-30mm off the ground, switching to 70mm wheels is going to bring the motor cover 10mm closer to the ground, giving you about 10-20mm of clearance. Thats a tight gap - it might scrap if you're not careful and debris might not clear it (rocks, twigs). 

If you're determined to give it a shot, I can give you the positions and dimensions of the stock gears, belt, and axels (motor and wheel) so that you can buy a gear that will fit.
```

---
## \#5 Posted by: ShannonDMV Posted at: 2016-04-11T18:50:27.086Z Reads: 100

```
That would be great. Sans wheels? I don't have a battery, I'll be ordering a lipo. It would be awesome though if you could let me know the diameter/tooth width of the drive wheel. I'll order a pulley first before I spend  $100 on the Yuneec wheel set. My only problem is I have no idea where to get a pulley. Thanks!
```

---
## \#6 Posted by: E-Boarding Posted at: 2016-04-12T19:51:35.559Z Reads: 97

```
[quote="KMeyerson, post:2, topic:2232"]
The battery is an 8s LiFePO4 (which means it is NOT actually 7s (29V) LiPo because LiFePO4 cells have lower votlages and thus need more cells for the same power).
[/quote]

I checked this, its a 7S3P, the cells are "Samsung ICR18650-26F" or "Panasonic NCR18650 RF" Lithium-Ion (not LiFePO4 and not LiPo), you can google this up, each is 3,7V 2600mAh
```

---
## \#7 Posted by: KMeyerson Posted at: 2016-04-12T21:32:32.399Z Reads: 93

```
Which year was your board made (do you have real CF/printed wood and what color is your battery PVC)? 
They do still advertise their batteries as LiFePO4s if I'm not mistaken, but your numbers do add up (I have not had the courage to open my generally waterproof battery case. 

The Max Voltage should be 29.4 and minimum voltage 23.1 (both of which sound more or less right).  Any idea what the max discharge in real life is? I've been discharging at 20Amps without issue, but i'm getting FOC speeds around 11-12 mph and poor hill climbing compared to the original ESC. I'd go up, but I'm not sure when the battery will cut out.
```

---
## \#8 Posted by: Mrmoonlight Posted at: 2016-04-27T19:32:46.016Z Reads: 89

```
I hooked up a set of 90mm Flywheels to my E-GO. I used an Evolve gear. Had to grind out the inside of the gear a bit to fit the E-GO trucks, but with a few modifications, it works just fine. Used a 220-5M belt. Had to adjust the motor to be around a mm closer to get the tension right, but the difference was small enough that I didn't have to do much beyond widening the screw holes that hold the motor a tad. Now I'm riding 90mm Flywheels. A much nicer and softer ride than the originals. 

You could throw on a pair of 83mm Flywheels and still have some clearance, although I wouldn't recommend it. If you want to mount different wheels, you have to find a gear that fits, but 71mm would still be too small. You only get around 1cm of clearance with 90mm wheels. With 71mm, that would put your wheels right at the level of the housing. You can see on the pics. There's not enough room to go much smaller. 

<img src="/uploads/db1493/original/2X/8/8e39e4946ebfe66f047bdb99d14fb8616d779da7.jpg" width="690" height="459">
<img src="/uploads/db1493/original/2X/1/1dfecce96d1fb69a910bc37b52997923cb5bf67b.jpg" width="690" height="459">
<img src="/uploads/db1493/original/2X/b/bb64f85bf291fb44a0ddffe2a1b7a2e80cdf11c7.JPG" width="690" height="459">
```

---
## \#9 Posted by: DAKOROB Posted at: 2016-07-03T19:14:51.289Z Reads: 69

```
I am trying to put a set of Zboard 110mm wheels on my ego..I know the gear wheel won't fit past the pully....so I'm thinking I might have to shave the inside.
```

---
