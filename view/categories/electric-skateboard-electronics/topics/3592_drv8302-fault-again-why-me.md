# DRV8302 fault again&hellip;.(why me?)

### Replies: 23 Views: 5203

## \#1 Posted by: gamma2 Posted at: 2016-05-21T08:43:40.078Z Reads: 307

```
Finally got the board running. First couple days on all stock voltages just feeling it out. Learned very quickly that smooth trigger input is key. Third day I upped the settings to 70 amps. Tried out FOC. Everything's peachy. End of the fourth day and I notice trigger input isn't being registered completely. Figured my controller is running low. As the day progresses the symptoms get worse and worse. Eventually, no response at all. Hook it up to my laptop and what do you know but another DRV8302 fault code. I really want to love this hobby; those first few days were the time of my life. But it's crazy when something custom made for our purposes and used not very much at all beyond stock settings, has managed to be broken for 5x the amount of time its been working for me. The worst part is, my university makerspace is having an event in two weeks and asked me to showcase alongside my board, but I guess that won't be happening. Is there any hope in me purchasing and soldering on a new DRV8302 or should I just go back to the source for repairs?

Thanks guys.
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-05-21T08:55:19.528Z Reads: 302

```
Well in this case i thing the problem was the FOC...
It can do some crazy stuff if not perfectly set up, and does kill many vescs in combination with some specific motors...

Here is a discussion on the @chaka VESC thread:
http://www.electric-skateboard.builders/t/ollinboardcos-high-output-vesc/636/110?u=flatsp0t
```

---
## \#3 Posted by: gamma2 Posted at: 2016-05-21T08:57:07.470Z Reads: 284

```
I guess I worded that weirdly. Tried out FOC for like all of 15 minutes and then switched back because I like the motor noise. I don't think FOC would have been responsible. Do you feel its worth the effort to try swapping a new DRV chip in or is it most likely going to be multiple issues?
```

---
## \#4 Posted by: flatsp0t Posted at: 2016-05-21T09:16:22.001Z Reads: 277

```
Well, i dont know how good you are in pcb soldering.

And i would ask @chaka or @jacobbloy if it is likely that orher components are also damaged.
```

---
## \#5 Posted by: dogeatgod Posted at: 2016-05-21T10:00:03.002Z Reads: 267

```
It’s not just you.

Damaging DRV chips whilst not seeming to do anything wrong is so so so frustrating – I wish I had sent my first VESC back to supplier, but at that time supplier did not have the knowledge or facility to troubleshoot and rectify the problem. As the technology was new and I thought of myself as a BETA tester I accepted that this happens and that future development would make the product more robust – I purchased another VESC and had the DRV of the first replaced in UK…VESC is still dead. 

I also had tried to run FOC and then returned to BLDC operation.

Possible outcomes replacing DRV yourself

1)	You are blessed - instantly solves problem.
2)	You are normal – once again DRV8302 fault, you’re back at square one 

As I replaced the chip myself I can’t expect the supplier to accept any liability so further cost of investigation and fix will be down to me.

If I purchased a VESC recently and a DRV fault appeared, providing that I had been using within acceptable parameters, it would go back to supplier for diagnosis.
```

---
## \#6 Posted by: 3sly Posted at: 2016-05-21T12:28:11.569Z Reads: 245

```
I've read around that FOC can be the culprit. But i've also read that once it works in FOC it isn't recommended to go back to BLDC as that's when the problems begin for many. If I could just find the link...
```

---
## \#7 Posted by: paragon Posted at: 2016-05-21T13:20:06.673Z Reads: 240

```
I've heard that a lot of these issues occur after disabling FOC.
```

---
## \#8 Posted by: 3sly Posted at: 2016-05-21T13:41:02.271Z Reads: 234

```
Jep me to, switching back from FOC to BLDC seems to cause alot of problems. Since @gamma2 and @dogeatgod dit just that, it might be true.
```

---
## \#9 Posted by: Vito Posted at: 2016-05-21T13:48:26.135Z Reads: 232

```
I kill my both vesc's after setting foc. Before i try foc they was running perfectly bldc mode. I think foc is not that relieble or dosen't work well with some motors...
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-05-21T14:11:19.203Z Reads: 229

