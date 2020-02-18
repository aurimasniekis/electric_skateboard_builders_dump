# How should my charging solution be?

### Replies: 29 Views: 1256

## \#1 Posted by: VAEsk8 Posted at: 2018-01-02T19:03:22.137Z Reads: 174

```
Hi! I'm kinda new to the eskate community, and I've been doing a lot of research. The one place where I get a little lost, is when it comes to the charging solution. Im thinking about using 2x 4s 5000mah 20c Lipo batteries and wire them in series. Then, wire the balance cables into a bms, the negative of the batteries aswell (i think, correct me here please). Then to the charger, I need a 33,6V balance charger, with a charging port. 

Links provided:
Batteries: ( https://hobbyking.com/en_us/zippy-flightmax-5000mah-4s1p-20c.html?___store=en_us )
Charger: ( https://www.ebay.com/itm/Intelligent-Smart-33-6V-2A-Charger-for-8S-28-8V-29-6V-Li-ion-Li-Po-Battery-EU/321471399664?_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20160727114228%26meid%3D3a6cde1467ce4e37be776d1146e82359%26pid%3D100290%26rk%3D1%26rkt%3D1%26sd%3D321471399664&_trksid=p2060778.c100290.m3507 )

Charging port: ( https://www.amazon.com/HDVDTM-10pack-5-5mm-Pigtail-Female/dp/B00CUKHN0S/ref=pd_sbs_421_2?_encoding=UTF8&pd_rd_i=B00CUKHN0S&pd_rd_r=YJYNH6H3WD0J6Y4Z6FNY&pd_rd_w=vhs4Z&pd_rd_wg=dIYv7&psc=1&refRID=YJYNH6H3WD0J6Y4Z6FNY ) or ( https://www.amazon.com/5-5mm-2-1mm-Female-Connector-Camera/dp/B005CMP434?ie=UTF8&amp;psc=1&amp;redirect=true&amp;ref_=oh_aui_detailpage_o01_s00 )

BMS: ( http://www.batterysupports.com/28v-29v-30v-30a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-262.html )
```

---
## \#2 Posted by: MysticalDork Posted at: 2018-01-02T19:17:16.189Z Reads: 157

```
Looks good, with a few caveats. 20c is a little low for a 5000mah pack, you'll end up with significant voltage sag and it's less than ideal for the health of the batteries. 30c or greater is recommended. 

The BMS you linked is only good for 30 amps, so unless you're willing to limit yourself to that, you'll have to bypass it for discharge, or get one that can handle more power.
```

---
## \#3 Posted by: b264 Posted at: 2018-01-02T19:17:38.515Z Reads: 146

```
First you need to decide whether you'll run your BMS in discharge mode (and charge mode also)  --  or bypass it - and only use it for charging.

That BMS is probably overkill for running in bypass mode, and probably not powerful enough for running in discharge mode, you'll want 80A or more for that for dual motor or 40A - 50A for single motor.  Unless you run in bypass, then it doesn't matter
```

---
## \#4 Posted by: VAEsk8 Posted at: 2018-01-02T19:24:06.316Z Reads: 124

```
Hi, thanks for your reply! I'm thinking to use the BMS for charging only. Then, are there any problems with the solution? The charging female port ok? Do you know if it has a limit on how many amps or volts in can handle? Should I use xt90's as connectors? Thanks!
```

---
## \#5 Posted by: VAEsk8 Posted at: 2018-01-02T19:25:29.152Z Reads: 121

```
Thank you for you reply! What do you mean with voltage sag? I thought the 20c only means that the batteries will output 5aH * 20c = 100 Amps.
```

---
## \#6 Posted by: MysticalDork Posted at: 2018-01-02T20:16:51.304Z Reads: 105

```
Theoretically that's true, but the battery manufacturers tend to overstate the actual real-world capability of their cells. It's better to have lots of buffer and not need it, than to be constantly running the battery ragged.
```

---
## \#7 Posted by: VAEsk8 Posted at: 2018-01-02T20:30:42.373Z Reads: 96

```
Okay, thanks! What do you think about the charger and charging port tho?
```

---
## \#8 Posted by: b264 Posted at: 2018-01-02T20:51:26.303Z Reads: 95

```
That charger jack is the correct jack, but it's loose on a wire.  It's probably better to get the ones that mount with a nut in a case
```

---
## \#9 Posted by: VAEsk8 Posted at: 2018-01-02T21:48:45.712Z Reads: 88

```
So you mean I should buy this one? https://www.amazon.com/5-5mm-2-1mm-Female-Connector-Camera/dp/B005CMP434?ie=UTF8&amp;psc=1&amp;redirect=true&amp;ref_=oh_aui_detailpage_o01_s00
```

---
## \#10 Posted by: b264 Posted at: 2018-01-02T21:56:26.381Z Reads: 85

```
No, more closer to [these](https://www.ebay.com/itm/152795579004)
```

---
## \#11 Posted by: VAEsk8 Posted at: 2018-01-02T22:21:04.037Z Reads: 78

```
That one has a "Contact rating-0.5A 30V DC". Aswell as it doesn't provide where the positive, negative and ground goes.
```

---
## \#12 Posted by: b264 Posted at: 2018-01-02T22:23:22.977Z Reads: 77

```
I mainly meant that style and not that specific one.  [This one might be closer](https://www.ebay.com/itm/361449834855) but curiously it's 2.1mm plus or minus 25.4mm, that's a pretty big margin of error.  Sounds like the seller doesn't know what's going on...
```

---
## \#13 Posted by: VAEsk8 Posted at: 2018-01-03T10:46:21.222Z Reads: 64

```
I dont think I will get a sag if I use the tb vesc with it, will I? It has a 50A max
```

