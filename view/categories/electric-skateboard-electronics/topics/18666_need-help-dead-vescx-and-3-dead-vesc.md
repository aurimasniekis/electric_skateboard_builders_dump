# Need help - dead VescX and 3 dead vesc

### Replies: 21 Views: 2216

## \#1 Posted by: Jebe Posted at: 2017-03-06T23:47:29.678Z Reads: 215

```

I'm having some trouble with a build.
Am running 2 R-Specs and vescs via Can bus with a GT2B on a vanguard.
 All connections were hotglued in place. 
Was performing brilliantly, top speed 43km ( more left but thats fast enough for me ) great accelleration and range.
I had about 300km's on it when I started having one motor brake while riding. This was only happening intermittantly and I was far from home. I noticed my GT2B was nearly flat so I put it down to this.
Got home and charged the board and the remote.
Next day we set off again( My fiance on the evolve GT because my DIY was kicking it's ass ).
Got around 1km away and had the braking issue again.
I thought this was a mechanical issue and tightened a belt as it was a lot looser than the other one.
Not long after this the board stopped altogether.
On the master Vesc, it looks like C44 has blown. 
Once back at home I tried to connect the BLDC tool but neither vesc would power up. Interestingly the GT2B reciever does power up. No lights on the vesc .
I found this on the forum 
http://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600
and tested as per the instructions. 
Is this an accurate test? Does not look like a short across C25.
It looks like the original problem is inside the motor with cables rubbing on the metal frame.

Pulled the motors apart and found a bad solder connection on one winding.
Resoldered and heat shrink applied. Check with meter. All seemed OK.

Connected up with spare vesc’s, one vesc and one vesc-x. I used the vesc-x as the slave. Ran the BLDC motor detect on both then connected the drive gear back up. Hot glue to finish

This time I used very conservative vesc settings. 20amps each battery and 50 amps motor. Motor regen -40 and battery regen -12
Took it for a ride and everything seemed fine, carving hard to try and recreate the issue with the motor braking. No problems there.
Unfortunately after about 2km, while under braking from around 20km/hr the board went dead again.
Master vesc shows no leds but powers up the receiver, Vesc-X has died as well. C44 looks OK this time. Bad burny smell lingering, :rage: 
Neither vesc will connect to BLDC tool.
4 dead vesc’s in a week – seem to be linked to Canbus, and under braking, but I don't really know.
One of these vescs was used in a single motor build for around 500km no problems.
Any ideas anyone?
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2017-03-06T23:56:38.121Z Reads: 194

```
could be a cold solder joint some place...i was getting that on one board....everything looked good....till i really dug around,,,the positive wire to the post was all jacked up and causing an intermittent disconnection till it stopped working
```

---
## \#3 Posted by: Jebe Posted at: 2017-03-06T23:58:31.946Z Reads: 191

```
On a vesc? This has happened on 2 sets of dual vescs. Was that the main positive connection?
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2017-03-07T00:04:37.458Z Reads: 181

```
it was,,,but it could be cold soldered at any soldered spot...just shooting out suggesting as to find the reason....that was my issue....yours could be different....i like going from simple to difficult
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2017-03-07T00:05:56.304Z Reads: 172

```
and the other reason could be a shorted motor.....
```

---
## \#6 Posted by: Jebe Posted at: 2017-03-07T00:06:28.128Z Reads: 171

```
appreciate that bud. Cheers
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2017-03-07T00:07:05.449Z Reads: 166

```
its like seeing one of our soldiers down lol
```

---
## \#8 Posted by: Jebe Posted at: 2017-03-08T00:52:38.884Z Reads: 147

```
@onloop waiting over a week for a response from your website bud. Can you shed any light on this?
```

---
## \#9 Posted by: Blasto Posted at: 2017-03-08T01:17:27.335Z Reads: 141

```
For shitz and giggles, how was your CAN bus connected? Did you solder wires on the CAN bus connector?
```

---
## \#10 Posted by: Jebe Posted at: 2017-03-08T02:20:12.547Z Reads: 135

```
Hi blasto. No I didn't solder them, I hot glued them in place.
```

---
## \#11 Posted by: Jebe Posted at: 2017-03-08T02:21:43.293Z Reads: 137

```
<img src="/uploads/db1493/original/3X/f/4/f4d5f0bcd1d9febe340cc90a12ec83db2e747415.jpg" width="690" height="388">
My dead vescs :( 
The one to the right of the vescx died from the firmware bug. The rest as described above.
```