```
Check the RPM max setting, it was the cause of many of my problem.

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#11 Posted by: Namasaki Posted at: 2016-05-21T14:23:25.188Z Reads: 234

```
Have you considered trying the Torquesboard 12s Esc?
I'm using them on my dual setup. The are very simple to set up. 
I run mine at 100% power with 12s Lipo for max power. Control is very good in my opinion. 
I run them hard and they remain very dependable. 
I can go 10 miles charging up and down long hills and never have to stop to cool down. Just when my legs get tired. They never cut out on me even when going up steep hills.
```

---
## \#12 Posted by: Kaly Posted at: 2016-05-21T23:16:11.338Z Reads: 216

```
My 2 cents here 

I have been trying the FOC and decide to investigate, this is the observation so far : 

Running FOC full throttle on 39.5 V for 3 min and monitoring temperature on the BLDC tool. the temperature of the PCB in particular rises faster than the other components, the FETS will eventually cach up to the chip but it seems that the DRV8302 is the one getting destabilized first (by the temperature) causing a heat runaway effect eventually killing the chip. 

I have istalled a 35mm fan on the side of the VESC to air cool the system and it works wonders the temperature have been keep under control preventing the runaway effect mention before. 

In the short run I'll keep the fans up.  it's working and I'm enjoying the excellent torque and silent if this device. 

By the way i did the same with the TB 12A ESC  I burn one and after the autopsy I confirm that it was the issue was the FETS got over heated and the solder melted just enoug that cause a short and provoke  a runaway effect that kill that device.
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2016-05-21T23:48:03.286Z Reads: 198

```
Nice simple analysis and tip.... Well done mate
```

---
## \#14 Posted by: kingbing Posted at: 2016-05-22T00:30:24.972Z Reads: 195

```
Could you post pictures of the fan on your Vesc? that would be helpul.
 thanks mate
```

---
## \#15 Posted by: Kaly Posted at: 2016-05-22T00:41:33.574Z Reads: 195

```
I'll do when I get home
Until then just one of this 

http://m.ebay.com/itm/High-Speed-5V-Dupont-Connector-3-5cm-35x10mm-35mm-Mini-DC-Brushless-Cooling-Fan-/221950608792?hash=item33ad498598:g:xlwAAOSwAKxWVWB0

position side ways so it can blow air cool all the FETS. It can be power by the VESC too
```

---
## \#16 Posted by: gamma2 Posted at: 2016-05-22T04:04:21.063Z Reads: 188

```
So it sounds like FOC is the culprit. Ugh. I guess I might as well try with a DRV replacement. Does anyone have a link to place that will ship it relatively quickly? I looked on DigiKey but there's a couple different types available and I'm not sure which I need.
```

---
## \#17 Posted by: chipoi84 Posted at: 2016-05-22T04:12:43.151Z Reads: 189

```
http://www.mouser.com/ProductDetail/Texas-Instruments/DRV8302DCAR/?qs=sGAEpiMZZMs0JQbjv5Ir6h9FrTVstRQs
```

---
## \#18 Posted by: jacobbloy Posted at: 2016-05-22T13:18:32.785Z Reads: 181

```
Iv had so many drv faults some times it's just the chip it's self, maybe why ti are fasing them out.
```

---
## \#19 Posted by: kingbing Posted at: 2016-05-23T00:04:21.492Z Reads: 174

```
Thank you. Waiting on the pics!!
```

---
## \#20 Posted by: dogeatgod Posted at: 2016-05-23T08:47:49.015Z Reads: 173

```
<img src="/uploads/db1493/original/2X/0/03a20f6b45baea5e448104e43aa23ae22d29d816.JPG" width="666" height="500">
<img src="/uploads/db1493/original/2X/c/c7671276e72d7a838fec6f0bb63ec1d93d706d39.JPG" width="666" height="500">

Not sure if that helps - pretty easy to fit
```

---
## \#21 Posted by: kingbing Posted at: 2016-05-23T15:57:09.146Z Reads: 167

```
Yes this does help a lot. Thanks for your input.
```

---
## \#22 Posted by: sprocket12 Posted at: 2016-08-24T19:33:22.024Z Reads: 138

```
Where did you find that heat sink/fan set up?  What is the voltage of your fan?  Are you running it directly from the VESC?  If so, where'd you plug-in?  I'm researching a heat problem now and really like your approach.
```

---
## \#23 Posted by: dogeatgod Posted at: 2016-08-24T20:50:06.363Z Reads: 130

```
eBay - search 5v fan and heat sink.
There's loads out there and really cheap.
Fan is powered from VESC - tapped into power supply to transmitter receiver unit thing.
```

---
