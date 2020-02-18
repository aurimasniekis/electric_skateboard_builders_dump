# Hall Sensors - Troubleshooting the jitters

### Replies: 18 Views: 1789

## \#1 Posted by: dogeatgod Posted at: 2017-03-30T16:30:52.458Z Reads: 189

```
Motor cogging and a bit jittery when starting from standstill. 
Running BLDC Hybrid and no problem with detection.
I can start from a standstill but motor grumbles/cogs and it can be a little jittery when accelerating (Have tried different throttle techniques)

136kw motor, 10S, Urban Carver, 7" wheels - plenty of torque.

This is the first time using a sensored motor - I expected a bit of fine tuning but can't get the smooth take off desired. Kicking off works, but had planned to use freebord bindings, so ultimately not a solution.

Tried adjusting start up boost (0.01 - 0.1 in 0.01 increments) - made difference and 0.09/0.1 setting works best but problem remains.

Tried adjusting Max Current Ramp - no notable difference.

Drawing about 40A when pulling off - motor max is set much higher

What is puzzling is that by disconnecting hall sensors and running sensorless the performance is much improved.

Not sure how detection works but could the sensors be in the wrong position? If so can adjustment be made electronically.

Nothing is over heating and no faults are reported.

Thanks in advance for any advice
```

---
## \#2 Posted by: peter Posted at: 2017-03-30T20:46:54.917Z Reads: 169

```
Motor wires should match with sensor wires.
Try swapping motor wires until you find a combination which runs smooth.
```

---
## \#3 Posted by: dogeatgod Posted at: 2017-03-30T21:12:12.738Z Reads: 162

```
Thank you for advice.

6 permutations so won't take long - will try tomorrow 🤞
```

---
## \#4 Posted by: mt37 Posted at: 2017-03-30T21:15:02.667Z Reads: 160

```
Super interesting topic to me as well. I hope you write a procedure to find the optimal combination while on the test bench.
```

---
## \#5 Posted by: Duffman Posted at: 2017-03-31T05:11:02.617Z Reads: 157

```
Which motors do you use and more important which exact type of hall sensor?

I tried several types of hall sensors and the especially by Chinese manufacturers commonly used 'Honeywell SS411A' were the worst I tried. The reason is, that they have no hysteresis like other types and don't get only triggered by the motors magnets but also get influenced by the pwm'ed coil magnetic field. This leads to jitter and whine at low speeds or stand still.

If you block the motor by hand, give a little bit of throttle and rotate the motor slowly, it should 'click' from magnet position to magnet position without oscillation, whining or jittering.
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2017-03-31T06:22:50.851Z Reads: 151

```
[quote="Duffman, post:5, topic:20011"]
that they have no hysteresis like other types
[/quote]

Pretty much this, if they are using the honeywell ones you mentioned. I personally use US1881-hall sensors which have a hysteresis for it's output logic states (https://www.digikey.fi/product-detail/en/melexis-technologies-nv/US1881LUA-AAA-000-BU/US1881LUA-AAA-000-BU-ND/431868)

<img src="/uploads/db1493/original/3X/0/e/0e9cf57296802fba97aae2081c5e4f9d7b81f0ba.jpg" width="690" height="459">

And even with the hysteresis I still sometimes got faulty states, because the hall-sensor wires were running parallel to the motor wires and that caused induced currents by the PWM spikes.

Try separating the hall sensor and motor wire bundles, if you haven't already.
```

---
## \#7 Posted by: dogeatgod Posted at: 2017-03-31T06:31:41.239Z Reads: 143

```
Trampa motor - PCB sensors - don't know part/model number and at this stage prefer not to open motor as new. 
I'll try your idea after work - what is purpose of this? To hear a click?
Thank you
```

---
## \#8 Posted by: dogeatgod Posted at: 2017-03-31T06:41:32.453Z Reads: 144

```
Thank you.
I'd prefer not to open a new motor at the moment.

I expect the sensors are quality as bought from Trampa.

@trampa - Frank, have you any thoughts to help troubleshoot?

