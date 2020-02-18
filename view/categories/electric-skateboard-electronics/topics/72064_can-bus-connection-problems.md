# CAN bus connection problems

### Replies: 20 Views: 575

## \#1 Posted by: Acklavidian Posted at: 2018-10-23T13:22:23.022Z Reads: 121

```
I'm having problems getting the CAN bus to work properly on my dual focbox setup. Originally, I had it working but at some point my slave unit would become unresponsive after a few minutes of riding. After some maintenance I found that it would cut out immediately during foc motor detection on the first step. I did some investigating and found that my CAN bus connector had almost been severed near one of the plugs. So I ordered a new CAN bus cable. In the mean time I decided that I would  use a PPM splitter that I had laying around until the CAN cam in the mail. I used the wizard to set both of my focbox units as a single unit. I also updated the firmware on both units to the latest. This worked well. However, now that I have my new CAN bus connector cable I can't get the units to communicate over the CAN connection. I've used the wizard to set the Master and slave unit via usb. But, the units won't communicate regardless. I can't even connect the configuration tool with CAN forwarding. Every time it reads "no firmware response received..." I've checked the setting set by the wizard a million times. Mainly the ID and CAN forwarding enabled options. What am I missing here?
```

---
## \#2 Posted by: Sender Posted at: 2018-10-23T13:24:42.754Z Reads: 115

```
Could have burned the can chip on the pcb
```

---
## \#3 Posted by: Acklavidian Posted at: 2018-10-23T13:26:57.214Z Reads: 111

```
How could I check this?
```

---
## \#4 Posted by: taz Posted at: 2018-10-23T13:27:59.606Z Reads: 109

```
Have you set a different id to the master and slave vesc?
```

---
## \#5 Posted by: Acklavidian Posted at: 2018-10-23T13:29:36.559Z Reads: 104

```
Yeah. I pretty much let the wizard do its thing on both. But setting the master as id: 0 and the slave as id: 1 is part of it.
```

---
## \#6 Posted by: Blasto Posted at: 2018-10-23T13:56:23.763Z Reads: 91

```
Untick “send status over can” on the master
```

---
## \#7 Posted by: Acklavidian Posted at: 2018-10-23T17:59:32.000Z Reads: 80

```
Thanks. I'll try this as soon as I get home. Did something change recently with the "send status over can" option?
```

---
## \#8 Posted by: Blasto Posted at: 2018-10-23T18:01:40.435Z Reads: 73

```
Should only be the slave esc that has that option ticked
```

---
## \#9 Posted by: dareno Posted at: 2018-10-23T20:42:11.203Z Reads: 69

```
Reckon its a program issue to be sure.  If you'd done the canbus chip they would both be dead as a dodo.  No lights nothing.  If by some strange reason the can bus is shot then you can remove the chips and they work again with split ppm.
```

---
## \#10 Posted by: Acklavidian Posted at: 2018-10-23T23:55:48.821Z Reads: 61

```
no luck. "send status over can" was set true on the master. I flipped it and still no connection.
```

---
## \#11 Posted by: Acklavidian Posted at: 2018-10-24T00:00:31.879Z Reads: 60

```
I took some screen shots of my settings to get the diagnostic juices flowing:
<h1>Master</h1>

![master|690x436](upload://8GFCDpmgRVfu4rU3MskJtsto1cl.png) 

![master_ppm|690x441](upload://nkwvKb6m7WnSYAAP1Jx0iuhvsm9.png) 
<h1> Slave </h1>

![slave|690x430](upload://212dnt9xLt3glqXBpjybXXQb3lk.png) 
![slave_ppm|690x443](upload://2y8YHAwwfnN2wtiiAkgXa4C44PD.png)
```

---
## \#12 Posted by: Acklavidian Posted at: 2018-10-24T00:01:56.211Z Reads: 56

```
![connection_attempt|690x441](upload://ryM1Wk0QbI6rsRo46R0KaNlMKqx.png)
```

---
## \#13 Posted by: Acklavidian Posted at: 2018-10-24T00:03:41.741Z Reads: 59

```
well both work perfect as of now on ppm splitter. So are you saying that would mean that the canbus chip isn't fried because they wouldn't boot up?
```

---
## \#14 Posted by: dareno Posted at: 2018-10-24T00:07:27.401Z Reads: 59

```
absolutely.  If you fry the canbus then the boxes will not work at all so a programming issue it will be.
```

---
## \#15 Posted by: Acklavidian Posted at: 2018-10-24T00:28:13.776Z Reads: 54

```
I can't help feeling like it's something to do with the version 3.40 firmware upgrade. Is anyone running dual vescs on 3.40 firmware?
```

---
## \#16 Posted by: Acklavidian Posted at: 2018-10-25T18:19:55.753Z Reads: 47

```
Did the down grade but still won't connect. Any ideas?
```

---
## \#17 Posted by: margrave Posted at: 2018-11-25T19:52:12.490Z Reads: 41

```
Veeeery similar issue here:

- Both motors work perfectly
- Both VESC controllers work and are updated to the same latest firmware
- Remote and receiver work fine and I'm able to control each motor individually, wither with the remote or with the VESC tool
- When connected via CAN bus, only the motor connected to the receiver works
- When enabling the "CAN bus forwarding" option on the side panel in the VESC tool, the software disconnects (also gives a "cannot read firmware version" error)
- Both motors are connected with the same colour order (yellow blue black), but one of them runs in reverse with the same motor and app configuration. I've used the VESC tool to reverse the motor on the app settings, but I don't know if I should change the cable order instead (does it have an impact on CAN bus data?)
```

---
## \#18 Posted by: ArnhemAnt Posted at: 2018-11-25T21:04:31.295Z Reads: 39

```
[quote="margrave, post:17, topic:72064"]
* Both motors are connected with the same colour order (yellow blue black), but one of them runs in reverse with the same motor and app configuration. I’ve used the VESC tool to reverse the motor on the app settings, but I don’t know if I should change the cable order instead (does it have an impact on CAN bus data?)
[/quote]

What you have explained with the motor directions is pretty normal. Mine have done the same thing. Dual motor setup, running dual ESCapes over CanBus. I just reversed the direction of the motor with the ESC tool and it's all working fine. No real need to swap motor cables around.
```

---
## \#19 Posted by: ArnhemAnt Posted at: 2018-11-25T21:07:36.290Z Reads: 39

```
[quote="Acklavidian, post:16, topic:72064, full:true"]
Did the down grade but still won’t connect. Any ideas?
[/quote]

The image you have posted showing the error message when trying to set up Can forward shows that you have the forwarding set up from 1. Have you tried to set this up from 0 instead?
I had similar problems with mine when I was setting them up and kept getting the error message, then I swapped the ID numbers and it worked perfectly. Hope this helps you out.
```

---
## \#20 Posted by: margrave Posted at: 2018-11-25T21:27:44.470Z Reads: 34

```
Thanks! Also I'll check the send data option, right off the bat not sure how did I have it setup (I know it is in reply to a different user but good think to check anyways)
```

---
