# First build, some questions about it; any suggestions?

### Replies: 15 Views: 749

## \#1 Posted by: edaemon Posted at: 2018-03-11T20:49:03.231Z Reads: 108

```
First of all this site has been really helpful so far, so thanks to everyone who's posted information here.

This is my first build, and I think I have everything I'll need, but here's the list in case anything is out of sorts:

1. [ESC from ebay](https://www.ebay.com/itm/Dual-motors-longboard-skateboard-controller-with-remote-ESC-Substitute/302538835504)
2. [Motors from ebay](https://www.ebay.com/itm/302546262750?ViewItem=&item=302546262750)
3. Two [5S1P 8000mAh batteries](https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c-xt90.html) in series
4. Either the [Bestech 10S BMS](http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html) or a [10S BMS from SuPower](http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html)
5. A [basic deck](https://www.skateshred.com/36-x-9-5-bamboo-drop-through-deck.html) from SkateShred

As you can probably tell I'm opting for something that's not too expensive or fast but has decent range. I'm hoping to commute with it so I don't want to run out of power on the way.

There are a few things I'm not sure of. First, the wiring is a little iffy to me -- I drew up a diagram that I think is right, but I'd appreciate any pointers. Second, I'm not sure which charger(s) I should buy. There are plenty out there but I can't tell which ones are reliable. Finally, the BMS situation: the Bestech BMS looks great and has a built-in e-switch but I have to buy two of them; I was going to buy the SuPower BMS but their site currently doesn't allow US customers to purchase from them. Should I just go with Bestech or does anyone know how I can order the SuPower?

Here's the wiring diagram I put together (this was with the SuPower BMS in mind):

_EDIT_: this diagram isn't quite right. I have an updated one in the comments.

![Longboard wiring diagram|690x285](upload://ssmHc45QJFWtaTDZVfcRJ68N2i1.jpg)

Thanks for any help!

EDIT: I was able to order the SuPower BMS via email. Hope that one works out!
```

---
## \#2 Posted by: Grozniy Posted at: 2018-03-11T23:33:17.386Z Reads: 88

```
All parts are OK. If you want it simple: don't get a BMS, get a IMAX b6 charger. You'll have to charge them separately or with a parallel board.
To connect the batteries in series, just get a series harness from hobby king.
If the deck is flexible you'll need a split enclosure.
Get some risers because you need about 10cm of ground clearance from the battery enclosure
```

---
## \#3 Posted by: MannyM0E Posted at: 2018-03-11T23:38:30.402Z Reads: 88

```
mmaner
Regular12d
This is what I use to pad electronics, a little hot glue and it will stay forever.
amazon.com10

Amazon.com: XCEL 54"in. Wide x 1'ft. Length x 1/8" Thick Soft/Medium Neoprene Sponge Foam Rubber Sheet, Black: Industrial & Scientific

Protect valuable tools, dampen sound, or weatherproof your home with this versatile Soft/Medium Neoprene Rubber Roll by XCEL. Made in the USA, this durable, foam rubber mat is the same type of materia ...

This is what I use to seal enclosures, you can 1/4 or 1/16 depending on your rneeds. I find that 1/8 give a lot of forgiveness against concave…
amazon.com7

Sponge Neoprene Stripping With Adhesive 1/2 Inch Wide X 1/4 Inch Thick X 35 Feet Long - - Amazon.com

This is a closed cell sponge neoprene that will not absorb water or oil. It is often referred to as weather stripping or rubber sealing and is primarily used as sealing tape to block air, dust and moi ...

3 Likes
@mmaner
```

---
## \#4 Posted by: pat.speed Posted at: 2018-03-12T02:11:32.022Z Reads: 70

```
I don't know why you think an IMAX B6 is simple but it's not, it is easy to setup but having to undo your enclosure every time to charge isn't exactly simple. It's also a pain in the ass. Ask me how I know

A bms is a little harder to setup in the start but is so much easier in the long run.
```

---
## \#5 Posted by: Sippahodge Posted at: 2018-03-12T02:29:11.296Z Reads: 62

```
I have a solution for that
```

---
## \#6 Posted by: pat.speed Posted at: 2018-03-12T03:06:54.750Z Reads: 56

```
A solution for what?
```

---
## \#7 Posted by: DeathByBacon Posted at: 2018-03-12T03:12:25.971Z Reads: 59

```
Nice setup. What app/software did you use to make the diagram?
```

---
## \#8 Posted by: edaemon Posted at: 2018-03-12T03:24:11.618Z Reads: 58

```
Thanks, I just put it together in Google Drawings.
```

---
## \#9 Posted by: edaemon Posted at: 2018-03-12T03:30:03.749Z Reads: 61

```
Thanks for the info. I looked at using chargers like the IMAX B6 but I'm opting for a BMS as I want to be able to charge it at work or in a coffee shop (I work remotely sometimes), so I don't want to lug a balance charger around in my backpack and have to take anything apart on the board to charge it. I need to be able to just plug it in.

I'm planning on making a split enclosure for the batteries and components out of some kydex I have left over from other projects. Thanks for the tip on clearance -- it might be good enough as-is but I hadn't though of that. I'll be sure to pay attention to it.
```