Thanks again for comments and help with this
```

---
## \#9 Posted by: trampa Posted at: 2017-03-31T07:59:34.364Z Reads: 136

```
Hi dogeatgod, we don't face these issues. I run my motor sensored all the time. What Version VESC and manufacturer, BLDC-Tool? Have you tried FOC-Mode? Does the motor turn smooth on sensor detection? Motor max should be around 40A, not higher if you like your VESC 4 to survive. 

Frank
```

---
## \#10 Posted by: dogeatgod Posted at: 2017-03-31T08:25:35.070Z Reads: 136

```
Thank you for speedy reply.
4.10 VESC from Enertion fw 2.18 (BLDC tool and FW downloaded a few days ago from esk8.de)
I've not tried FOC as was worried about frying DRV, as many have, but reading up  it looks more like an issue of going between BLDC and FOC without clearing and reconfiguring settings correctly.
Motor turns smoothly on sensor detection.
I'll lower motor max from 60 to 45 - pulling off currently (excuse the pun) draws 36.
```

---
## \#11 Posted by: trampa Posted at: 2017-03-31T08:38:52.185Z Reads: 132

```
If the motor runs smooth on sensor detection, sensors work just fine. Try out FOC with 40 A max, works seamless on all our VESCs (4.7-4.12). You can increase the startup Amp flow a bit. To low and your motor cant start up well.
Our Motors are low KV and using 40A max there is no DRV issue. People fry there VESCs because the Motor KV is to high and the Amp setting is to high. Please also lock down your motor cables next to the motor housing  to prevent them from bending and wires braking. This can also create issues. Tape or Zip tie with some additional shrink tube on the motor leads. You have the advantage of the long front motor shield, make use of it. Also ad mesh metal on the back if you can!

http://www.trampaboards.com/118-kv-2400w-dc-brushless-out-runner-motor-6364-foc--bdlc--60-p-12966.html
Click on manuals, (below the mage) and download the PDF.

Frank
```

---
## \#12 Posted by: dogeatgod Posted at: 2017-03-31T08:45:27.669Z Reads: 117

```
Thank you for advice.
I'll do a little more reading before trying FOC - will give it a go once comfortable precautions are in place.
```

---
## \#13 Posted by: dogeatgod Posted at: 2017-03-31T18:33:08.701Z Reads: 111

```
Tried all combinations, ran detection and reconfigured each time. There was one combination that appeared to run a little smoother with motor in reverse but nothing to write home about. Gave it a go though : )
```

---
## \#14 Posted by: dogeatgod Posted at: 2017-03-31T19:08:21.243Z Reads: 112

```
Just been out running unsensored, so, so, so much fun :grinning:

No cogging, very quiet, plenty of go : )

<img src="/uploads/db1493/original/3X/5/c/5c713835384d241f9ee346b51e03d1c2019cc68d.jpg" width="666" height="500">

Rain stopped play.

No stress on motor cables but will follow your advice once final decision made regarding layout. I'll probably make a mount for batteries behind/above electronics enclosure - similar style case. Gaffer tape, table cloth clips and an old battery box work a treat whilst testing though.

I'm going to stick with sensorless until having a spare VESC in the tool box, probably in the next week or so. Then will swap and try sensored again, if no joy will then go FOC.

Thank you all for the help - will keep you posted
```

---
## \#15 Posted by: RogerD Posted at: 2017-04-01T09:54:35.484Z Reads: 99

```
I'd stay unsensored mate. The VESC's key USP is smooth unsensored motor control.
```

---
## \#16 Posted by: dogeatgod Posted at: 2017-04-01T17:25:52.037Z Reads: 97

```
I think you are right. 

I'll try sensored again with the other VESC; if no difference will quit whilst ahead in an effort to break current VESC cycle.

V ery 
E xcited
S topped Working
C ash

(Repeat)
```

---
## \#17 Posted by: Smorto Posted at: 2017-04-02T00:16:01.430Z Reads: 94

```
[quote="dogeatgod, post:16, topic:20011"]
V ery E xcitedS topped WorkingC ash
[/quote]

Lol love this
```

---
## \#18 Posted by: Landshark Posted at: 2017-05-29T03:53:00.944Z Reads: 75

```
Any solution here?  I'm running BLDC with hybrid sensors and I get the same cogging/jittering at startup also braking at slow speeds locks the wheels up.  Braking at faster speeds is fine though...
```

---
