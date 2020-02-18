# First Build &#124; Seabiscuit &#124; Caliber trucks &#124; Turnigy Aerodrive SK3 &#124; DIY E-board Mounting kit &#124; ZIPPY Flightmax 8000mAh 6S1P 30C &#124; VESC

### Replies: 15 Views: 1478

## \#1 Posted by: Strawbs Posted at: 2016-06-13T22:48:00.370Z Reads: 154

```
For my first build I want to do something simple yet high quality.

Deck: 
http://www.rayne.com/product/savage-v2-longboard/

Trucks:
Caliber

Motor mount:
product/single-bolt-on-motor-mount-with-drive-wheel-kit/

Motor:
http://www.hobbyking.com/hobbyking/store/%5F%5F18181%5F%5FTurnigy%5FAerodrive%5FSK3%5F6364%5F190kv%5FBrushless%5FOutrunner%5FMotor.html

Battery x (2):
http://www.hobbyking.com/hobbyking/store/%5F%5F16228%5F%5FZIPPY%5FFlightmax%5F8000mAh%5F6S1P%5F30C.html

VESC:
http://www.ollinboardcompany.com/product/vedder-s-speed-controller

My confusion is mostly about batteries, and calculating the voltage.  If i buy 2 ZIPPY Flightmax 8000mAh 6S1P 30C (22.2v) will that make my total voltage 44.4v?  I am aiming for ~28mph top speed.  using Calc RC shown below,

<img src="/uploads/db1493/original/2X/4/45994d2c163982bc507a07c1a2844a6d0e86a311.png" width="573" height="443">

And how do I calculate the estimated mileage? 

Do you guys have any tips or suggestions regarding the parts I've selected?  What other misc. items may i need to have in order to complete this build?

Thanks!
```

---
## \#2 Posted by: Namasaki Posted at: 2016-06-13T22:55:02.354Z Reads: 140

```
If you connect those batteries in series then the nominal voltage is 44.4v but at full charge, it will actually be apx 50.2
Lipos always yield higher voltage when fully charged. As you drain the batteries, the voltage will drop slowly.
It is a good practice to stop and recharge them when they drop to the nominal voltage of 44.4 especially with Zippy batteries. Once the voltage drops to nominal it can go too low real fast. I ruined a brand new set of Zippy compacts that way.
Also I would recommend a larger gear on the motor. 13/36 is a little low on the gearing for a 190kv motor.
You can greatly improve top end speed and still have plenty of torque especially running 12s voltage with a 16/36 gear ratio.
The top speed that your calculator is showing is not realistic. It is most likely not adding in load factor.
I'm running dual motors 230kv on 12s with 16/36 gearing and 90mm wheels and top speed is only 30mph
190kv and 83mm wheels will render less top speed
```

---
## \#3 Posted by: Strawbs Posted at: 2016-06-13T23:01:22.825Z Reads: 127

```
How do I calculate the distance these batteries will take me before they hit nominal?

And if running in series will double my voltage will that affect the distance as well?
```

---
## \#4 Posted by: Jinra Posted at: 2016-06-13T23:01:49.011Z Reads: 125

```
It may be low, but he'd get decent torque on it. Though if you ever need to pull that much torque, the belt may slip. I'd go at least 14T with a 12mm+ belt with that setup.

@strawbs You can use nominal for calculations, just know that you'll be going faster on a full charge. Putting the pack in series will double the watt hours of that pack which will increase distance. Voltage doubles in series, Amp hours double in parallel. So yes, you'll have 44.4v nominal
```

---
## \#5 Posted by: Namasaki Posted at: 2016-06-13T23:02:58.474Z Reads: 121

```
There is a formula but i'm not sure how accurate it is.
I'm getting 12miles with 5000mah at 12s with my setup
you should do better with 8000mah
```

---
## \#6 Posted by: Jinra Posted at: 2016-06-13T23:04:22.205Z Reads: 120

```
Oh and you should hit about 20 miles with this pack, probably more if you're on mostly flat ground.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-06-13T23:07:07.792Z Reads: 120

```
Whether you run them in series or parallel you will get about the same distance. But in series you will get much more power and speed.
I have tested this theory by running mine both ways.
12s/5000
6s/10000
both configurations got me 12 miles
```

---
## \#8 Posted by: Strawbs Posted at: 2016-06-13T23:24:03.416Z Reads: 111

```
So it seems like series is the way to go.  I'm more concerned with top speed than distance.  What types of connectors do i need in order to run these in series and connect them to the VESC?  

As far as the electronics connections, this is how I understand it:

<img src="/uploads/db1493/original/2X/9/9b9ba7c162aa72e47d763c5d10d8efc09a9a26c9.png" width="690" height="185">

Is there anything I'm forgetting?
```

---
## \#9 Posted by: Jinra Posted at: 2016-06-13T23:26:29.085Z Reads: 106

```
You'll want a volt meter to measure your remaining battery life. You typically want an xt-60/xt-90/deans plug/bullet,etc for the VESC to battery and motor usually runs a 4mm/5.5mm bullet connector.
```

---
## \#10 Posted by: Strawbs Posted at: 2016-06-13T23:34:18.506Z Reads: 105

```
Yes volt meter sounds important.

Another thing I'm not understanding is ease of charging.  Off-the-shelf models just have a simple external plug to charge your batteries.  With the DIY route, will I need to remove the batteries from the housing each time I charge?  Is there some sort of connector I need to add for charging the batteries?
```

---
## \#11 Posted by: Jinra Posted at: 2016-06-13T23:36:31.176Z Reads: 102

```
You can add a charging port in the configuration, but you'll want to make sure those packs are balance charged. The easiest way is to just not do that and take the packs off to charge. Packs that have everything all-in-one including a charge port usually have a BMS to balance charge the cells.
```

---
## \#12 Posted by: Strawbs Posted at: 2016-06-13T23:46:05.044Z Reads: 103

```
The batteries sound like the biggest hassle.  

Parallel vs series, voltage, watt hours, BMS, balance charging... it's too much.

I might just go with the SPACE cell.  Seems like that takes care of all those things at once.
```

---
## \#13 Posted by: Jinra Posted at: 2016-06-13T23:50:57.568Z Reads: 98

```
Yep, the space cell is one of those all-in-one solutions. Shipping times are iffy on them though. People who ordered months ago have yet to receive them. You can try your luck ordering a similar pack from , though I'm not sure what they're delivery times are.
```

---
## \#14 Posted by: Namasaki Posted at: 2016-06-14T00:57:59.492Z Reads: 98

```
The Spacecell or similar type lithium ion battery pack is definitely the way to go if you want convenience. 
If you go with Lipos, charging time is shorter but it's recommended that you remove the batteries and put them in a fire safe bag while charging them and you have to monitor them while charging in case something goes wrong. 
With a Spacecell, you just plug it in and walk away. 
I would recommend spending a little extra for the fast charger.  1-2 hr charge. 
Lipos like the ones you listed are much thicker so ground clearance is more of an issue as well. 
My battery box is 2" thick so I have to be very careful about rolling over speed bumps.
```

---
## \#15 Posted by: torqueboards Posted at: 2016-06-14T01:52:50.041Z Reads: 96

```
I should have some ready to ship in about 1-1.5 weeks. 6s2p, 10s3p, 12s3p. Working on enclosures for them and they will be able to fit up to 2x ESCs + wiring.

Have some enclosures for ESCS + 2x3s or 2x6s. These enclosures should be easier to open which makes LiPo easier to deal with.
```

---
