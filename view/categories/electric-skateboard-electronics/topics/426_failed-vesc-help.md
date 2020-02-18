# Failed VESC help

### Replies: 38 Views: 4845

## \#1 Posted by: Moja Posted at: 2015-11-07T08:51:51.857Z Reads: 106

```
Whilst riding my VESC failed and is not showing any blue (on) LED's. I have tested the voltage on the connection going into the VESC and I am reading 40V. It wont connect to BLDC and is clearly not powering on. 

The key difference I have noticed is the PCB is very hot compared to my other working VESC, the heat is coming from the circular coiled piece in the centre of the VESC and is radiating throughout the components. What does this suggest? 

<img src="/uploads/db1493/original/1X/052805bf0136903d42798b7651f8d3ac5647bcef.JPG" width="690" height="460">
```

---
## \#2 Posted by: lowGuido Posted at: 2015-11-07T09:07:23.498Z Reads: 103

```
Hard to tell from the photo.  But looks like the microprocessor is cooked. (Its a bit blurred) There's a few other burn marks that im not sure where they came from and the soldering on the motor wires is horrible.
```

---
## \#3 Posted by: Moja Posted at: 2015-11-07T09:26:53.426Z Reads: 103

```
The marks on the microprocessor are just residue from hot glue, it seems fine. I got the soldering on the motor wires done "professionally" as I don't have much soldering experience, the connections are messy but they are solid and I cant see anything that is fried on the board.
```

---
## \#4 Posted by: jacobbloy Posted at: 2015-11-07T09:44:14.185Z Reads: 103

```
Please look on the other side on the vesc under the round thing you speak of, on that side of the vesc is a componant that regulates 3.3v. It have 3 pins and a little lug on the other side, the side with 3 pin stick a voltage problem on the right pin GRD I think and the probe the other 2 pins, one should have 5v coming from the DRV is you don't get the 5v then there could be a short there or DRV Buck is gone! The other pin would have 3.3v that goes to the mcu and other components, if you don't get 3.3v then it is the regulator or there is a short between GRD and 3.3v. Remember a volt meter measures voltage difference between the 2 probs to if you are getting 0v or 0.3v example then that could mean there is 3V going through your ground plain heating all componants including the little round componant you speak of more so because it is a coil.

If you can't see an external short internal shorts can happen in side say the mcu.
```

---
## \#5 Posted by: lowGuido Posted at: 2015-11-07T10:08:08.315Z Reads: 98

```
Its hard to fault find electronics from a photo.
Im just pointimg out the small things that i can see that may be a problem.
```

---
## \#6 Posted by: jacobbloy Posted at: 2015-11-07T10:14:14.490Z Reads: 93

```
And some time eyes are no help unless there is a big burn mark!
```

---
## \#7 Posted by: Blasto Posted at: 2015-11-07T16:25:15.221Z Reads: 88

```
Like @jacobbloy said, looks like you drv went tits up.

I replaced both of mine, seems to be the same batch as me (august)
```

---
## \#8 Posted by: chaka Posted at: 2015-11-07T17:10:57.566Z Reads: 87

```
I see some loose bits of solder in the image, sometimes after the boards have been through the re-flow oven they can have little loose balls of solder stuck to various areas on the solder mask. If the board heats up enough the flux residue holding those balls in place will soften, they can come loose resulting in a short if they come into contact with something.
```

---
## \#9 Posted by: Moja Posted at: 2015-11-08T03:27:48.293Z Reads: 90

```
Hi Jacob, 

 I did the test that you suggested, I got 5V on one pin and 0.01V on the other pin. You said the right pin is the ground pin, I assumed that is with the VESC upside down with the motor terminals on the left side. I now have the same problem with my second VESC and I'm pretty disappointed. On the first VESC I have also noticed a burnt out element under the mini USB port which can be seen in this image. I've been careful not to cause any shorts, there are no unwanted connections being made by solder spots. I believe these problems are a result of manufacturing issues, am I right?. 
 What is the suggested repair process for this? I bought the VESC's from the Enertion site. 

Thanks for the support, 
Moja. 

<img src="/uploads/db1493/original/1X/72dc802cd2bcf2920c5c3df5b6a843c2d1975e11.JPG" width="690" height="460">
```

