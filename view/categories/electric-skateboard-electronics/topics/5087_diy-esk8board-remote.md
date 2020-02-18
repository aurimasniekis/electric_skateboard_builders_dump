# DIY esk8board remote

### Replies: 20 Views: 5686

## \#1 Posted by: JTAG Posted at: 2016-06-24T13:05:40.038Z Reads: 449

```
OK Guys who else likes the design of these remotes?:
<img src="/uploads/db1493/original/2X/7/78e38850ecbc9bb796a79ea2cb636c01425300b7.png" width="690" height="342">
<img src="/uploads/db1493/original/2X/0/046837fc86ecec02565dc6ded161c59577711bf1.gif" width="360" height="240">

I like the boosted board remote because of its ergonomics + button (rubber soft touch) and like the stary remote for the screen / menu. For a while now I think the VESC / opensource / DIY lovers (me included ) lack a "fancy" finished product style remote. 

The things I rally miss om the "regular" remotes are:

* Seeing the state of charge of the battery.
* Being able to turn down the torque to let other people do their first ride on my board.
* See the speed
* Being ably to charge simply (it now has 2 AA batteries)
* (be waterproof)

What do you guys like to see?
```

---
## \#2 Posted by: lox897 Posted at: 2016-06-24T13:17:13.478Z Reads: 430

```
We are really missing out on the modes for beginners. Cruise control maybe? Cruise control is only on two of the available remotes to us DIYers.
```

---
## \#3 Posted by: flatsp0t Posted at: 2016-06-24T13:20:25.086Z Reads: 424

```
CC would be nice, but the most needed/missing is the "low power / speed" button.
Fiddling with a laptop and the vesc settings every time a beginner wants to ride is really pain in the ass
```

---
## \#4 Posted by: Kaly Posted at: 2016-06-24T13:28:10.483Z Reads: 417

```
Here is a good starting point for this remote project 

http://vedder.se/forums/viewtopic.php?f=14&t=19&sid=10f406f6f267f1f10f5f6cc2fbe79d24
```

---
## \#5 Posted by: Maxid Posted at: 2016-06-24T13:35:06.788Z Reads: 399

```
+1 for cruise control
and it would be nice if this would all be possible even with other ESCs than the VESC.
```

---
## \#6 Posted by: RunPlayBack Posted at: 2016-06-24T13:57:23.472Z Reads: 391

```
I agree. This is why I keep an EGO and Boosted in my collection, for beginners to learn on and to avoid having to reprogram all the time.
```

---
## \#7 Posted by: harpie Posted at: 2016-06-24T14:22:15.982Z Reads: 376

```
I bought myself one of those winning (jason is currently using one) remotes. It has an rfm chip and a microcontroller. I am hoping its a pic or an atmel. In that case I am planning on writing new firmware with an oled screen mod. Would be cool to implement all of these features. It should be easy getting the battery data back to the remote. Some options could be built in to tune the pwm range or profile for beginner mode.
```

---
## \#8 Posted by: treenutter Posted at: 2016-06-24T14:25:21.351Z Reads: 365

```
This sounds great @JTAG. The number one feature should be 100% reliability with zero dropouts. Everything else is nice to have, but a luxury compared to reliability. The number of people that have SYF'd because of a controller\signal dropout is way too high.

[In another thread about remotes](http://www.electric-skateboard.builders/t/good-radio-transmitter-hand-controller-for-use-with-diy-electric-skateboard/928/19), @chaka commented that a hybrid remote would be ideal; FHSS for throttle, AFH for everything else. I completely agree. I would prefer to avoid BT as the transmission protocol for throttle.

[quote="chaka, post:21, topic:928"]
Me too, we should build a hybrid. FHSS for throttle and braking, AFH for telemetry and auxiliary features.
[/quote]
```

---
## \#9 Posted by: mason Posted at: 2016-06-24T16:06:17.227Z Reads: 334

```
Trigger should have gt2b reliability. The telemetry data should be on Bluetooth or similar, because it isn't nearly as bad if you get telemetry drop outs
```

---
## \#10 Posted by: Dutch Posted at: 2016-06-24T17:04:31.815Z Reads: 334

```
For now i'm sticking with a nunchuck as remote for my build. But when my parts arrive i'm going to build one of these.
One with a little display on it. The case is pretty much the same and will be made on the CNC soonish.
Going with a black or antraciet aluminum brushed look. Mainly because the plastic ones are to light in my opinion, need some weight in my hand.
```

