# Recommendation for purchasing VESC hardware, today

### Replies: 19 Views: 1495

## \#1 Posted by: mfidelman1 Posted at: 2017-07-18T19:16:22.969Z Reads: 172

```
Hi Folks,  

I'm putting together a motorized "mobility walker" (think a very wide e-board with hand rails) - designed to run at very slow speeds.  Busily accumulating parts to experiment with (e.g., hub motors with reasonable performance at low RPMs).  Zeroed in on a couple of custom winds that Hummie is putting together, and the Maytechs.

I've just turned by attention to VESCs - I expect to be running FOC mode and relatively high amps.  The new FOCBOX looks like a good unit, but it's not clear they're shipping (taking pre-orders).  Can anybody suggest something that has the latest chips, can handle high amps, supports FOC, is reasonably reliable, has a solid vendor, and will actually ship if I place an order?  (If it makes any difference, I'm going to use a pair of them, or 2 channels, and tank-mode differential steering - i.e., turn left by sending power to the right-hand motor.  I also expect to use hard-wired controllers - don't need wireless.)

Thanks much, Miles Fidelman
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-18T19:18:34.496Z Reads: 171

```
Ollin, Axle, and Enertion all make higher spec'd VESCs.

Ollin is shipping, but may take a couple weeks to get them out the door

Axle is not taking orders right now

Enertion's FOCBOX is shipping but may also take a couple weeks. However, there are a couple threads are here from other users selling new FOCBOXs

http://www.electric-skateboard.builders/t/new-vesc-x-for-sale-us-free-shipping-price-reduction/19089/150
```

---
## \#3 Posted by: Jebe Posted at: 2017-07-18T19:36:18.274Z Reads: 154

```
ollin or trampa
```

---
## \#4 Posted by: gliz5714 Posted at: 2017-07-18T19:39:22.580Z Reads: 150

```
I talked to Enertion chat a few days ago and if you order today, the shipment will "likely" go out in mid/late August. Sounded like they have one wave going out in the next week and it takes ~3-4 weeks to fill each consecutive shipment.
```

---
## \#5 Posted by: mfidelman1 Posted at: 2017-07-18T19:58:46.801Z Reads: 136

```
Any opinions on the TORQUE BLDC devices, or the Maytech VESCs?
```

---
## \#6 Posted by: gliz5714 Posted at: 2017-07-18T20:06:15.580Z Reads: 131

```
AFAIK DYEe's Torque VESC is the base VESC - not upgraded with exception to Vedders recommendation (hence the lower price vs FOCBOX/Ollin).  Not sure what that means in terms of your board, if it can handle the higher Amps is up to your usage.
```

---
## \#7 Posted by: mfidelman1 Posted at: 2017-07-18T20:24:46.824Z Reads: 120

```
Thanks.  Very useful feedback.
```

---
## \#8 Posted by: detroitwheelin Posted at: 2017-07-18T20:35:34.220Z Reads: 118

```
Why are you planning to run “high amps” for a slow mobility walker solution?  What motors are you planning to use?  What is the rated max amperage on the motors?
```

---
## \#9 Posted by: trampa Posted at: 2017-07-18T20:39:50.952Z Reads: 124

```

I would recommend to go for VESC Six. Benjamin Vedder spent the last two years making the new Software VESC-Tool and the new firmware for VESC Six. Three shunt measuring will make nearly any motor run perfectly smooth in FOC. 80A continuous is no issue. 

http://www.trampaboards.com/vesc-6-complete--vedder-electronic-speed-controller-trampa-exclusive-p-24166.html

We do the official release of the HW together with Benjamin Vedder. So its guaranteed 120% top spec and Vedder approved.

We will get the next batch in a couple of days. Estimated shipping is first week of August, after programming and testing each device.

Frank
```

---
## \#10 Posted by: rpn314 Posted at: 2017-07-18T20:52:49.108Z Reads: 120

```
[quote="mfidelman1, post:5, topic:27974, full:true"]
Any opinions on the TORQUE BLDC devices, or the Maytech VESCs?
[/quote]

I strongly discourage the Maytech VESC, especially for high current and/or FOC. @torqueboards's VESCs are good though. They do have slightly upgraded parts compared to the original Vedder BOM. If you can wait for it, a VESC 6 would be a very good option as well.
```

---
## \#11 Posted by: mfidelman1 Posted at: 2017-07-18T20:59:02.034Z Reads: 109

```
I've been looking at several different motors, with peak amperage up to about 30 amps.

I expect to be running at 3-5mph max speeds, which is at the really inefficient end of a DC motor's power curve.  That says high amps to me.  I won't really know for sure until I actually try things out.  So... I'd rather over-specify all the electronics, than have stuff melting or blowing up.
```

---
## \#12 Posted by: trampa Posted at: 2017-07-18T21:10:10.045Z Reads: 106

```
[quote="mfidelman1, post:11, topic:27974"]
5mph
[/quote]

Your Project sounds interesting. Try to use gearing and skip the hubs. Precise sensors are what you want. E.g. AS 5047 magnetic sensors. A very smooth startup is essential I guess. Benjamin implemented Hall, ABI and AS 5047 in the new software. 

Frank
```

---
## \#13 Posted by: mfidelman1 Posted at: 2017-07-18T21:15:02.227Z Reads: 102

```
I know - gearing is a lot more efficient.  But also requires more maintenance.  I'm building this for a 97-year old guy who wants nothing to do with things like tightening belts, or cleaning road dirt out of gears.  So I'm going to see if I can get the performance and battery life that I need (say, an hour of runtime on a charge) out of a hub motor, before resorting to gearing.  (The other approach is to use something like a hoverboard motor, that's designed for lower speed operation.  But the weight gets rather high.)

Can you say more about the sensors?  The motors I'm looking at have hall effect sensors built in.
```

---
## \#14 Posted by: Jinra Posted at: 2017-07-18T21:16:16.762Z Reads: 102

```
VESC has hall sensor support, you just need the right JST-PH 2.0mm pitch header to plug it in. You can run FOC sensored for quiet, smooth performance.
```

---
## \#15 Posted by: trampa Posted at: 2017-07-18T21:20:25.908Z Reads: 100

```
Hall is not very precise. 97 years is probably in the category of AS5047. These are magnetic sensors. A diametral magnetized magnet spins above a chip that reads out the angle value very very precise. So you know exactly where the rotor is. This helps to spin up with precision and lots of torque. 

Frank
```

---
## \#16 Posted by: mfidelman1 Posted at: 2017-07-18T22:10:48.334Z Reads: 98

```
So how does that actually work.  Where do you mount the magnet & the chip?
```

---
## \#17 Posted by: trampa Posted at: 2017-07-19T03:56:55.286Z Reads: 92

```
The magnet on the axle, the chip in front of it. For a hub motor that is somehow stupid. So in that case you need to use the build in hall sensors.

Boosted boards use the AS5047 as far as I know. Send me a mail, and I send you a pic.

frank@trampaboards.com
```

---
## \#18 Posted by: ATLesk8 Posted at: 2017-07-19T04:04:39.673Z Reads: 90

```
I've had very good customer service and reliability from Dexter and his Torqueboards not-vescs and other products as well. They're usually actually available to ship which is nice as well. I do also have 2 focboxes on the way from a group buy so we'll see how those compare to the 5 Torqueboards notvescs.
```

---
## \#19 Posted by: mfidelman1 Posted at: 2017-07-19T13:08:49.234Z Reads: 76

```
Thanks!  email is mfidelman@meetinghouse.net
```

---