---
## \#10 Posted by: lowGuido Posted at: 2015-11-08T04:01:26.241Z Reads: 81

```
well one of the Caps (C25) is burnt to a crisp there. I noticed that the USB port was a bit melted on the topside photo too. likely the cause of that. 
the little black rectangle with 3 tabs it the voltage regulator. It has probably died, it also looks a bit fried.
```

---
## \#11 Posted by: Moja Posted at: 2015-11-08T04:37:20.565Z Reads: 87

```
Here are some clearer images for reference. 

<img src="/uploads/db1493/original/1X/11e875ff25aa753ebe8b94b6aee2bedd118550a7.jpg" width="360" height="500"><img src="/uploads/db1493/original/1X/0a13af781ca82b217702205d089c500861156251.jpg" width="344" height="500">
```

---
## \#12 Posted by: lowGuido Posted at: 2015-11-08T04:56:53.920Z Reads: 86

```
what a schmozzle. there is solder everywhere shorted pins left right and centre..
pins 50 - 56 on the gate driver look shorted
pins 58 -61 on the micro also look shorted

either way its a mess.

and im not really sure about your Cap mounting either.. is all of your -ve voltage going through the caps leg?
```

---
## \#13 Posted by: Moja Posted at: 2015-11-08T05:21:57.350Z Reads: 85

```
Assuming the gate driver is at the top, there was a small piece of solder that I just removed easily. The shorts on the micro are mimicked on my other VESC which was working even with the short until not long ago, I assumed it may have been an intended connection as there is the exact same thing on the the other VESC. Would you point to this as the cause of the failure? 

As for the CAP mounting, yes the voltage is passing though the leg, in the above image the negative is disconnected.
```

---
## \#14 Posted by: jacobbloy Posted at: 2015-11-08T06:45:37.239Z Reads: 82

```
The regulator is TC2117, Google the data sheet, in solder the regulator, plug in an external 3.3v source from an stlink or arduino to one of the 3.3v pin and GRD see if things still get hot, then you know it's more then the just the regulator. Shorts can cause high current and voltage spikes enough to to blow a cap!
```

---
## \#15 Posted by: jacobbloy Posted at: 2015-11-08T06:47:07.200Z Reads: 84

```
Those 2 pins on the drv are meant to be bridged! On every one of vedders photos and every vesc Iv seen has it!
```

---
## \#16 Posted by: lowGuido Posted at: 2015-11-08T06:55:05.421Z Reads: 84

```
Ok. If its supposed to be that way then that's fine.
Still a mess tho.
```

---
## \#17 Posted by: Moja Posted at: 2015-11-09T05:24:36.878Z Reads: 79

```
Thanks for your support guys, I've decided I'm out of my depth here and I've passed the two VESC's onto a module repair service for inspection, hopefully its just the regulators and one C25 cap that needs replacing.
```

---
## \#18 Posted by: trbt555 Posted at: 2015-11-09T05:37:01.676Z Reads: 77

```
Where did you source the VESC from ?
It doesn't look like the kind of quality you'd expect when buying a $100 piece of kit.
```

---
## \#19 Posted by: Moja Posted at: 2015-11-09T05:45:24.429Z Reads: 79

```
From Enertion, Jason has kindly offered his support. Regarding quality, yes you are right.. however I understand it's still early stages for the VESC's (these are 4.7). Provided the support is there I am still a happy customer :)
```

---
## \#20 Posted by: onloop Posted at: 2015-11-09T06:51:04.987Z Reads: 80