---
## \#11 Posted by: JTAG Posted at: 2016-06-24T17:59:04.436Z Reads: 313

```
Glad to see that others also like to see a beginners mode option / desire on the remote!

Currently the new VESC design seen to carry the NRF24 chip for control. I looked at the VESC code and it seemed easy enough do be adapted and support the features we desire. So for the remote I am also looking into the NRF24 chipset. 

I don't really see the benefit for a dual radio solution, it doubles the cost and any type of radio you choose nowadays is already full-duplex. Since the upstream data is not that important it can be a very low data speed such that it wont bother the important desired torque setpoint that goes down.
```

---
## \#12 Posted by: treenutter Posted at: 2016-06-24T18:35:46.032Z Reads: 306

```
@JTAG the benefit would be signal strength (that it never drops because of distance from receiver) and signal integrity (that it never drops because of interference from other signals in the air).

This is definitely not my area of expertise, so if there is a solution that assures zero dropouts, that's excellent, please bring it to the masses!

However, reading here and ES it seems like BT signals are far less reliable, and FHSS never drop. Personally, I'd pay double for a controller that never drops. Given the choice between a single SYF incident, and higher cost, I'd say to take my money.
```

---
## \#13 Posted by: hexakopter Posted at: 2016-06-24T19:19:22.179Z Reads: 292

```
Maybe you should read this here: [http://www.electric-skateboard.builders/t/vesc-nunchuk-rf/588/82?u=hexakopter](http://www.electric-skateboard.builders/t/vesc-nunchuk-rf/588/82?u=hexakopter)
Just because you mentioned the NRF24L01 chips. And I think vedders implementation should have prevent that, but because I still feel the pain I know that it wasn't in my case. Still don't know why.
```

---
## \#14 Posted by: JTAG Posted at: 2016-06-24T19:35:23.363Z Reads: 290

```
Thanks for the pointer. Yes we will need to track that issue down and fix it. Hope your pain will go away fast.
```

---
## \#15 Posted by: Kaly Posted at: 2016-06-24T20:32:12.765Z Reads: 306

```
I really like the project of a device like this in the DIY community but For now and until this remote is a reality it will be good to think about a DPDT switch for the following reasons. 

1- ability to switch battery configuration 6S -12S ( beginner to advance)   

2- 6S charging capability ( less money in charger and power supply ) 

3- emergency cutoff switch at your finger tips. 

And all this with a device that cost $ 5.99 at the Home Depot.

I put this switch on all my builds. 

 <img src="/uploads/db1493/original/2X/4/488814fd2c297d4e6d99aa7a50fde244f14937e5.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/1/190fee21af852872b27fb325335aaa394510a93a.jpeg" width="375" height="500">
```

---
## \#16 Posted by: Mobutusan Posted at: 2016-06-24T22:51:33.013Z Reads: 277

```
@JTAG How about a trip counter/odometer? And maybe capability to add temp sensors for ESC/motor and monitor on remote?
```

---
## \#17 Posted by: JTAG Posted at: 2016-06-24T22:53:22.488Z Reads: 271

```
Nice idea! You need some matching with wheel diameter / poles / gearing ratio but nothing really high tech.
```

---
## \#18 Posted by: Mobutusan Posted at: 2016-06-24T23:13:00.562Z Reads: 280

```
@JTAG Also, I don't know if it's feasible, and wouldn't necessarily need to be incorporated into the remote, but how hard would it be to add in capability to monitor and datalog current draw, voltage, watts, max/min values? Maybe as a standalone module or something? I'm planning on using a watt meter and a gopro (yi) camera to video log my setups, so I can figure out where problem areas/configurations might be, and also see if I can determine if one setup operates more efficiently than another.
```

---
## \#19 Posted by: Nordle Posted at: 2016-06-24T23:23:47.811Z Reads: 270

```
I would take a look into [''RollingGecko''] (http://rollinggecko.github.io/ArduBoardControler/) this.
For sure a good point to start from.
```

---
## \#20 Posted by: tardyparty7 Posted at: 2018-10-29T05:26:55.971Z Reads: 77

```
bro, if ur still working on this, u could check out SolidGeeks diy remote.
```

---