---
## \#10 Posted by: gigoy Posted at: 2018-03-12T04:02:50.846Z Reads: 66

```
This was almost exactly like my first build, sans the BMS.

It's a solid build and can be a nice ride especially if you have nice roads. On unforgiving roads, it's a different story. A few kilometers will turn your legs to jelly. Shock pads and good shoes will help.

The ESC, to my surprise, is quite robust. I've dropped it at a height, dragged it on pavement, and got it wet. I even accidentally dropped a metal screw on it, and I guess the electronic parts that shouldn't make contact with each other got connected by the metal screw, and sparks and smoke ensue. Disconnected loopkey, and batteries and saw that the board looked burnt. Desperate to go for a ride, connected the ESC again, and still worked.

I used a lunch box enclosure with clip locks for easy access. I didn't use a BMS so I had to take out the LiPos every time for charging. And @pat.speed is right, charging can be a pain. If at the time I've known LiPos can be connected to a BMS, I would've done it, even if it was just for charging.

At 100kg, I was able go max 36-37kph on flat ground. I had no troubles going uphill, albeit you can only go as fast as 10kph on steeper hills.

My only complaint about this build/components are the brakes. I can't stress this enough, always use protective gear, be aware of your surroundings, and at minimum, learn how to do a foot brake. Going down a steep hill at speeds of 30-40kph, and you're on a collision course with a person, car, truck, so you want to stop - only 2 things can happen -  1) you pull the brake all the way for a full stop, it will work, but it will send you flying or 2) you gradually pull the brake you slow down a bit, but will never slow you down enough to a safer speed or a full stop even if the lever on the remote is fully depressed - use your foot brake. Another thing you can do is not to go full speed downhill. Use your brake halfway and don't pick up speed.

Uhmm... I guess that's it? I just wanted to give you an insight on my experience with this kind of build. Bottomline: It's a good build, a functional "toy" for commuting, and a cheap way to get into the hobby. Have fun!
```

---
## \#11 Posted by: edaemon Posted at: 2018-03-12T04:34:21.370Z Reads: 61

```
Thanks for the insight! I appreciate it. I'm glad to see this setup should work out, assuming I don't screw something up.

I live in a city with good biking infrastructure so I'm not too worried about the road quality -- I'll be on a flat bike path most of the time -- but I'll be careful with the brakes. This will be my first time on a skateboard since I was a teenager so I'll be taking it pretty easy anyway, but I appreciate the warning/advice.
```

---
## \#12 Posted by: Sippahodge Posted at: 2018-03-12T12:34:22.946Z Reads: 49

```
Make an enclosure with a lid and easy latch, so easy access makes charging lipos easy with a parallel board.
```

---
## \#13 Posted by: pat.speed Posted at: 2018-03-12T20:13:16.918Z Reads: 44

```
Yeah, I can slide my fattest case in and out and it's held by one bolt so it only takes about 20sec to do but it's still a bit annoying after a while
```

---
## \#14 Posted by: edaemon Posted at: 2018-03-15T21:59:32.290Z Reads: 36

```
I realized that the position I had the anti-spark switch in didn't seem right: the anti-spark would have to be connected for it to charge, and if it wasn't connected the charger might put power through the ESC. I moved the anti-spark in the diagram to where I think it makes more sense.

![Longboard wiring diagram|690x285](upload://2Qn33NmaFZCMuzs043Cct0wxSJ8.png)

Let me know if that's still not right...
```

---
## \#15 Posted by: edaemon Posted at: 2018-03-24T05:16:05.969Z Reads: 28

```
Realized again that I had the wiring incorrect, this time with the BMS. Just updating the diagram in case anyone comes across this thread when they're searching for how to wire things up...

![Longboard wiring diagram - BMS correction|690x285](upload://xDdolrE4bGYhql7vhz8Hi4yRqsV.jpg)

To explain for my own understanding, the BMS wiring has to go to all the pins on the bottom battery and only the middle four on the top battery.

I finally got my head around it when I realized the negative wire (top black one) on the bottom battery's balance lead and the positive wire (the red one) on the top battery have no voltage difference. The bottom negative wire comes after the last cell in the bottom battery and the top positive wire comes before the first cell in the top battery -- meaning there is no cell between those two wires. Obviously the BMS can't balance a cell that doesn't exist, so you have to skip the positive lead and use the second wire to catch the first cell.

If you're wondering how the last cell gets balanced, the negative balance lead and the actual negative lead (the big black wire) are wired together. If you test it with a multimeter the difference between them is 0V, so the BMS can use the negative lead connected to B- to balance the final cell in the top battery.

(I'm fully prepared for someone to show me how I'm entirely wrong...hopefully before the BMS arrives and I hook this up.)
```

---