---
## \#12 Posted by: Blasto Posted at: 2017-03-08T02:30:39.977Z Reads: 136

```
Not sure i understand, you hot glued just the wires to the pins or you used a connector? 

Were those bullets completly isolated from each other?
```

---
## \#13 Posted by: Pantologist Posted at: 2017-03-08T02:35:56.590Z Reads: 133

```
The Vesc X died from a software issue? Care to explain?
```

---
## \#14 Posted by: Blasto Posted at: 2017-03-08T02:36:37.233Z Reads: 134

```
[quote="Pantologist, post:13, topic:18666, full:true"]
The Vesc X died from a software issue? Care to explain?
[/quote]

Think that was a typo... the vesc to the right
```

---
## \#15 Posted by: Jebe Posted at: 2017-03-08T02:50:37.673Z Reads: 134

```
I used a connector - bought it from ollinboards with 2 of his motors. I used hotglue to hold these in place.
The motor bullets are well insulated - I use a cable gland entry like this.
<img src="/uploads/db1493/original/3X/f/3/f35813848f2e92261167fad74f9db63629365158.jpg" width="690" height="419">
It keeps pressure on the connectors and keeps them well away from each other.
I use heat shrink on the connectors then push them into this. 
No the vesc to the right of the vesc x did.
It had the issue described here[http://www.electric-skateboard.builders/t/vesc-faq-firmware-bug-pre-august-2016-please-upgrade/8018](http://www.electric-skateboard.builders/t/vesc-faq-firmware-bug-pre-august-2016-please-upgrade/8018)
Vesc-X was being used as a slave unit on canbus.
Was braking slowly from about 20km/hr when the board just went dead :'( 
Under braking as I'm sure the first one did. Hard to say as I had a bad connection on a motor - I thought this must have somehow fried the first lot - open phase - circulating currents with no where to go under braking? 

With the second pair, I had resoldered all the motor connections, silicon wire to phase wire and did not experience the braking/cogging issue I had before yet symptons look the same. powers the reciever but no lights on the vesc, no connection to BLDC tool and that nasty tell tale smell of magic smoke being released.
```

---
## \#16 Posted by: Michaelinvegas Posted at: 2017-03-08T06:06:43.654Z Reads: 126

```
@Jebe  thats terrible luck man... totally feel for you...so frustrating
```

---
## \#17 Posted by: Eboosted Posted at: 2017-03-08T06:42:15.855Z Reads: 128

```
Thanks crazy man!, I don't understand how could this happen with those conservative VESC settings.

Have you checked the current ramp value?

I had issues when writting VESC settings more than once reseting to default values, when it happened I clicked on write and the inmediately clicked on disconnect/reboot too fast, even before VESC was able to write/save the information.

Batt min (regen) was -20 (-40 for dual) instead of -10 (-20 for dual), all PPM settings, motor max and min were default as well.

So, I'd suggest to read the settings before unplugging the USB from both VESCs just verify.

The other thing you could do it buy a bluetooth modu;e and datalog at least your first complete ride.

BTW I use -10A bat min (regen) for each VESC not -12A as you
```

---
## \#18 Posted by: makevoid Posted at: 2017-03-08T08:01:39.129Z Reads: 120

```
I had a problem with RSpec phase wires not well insulated and that caused a vesc to fail. I suggest to check the wires that go into the motor, if they're properly insulated and to shrinkwrap them if they are not
```

---
## \#19 Posted by: Jebe Posted at: 2017-03-08T08:34:51.290Z Reads: 116

```
I found the same thing, blamed that for the first pair failing, removed resoldered and re-insulated all phase wires.
:confused:
Still don't understand how it could take BOTH vesc's out.
 I dont want to use these motors again. Have 2 ollinboard 200kv motors.

Just need that wider caliber hanger @torqueboards 
Thanks for all the input guys.
```

---
## \#20 Posted by: Jebe Posted at: 2017-03-08T08:36:06.064Z Reads: 116

```
Current ramp is 0.04 - not increasing like that dodgy firmware revision caused.
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2017-03-08T13:50:53.239Z Reads: 112

```
[quote="Jebe, post:19, topic:18666"]
I found the same thing, blamed that for the first pair failing, removed resoldered and re-insulated all phase wires.
[/quote]

If you had a short at first. The possibilities for overheating the motor (if you had try to run it with the short still on) and create second short over the winding is there... I'm pretty sure you have a dead motor and like a zombie will continue to eat the brain of each new vesc you put on it, so you might want to change it before trying another vesc.
```

---