---
## \#14 Posted by: Acido Posted at: 2018-01-03T11:34:15.924Z Reads: 68

```
Dude stuff like this doesnt matter, plug the charger to this then just measure it with an multimeter if the voltage is in - its the other way around and boom you know where is plus and where is minus
```

---
## \#15 Posted by: Acido Posted at: 2018-01-03T11:34:55.793Z Reads: 65

```
Voltage sag has nothing to do with esc's
```

---
## \#16 Posted by: Acido Posted at: 2018-01-03T11:35:23.731Z Reads: 64

```
Probably just a typo
```

---
## \#17 Posted by: MysticalDork Posted at: 2018-01-03T15:35:33.689Z Reads: 56

```
You'll always get some sag, it's just a question of how much is acceptable to you and the batteries. 5ah 20c is right at the fine line of "barely acceptable" to me, but it's probably fine.

Bear in mind that I have a tendency to overbuild my stuff.
```

---
## \#18 Posted by: VAEsk8 Posted at: 2018-01-04T12:13:20.883Z Reads: 49

```
So if I use 2x 5s 5000mah 20c batteries in series to a 10s battery, it would be nice?
```

---
## \#19 Posted by: MysticalDork Posted at: 2018-01-04T15:35:52.496Z Reads: 52

```
Like I said, 5ah 20c is barely acceptable in my book, no matter how many in series. If I were you I'd either increase the C rating to at least 25 or 30, OR increase the Ah of the pack, either by using larger cells, or putting some in parallel.
```

---
## \#20 Posted by: mmaner Posted at: 2018-01-04T15:46:38.823Z Reads: 55

```
[quote="VAEsk8, post:18, topic:42581, full:true"]
So if I use 2x 5s 5000mah 20c batteries in series to a 10s battery, it would be nice?
[/quote]

I wont be a torque monster or speed demon, but it will work.  Depending on weight and terrain you should be able to hit 20 mph and handle some small grades.  The best lipo solution is using 2s lipo packs in a series of x5 to make a 10s pack.  I built one using 20c lipos and it was a beast.  Very fast and torque to the point that I could leave thane on the ground.  Its pretty inexpensive too.

Check out this thread, it will tell you all you need to know about Lipo packs.  @Namasaki is a genius ...
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014

Here's something I did just for the hell of it :slight_smile:. 
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/415?u=mmaner
```

---
## \#21 Posted by: VAEsk8 Posted at: 2018-01-04T17:36:45.617Z Reads: 43

```
Only 20mph? According to esk8 calc it should be able to hit 25mph. Is it because of the discharge rating? I will bypass this in the bms btw. I dont think I want 5x 2s lipos, because it will take up alot of space, and is more expensive than just buying 2x 5s lipos. Im not sure how many people who have used bms with their lipos tho.
```

---
## \#22 Posted by: mmaner Posted at: 2018-01-04T17:42:08.495Z Reads: 43

```
You might hit 25, who knows.  I have found that I usually come in at 80%.  Lots of people have used a BMS with lipos, look at the links I sent you and search.
```

---
## \#23 Posted by: Namasaki Posted at: 2018-01-04T18:25:28.139Z Reads: 42

```
[quote="VAEsk8, post:21, topic:42581"]
Only 20mph? According to esk8 calc it should be able to hit 25mph.
[/quote]

Esk8 calcs do not take into consideration voltage sag. 
Using 5000/20C packs at 10s, you will have voltage sag that will reduce your max speed and range. 
What I recommend is a minimum of 60C at 5ah and even then you will have a small amount of sag. 
With 20C at 5ah you might also have issues with your packs heating up and getting puffy.
```

---
## \#25 Posted by: VAEsk8 Posted at: 2018-01-04T20:07:38.168Z Reads: 39

```
Okay, thanks! But my wallet is obviously not as big as yours, and the 60c batteries cost a lot more. Still wouldnt want heated and puffy batterypacks. Mabye ill go for 30c. Or a 8s system instead. The thing is just that there are few people using 8s, and therefore few brick chargers with 8s (33,6v). And then have a matching charging port to that brickcharger etc. BMS too :confused:
```

---
## \#26 Posted by: skelstar Posted at: 2018-01-04T21:14:19.618Z Reads: 35

```
I use (and started with) 2x 5s 5000mAH batteries (20C) and I have found it fine. I'm a bit careful/timid on my board (can't afford to crash) but go up some hills while commuting. 

I generally cruise at about 22km/h (I know that's slow, but I'm not limited by the batteries).

I also have my motor current limited to 20A in the VESC setup (running a 5035 125kV motor)... more than enough for me.

I would only change the setup for size/stealth/asthetics reasons.
```

---
## \#28 Posted by: VAEsk8 Posted at: 2018-01-04T21:45:50.091Z Reads: 34

```
Nice dude! What discharge rating does the batteries have? :)
```

---
## \#29 Posted by: skelstar Posted at: 2018-01-04T21:47:59.197Z Reads: 34

```
Updated post. 20C...

Thought they might be a bit low (in the month and a half that they took to get here) but I had nothing to worry about.
```

---
## \#30 Posted by: Hummie Posted at: 2018-01-04T21:48:02.010Z Reads: 31

```
motor current isn't decided by the battery.  only the "battery amps" are true amps coming from the battery.  So you could set your vesc to have a miniscule 20 battery amps and 120 motor amps and still only pull 20 amps max from the battery yet still have great low speed torque.
```

---
## \#31 Posted by: skelstar Posted at: 2018-01-04T21:49:13.670Z Reads: 33

```
Totally. I get that. I figured that there would be some capacity stored in the VESC and tutorials I had seen suggested doing the limiting at the motor rather than battery.

I wanted to dull the acceleration for a while as I learn how to ride the board with motors.
```

---
