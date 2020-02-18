# Dual VESC over CAN - One belt break, the other motor looses power, Why?

### Replies: 20 Views: 261

## \#1 Posted by: Pedrodemio Posted at: 2019-03-23T22:43:28.474Z Reads: 103

```
The title says all

I can't understand why is this the default behavior, it totally kills one of the main points of dual motor, redundancy

@trampa

Maybe @Deodand also has some insight 

Long history, after doing some stupid donuts on the dirt in the middle of nowhere, the belt gets shredded, ok my fault , even more for not bringing my phone or any tools, but it still doesn't change that the current behavior is bad

Is this the same problem that cause one of the motors to spin slower when they are unloaded? Thought a lot about in my 6 km walk of shame home
```

---
## \#2 Posted by: taz Posted at: 2019-03-24T06:56:51.073Z Reads: 92

```
Did you have traction control enabled?
```

---
## \#3 Posted by: rich Posted at: 2019-03-24T07:45:18.153Z Reads: 85

```
I had many walk of shames. 

Meanwhile I carry every tool and spare part I could need in my backpack.

Was ist the master or slave motor where the belt snapped?
```

---
## \#4 Posted by: trampa Posted at: 2019-03-24T07:49:34.473Z Reads: 85

```
That's why you want a BLE dongle and the VESC-Tool app. Maybe your walk of shame could be an inspiration for a new feature, allowing to control the slave via master, but have the master motor switched off.
```

---
## \#5 Posted by: taz Posted at: 2019-03-24T08:53:11.562Z Reads: 76

```
[quote="trampa, post:4, topic:88073"]
allowing to control the slave via master, but have the master motor switched off.
[/quote]

Can't we already do that by setting 0 amps for everything on the master and disabling traction control?
```

---
## \#6 Posted by: Andy87 Posted at: 2019-03-24T09:28:52.543Z Reads: 69

```
Maybe the software can just detect the load loss and do that by there own? 🤔 probably the better way, instead of depending on a second device which could have a connection loss or empty battery or what ever...

Edit:
[quote="Pedrodemio, post:1, topic:88073"]
more for not bringing my phone
[/quote]
@trampa that’s what I mean. Even the new tool and the BLE dongle wouldn’t have helped him in this case.
```

---
## \#7 Posted by: trampa Posted at: 2019-03-24T09:45:20.025Z Reads: 64

```
That's why you prepare for the ride. Phone, spare inner tube, maybe spare belt, some tools.
We design our boards to require a minimum of tools. 
@taz Yes, you can set master to zero amps and only drive slave. That could also be a single button for convenience.
```

---
## \#8 Posted by: Andy87 Posted at: 2019-03-24T09:52:14.116Z Reads: 61

```
I see we look from different sides on it and that’s ok. Just there million other ways why a phone could stop to work. I think you know best by your own that it doesn’t matter how good you prepare, you most likely will need the things you don’t have with you. That’s why, if a sw can do that why to relay on a second tool.
```

---
## \#9 Posted by: banjaxxed Posted at: 2019-03-24T09:52:25.166Z Reads: 61

```
would be nice to be able to instruct a slave to become the master, maybe difficult with canbus
```

---
## \#10 Posted by: Battosaii Posted at: 2019-03-24T12:22:33.155Z Reads: 52

```
You would need 2 receivers for that to work because the master Vesc is the one that should be plugged into the remote receiver. Unless you can open your enclosure
```

---
## \#11 Posted by: banjaxxed Posted at: 2019-03-24T12:27:17.369Z Reads: 52

```
Mmm yes of course 🤭

maybe possible to have the receiver wired to both ESCs for that scenario, if of course the firmware allowed for the slave to ignore signal until the slave detects no can comms then slave becomes master

Firmware and 3pin cable mod, could be my simplification of a complicated process tho

I use can and not split receiver so gotta say this is of interest personally
```

---
## \#12 Posted by: Andy87 Posted at: 2019-03-24T12:27:18.740Z Reads: 49

```
I don’t see a problem the master request the ppm signal from the slave ppm port via can.
It’s just not implemented in the sw. If it works in one direction, why it shouldn’t in the other?
```

---
## \#13 Posted by: banjaxxed Posted at: 2019-03-24T12:31:41.112Z Reads: 52

```
Drawbacks?

Maybe the can cable becomes detached from either ESC, maybe the can chip goes poof on either ESC.

In that case you are now running split receiver(with one dead esc), congratulations you get home on the slave’s back praising Skatan all the way
```

---
## \#14 Posted by: banjaxxed Posted at: 2019-03-24T12:34:45.299Z Reads: 47

```
My understanding is canbus is bidirectional

@Ackmaniac 
@Deodand 
@trampa  

What say the F/W peops?
```

---
## \#15 Posted by: Andy87 Posted at: 2019-03-24T12:37:34.230Z Reads: 45

```
Sure everything is possible and can fail.
Your ppm receiver antenna can break as well or the plug can get lose. 
As far as I know the latest versions of the CAN connection are pretty stable against any damage.
```

---
## \#16 Posted by: banjaxxed Posted at: 2019-03-24T12:41:11.412Z Reads: 45

```
Is the receiver is damaged game over typically, nothing to be done there in f/w

Even the dual single pcbs like the unity rely on can, so if the master side dies, you should be able to limp home
```

---
## \#17 Posted by: taz Posted at: 2019-03-24T14:24:44.903Z Reads: 40

```
I think the only way to be able to ride home, regardless of what was damaged (apart from a damaged remote), is to use 2 receivers and no can connection.
```

---
## \#18 Posted by: trampa Posted at: 2019-03-24T16:17:10.443Z Reads: 36

```
Something can always brake, that's the nature of technology. If you take a 4X4 car off road, you prepare yourself. Spare tire, tools, winch, spare fuses, 10L extra fuel, oil, maybe satellite phone. 
Before you start your adventure the car gets a proper service and checks. 

I never had a VESC 6 fail on me, chance of burning it mid way seams to be very very little. Worst case scenario: Open the lid, plug receiver to slave, re-configure via App. 5V usb jack for phone should be easy to install on any board. 
Two receivers can be used, even when using can. You can plug it in, but deactivate ppm or NRF. When you need it, switch it back on. 
Carry a spare 50 $ android Phone if you are totally paranoid of getting stranded.
```

---
## \#19 Posted by: banjaxxed Posted at: 2019-03-24T16:33:10.145Z Reads: 33

```
It would be nice to have the option not to open it up, some environments are hostile to open electronics.

Just a sugg. on a possible enhancement requiring only software and 3cm of receiver cable
```

---
## \#20 Posted by: Pedrodemio Posted at: 2019-03-24T16:47:39.934Z Reads: 31

```
Thanks for all the input guys

Yeah, traction control would have saved, but never had a need for it so it was off, first thing I did after creating this topic is to turn it on

@trampa my main question is why this is the behavior happening, lets say I'm commanding X amps, why if one motor isn't able to get to the desired current, the other one doesn't even try

In my head with traction control off, they should be completely independent, I'm not even talking about the slave turning master or something like that, I would had no problem with the beltless motor spinning at full rpm if that would mean that I had power on the other one

Maybe is something you could bring it to Benjamin

 @rich I feel you, I stopped carrying anything in shorter rides due to the board being pretty reliable

It's the master that snapped, I think if it was the slave I would be fine
```

---