```
*Actually these things cost more than $100...*

The problem is that VESC can fail for many reasons, especially in its raw form without no case!, one of the reasons they can fail is shorting them out accidentally - I did this to two VESC :frowning: - it's simply bad luck! and not covered under warranty.

**The warranty I offer is only good if the fault is proven to be a manufacturing fault.**

From the 250 units sold by me so far, since the BETA program started, it actually seems the failure rate is fairly low! I am not sure what an acceptable failure rate is with electronics but so far it seems ok.

Originally I had people return the first batch because of the wrong capacitors being used during assembly, not necessarily because of faults - those vesc actually did worked well with the wrong caps.. Those people got their money back
The 2nd batch - all made to spec -  maybe just 2 or 3 out of 100 (which is what batch @moja has @cmatson) - these guys will get a repair or replacement. whatever is cheapest/quickest
This last batch it's too early to know if there is problems. hopefully none!

Most people's VESC problems can be solved/repaired by replacing a few parts that often cost much less than $5 - the difficult part is the soldering job and man hours, so REPAIR is what i offer first..depending how/who carries out the repair i might offer store credit or cash refund etc to cover cost of repair..

Like I said these things are super expensive and I make next to no margin out of selling them, so of course I am reluctant to straight swap these for people - especially when I have not stock of them to swap with.... So in the long run if failure rates get too high I will simply stop having them made as it won't be viable. 

However, so far i think it's been fairly acceptable in terms of reliability & failure rates & most people are being reasonable when it comes to solving problems. ALSO I am not a PCB technician OR Software engineer so don't get shocked when i say i can't fix it! I can't because i don't know how! I also can't fix the dead ones in a box on my bench so I'm out of pocket on those ones too.

At the end of the day, If we all work together we can find viable solutions... Hopefully this melbourne business can repair the moja VESC, if they can at a reasonable price i will contact them and try to negotiate a repair contract so that i can offer better warranty & service to everyone through the form of repair. Maybe eventually I could even start offering extended warranties OR replacement warranties!

For folks in the us with VESC i know that @chaka has done some repair work. Contact him to get a quote & ill pay the repair cost. if he is obliging. My general concept is to ensure no one is out of pocket if their vesc fails due to manufacturing faults.

Eventually VESC won't be considered a BETA and then everyone can expect much better warranty & service but in return likely pay a small premium more per unit for that.

I hope this make things clear to anyone wondering about buying a vesc!
```

---
## \#21 Posted by: trbt555 Posted at: 2015-11-09T11:19:46.271Z Reads: 79

```
@onloop Your pragmatic and service-oriented attitude is commendable.
Could you shed some light on the kind of testing that is done on the VESC before they are issued to customers ?

I'm new to the scene but so far I've seen only VESC's coming from either Australia or the US, I'd love to see them become available from a European source as well and I might even try to source them from a local supplier myself. 
Any tips/recommendations ?
```

---
## \#22 Posted by: chaka Posted at: 2015-11-09T14:02:01.605Z Reads: 79

```
FYI, I offer a "bare bones" VESC for $100 with free US shipping so they are available at that price.

I also manufacture them "in house" so repairs are a snap. 

"BareBones"
<img src='/uploads/db1493/original/1X/c8207c3ee94dde1bf7afc8dade8ed02fd728a799.jpg'>
```

---
## \#23 Posted by: lowGuido Posted at: 2015-11-09T22:47:34.604Z Reads: 78

```
I know that its been stated that the gate driver pins 50-56 are supposed to be shorted, but the picture of @chaka 's VESC doesn't appear to be, and is a lot neater.
<img src="/uploads/db1493/original/1X/a7b04071f297c625a7d564ff835b91a60abbfe23.jpg" width="415" height="123">
```

---
## \#24 Posted by: chaka Posted at: 2015-11-10T01:33:47.384Z Reads: 77

```
If you take a look at the gerber files using KICad those pins are joined under the solder mask. It looks like a little clean up on the micro processor and a fresh tantalum capacitor might fix this unit. It is hard to say what cooked that cap, I see it was covered with a bit of foam. Could it have overheated?
```

---
## \#25 Posted by: kai Posted at: 2015-11-10T03:53:42.199Z Reads: 77

```
@chaka do you offer repair service on enertian vesc? or will you only repair the barebones vesc?
```

---
## \#26 Posted by: chaka Posted at: 2015-11-10T07:09:23.019Z Reads: 74

```
I suppose I could but it will have to wait till things settle a little bit, I have to take care of my customers first.
```

---
## \#27 Posted by: trbt555 Posted at: 2015-11-10T12:25:57.282Z Reads: 73

```
Lead time is still 2 weeks ?
```

---
## \#28 Posted by: kai Posted at: 2015-11-10T14:56:47.597Z Reads: 70

```
i am assuming lead time is from time of order till shipping? or receiving?
```

---
## \#29 Posted by: chaka Posted at: 2015-11-10T15:49:47.688Z Reads: 72

```
Yes, it is still 2 weeks. That time is based on ordering PCB's from Hackvana. I am going to order a few hundred for the next batch but that will probably go just as quick.
```

---
## \#30 Posted by: elkick Posted at: 2015-11-11T10:04:50.859Z Reads: 68

```
@chaka and @jacobbloy: I'm assembling a VESC but cannot find R15 in V4.10 anymore compared to V4.7. 
Its a resistor 330kOhm at R15. Was it just omitted and Benjamin forgot to remove it from BOM V4.10?
```

---
## \#31 Posted by: chaka Posted at: 2015-11-11T14:44:27.389Z Reads: 67

```
Yes, it was removed.
```

---
## \#32 Posted by: elkick Posted at: 2015-11-11T15:41:51.105Z Reads: 71

```
Thanks Chaka, that's good to know.
```

---
## \#33 Posted by: trbt555 Posted at: 2015-11-14T18:22:21.309Z Reads: 74

```
@onloop, no testing ?
```

---
## \#34 Posted by: onloop Posted at: 2015-11-14T21:02:20.096Z Reads: 78

```
They get powered on. They get firmware loaded. They generally work or they don't.

I'm happy to do more testing though. I can do motors spin testing. What else do you want done? You probably looking at about some additional surcharge though.
```

---
## \#35 Posted by: lowGuido Posted at: 2015-11-14T21:19:39.759Z Reads: 80

```
I recieved my 4.10 VESC from enertion the other day. I havent had time to test it yet but on appearance it looks a lot neater than the OP's
<img src="/uploads/db1493/original/1X/e226e6fdc3044b374e450c7878415f99f661eea7.jpg" width="281" height="500">

however as mentioned in another post the black lead from PCB to Cap board is about 4 or 5 mm too short which brings the live rails alarmingly close to the servo pins. i'l be re doing that one before I do any testing.

oh.. for what its worth I understand the need/want to get the power rails as close to the FETS without having to potentialy make the board larger with fat tracks. but leads connecting to the middle of a board is poor design in my books. (not pictured) on the otherside of the board the +ve lead runs right over the 5v pin on the CANBUS connector. its not shorting yet, but I bet a couple hundred ks on a skateboard will be different.

keeping in mind that this is essentially a BETA product, and its still in the teething stages. I wouldn't expect any warranty to be offered and all work should be performed by a qualified technician.
```

---
## \#36 Posted by: trbt555 Posted at: 2015-11-15T08:10:01.969Z Reads: 66

```
Personally I wouldn't mind paying extra for the knowledge that the VESC's I'm receiving have actually run motor current.
I've PM'd you.
```

---
## \#37 Posted by: jacobbloy Posted at: 2015-11-15T09:17:48.052Z Reads: 67

```
Testing is fine but just plugging in every vesc and loading firmware and bootloader takes time, Iv written a script to cut the process in half but just plugging it in and pressing enter and parameters for ppm and enertion motors are preset. To do 120 vesc you can imagine can take a few hours, then to plug in a motor and pin test we are taking about longer because the time loading isn't programming its plugging in and unplugging and plugging the next in.
```

---
## \#38 Posted by: Batou Posted at: 2015-11-15T22:00:09.826Z Reads: 69

```
Hi all! I also received the VESC 4.10 from Enertion. The overall quality looks good, but as @lowGuido I am a bit worried about the red and black leads at the center of the PCB. 
One of the component has already cut through the insulation of the black wire and the copper is visible. As for the red wire it is indeed very close to the 5v pin. 
For now I won't plug the VESC as it is. I don't like it, but I think I will try to re-solder these wires perpendiculary to the PCB. Also I will try to make a small PVC enclosure. Apparently a lot of VESC failures are due to shorts so I don't want to take a lot of risks.
```

---
