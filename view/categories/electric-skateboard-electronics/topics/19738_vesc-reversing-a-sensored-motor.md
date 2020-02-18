# VESC - Reversing a sensored motor

### Replies: 40 Views: 4292

## \#1 Posted by: mt37 Posted at: 2017-03-26T22:32:22.161Z Reads: 329

```
My motor is turning in reverse and I can't find a way to change the direction in software. (besides using the nunchuck in reverse).

I've tried swapping phases (which works for reversing), but the hall sensor detection always fails now. I think I've tried all the permutation of swapping the hall sensor wires and it always fails.

Any idea how to reverse direction, besides mounting the motor on the opposing wheel ?

It seems like it should be possible in software - if I can do it from the nunchuck.
```

---
## \#2 Posted by: JLabs Posted at: 2017-03-26T22:50:28.373Z Reads: 323

```
Im not really a VESC expert but I'll try to help. 

Put the phase wires in the way you say detection works. Turn off power, unplug vesc from computer. Flip outside phase wires. Turn vesc back on, plug in and connect. Try detection again. 

Again, I'm no VESC expert but it worth a try.

Edit - From VESC Tool: 
Z-Button:
The Z-button is used to change the direction of the motor if reverse is activated. Without reverse, Z has no effect.

_Edit 2: Make sure control mode is disabled. You may have it on, and forgot to change it. (App config, PPM) make sure to write config and then reboot the VESC._
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2017-03-26T22:54:53.207Z Reads: 305

```
[quote="mt37, post:1, topic:19738"]
I've tried swapping phases (which works for reversing), but the hall sensor detection always fails now.
[/quote]

Sadly the sensor inside the motor are possibly badly place, they are probably too far from the stator, or in a small angle, that could lead them to work in one direction but not the other. :worried:

You can open the motor to see if you can move the sensor, but they are most likely to be pot in epoxy. 

I guess to best outcome, is to change the side of the motor, or just run without sensor.
```

---
## \#4 Posted by: mt37 Posted at: 2017-03-26T23:11:00.397Z Reads: 284

```
@JLabs how do you know which one are the outside phase wires ?

There is a black, a blue and a yellow wire.

It will go in reverse with Z activated, but I would like to avoid pressing Z all the time.

I'll try all the suggestion, and eventually switch motor side if nothing works.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-03-26T23:17:04.537Z Reads: 276

```
[quote="mt37, post:4, topic:19738"]
There is a black, a blue and a yellow wire.
[/quote]

The black is the ground... the red is the 5V.... and the 3 other are sensor (they are automatically detect if your using a vesc) you don't have to know witch one is witch. But you can still try to move there position, to see what can happen
```

---
## \#6 Posted by: rpn314 Posted at: 2017-03-27T00:59:15.089Z Reads: 254

```
[quote="mt37, post:4, topic:19738"]
how do you know which one are the outside phase wires ?

There is a black, a blue and a yellow wire.

It will go in reverse with Z activated, but I would like to avoid pressing Z all the time.

I'll try all the suggestion, and eventually switch motor side if nothing works.
[/quote]

You can pretty easily swap the sensor wires (which I imagine is much easier/less likely to break something by opening the motor). Each phase has a corresponding sensor wire. In the image below, the sensor wires plug into the holes on the top left of the board on the left. Going left to right, you can see a 5V, TEMP, H1, H2, H3, GND. That's the sensor's 5V, Temp sensor, corresponding hall sensors, and the ground. The corresponding phase connectors, going from left to right on the bottom of the board on the left are P1, P2, and P3.

<img src="/uploads/db1493/original/3X/6/e/6eb0f672749f24370bb552983b842e3652ae0d15.jpg" width="629" height="500">

So plug in your phase wires so that the sensor detects correctly, then swap 2 phase wires (to swap the spin direction) and swap the same (corresponding) sensor wires. ie. If you swap the wires connected to phase 1 and phase 2, then swap the sensor wires H1 and H2.

Edit: if you're adamant about no hardware changes, you could swap the port configuration (what physical pins on the processor correspond to what function) in the firmware, essentially swapping the sensor wires.
```

---
## \#7 Posted by: mt37 Posted at: 2017-03-27T01:29:27.880Z Reads: 217

```
@JohnnyMeduse I was talking about the phase wires. not the hall sensor wires
```

---
## \#8 Posted by: mt37 Posted at: 2017-03-27T01:46:18.677Z Reads: 215

```
@rpn314 I tried, from my configuration that works

to swap the outer phase cables, and also swap the outer hall sensor cables (that should make sense right ?)

but it failed

anything that could explain that ?

I'll be trying again
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-03-27T01:49:15.856Z Reads: 206

```
Sorry my bad... but still unlike other esc vesc is mde to automatically detect the motor and sensor... also if the problem is inside the motor there only little you can do
```

---
## \#10 Posted by: mt37 Posted at: 2017-03-27T02:03:29.042Z Reads: 212

```
@JohnnyMeduse it's unclear why it would be a physical issue in the motor. 

but so far no luck switching phase and hall sensors.

it seems like it should be a really simple software fix though.
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2017-03-27T02:21:47.932Z Reads: 210

```
Sensor are suppose to be place at certain range (generally glue directly to) of the stator, if the are too far or badly place, they might only work in one way if the magnetic field is strong enough 

<img src="/uploads/db1493/original/3X/a/1/a1acc6988929c5857dfd92161c4696fd76ed5684.JPG" width="375" height="500">
```

---
## \#12 Posted by: mt37 Posted at: 2017-03-27T02:30:07.322Z Reads: 199

```
@JohnnyMeduse why does everyone else seem very intent that changing phase & sensor wire will work ?
```

---
## \#13 Posted by: mt37 Posted at: 2017-03-27T02:33:38.606Z Reads: 196

```
Here is my methodology right now : 

**hall sensor & phase wires**
H: blue green yellow & P: black yellow blue WORKS (reverse)
reboot
H: blue green yellow & P: yellow black blue DOES NOT WORK
reboot
H: yellow green blue & P: yellow black blue DOES NOT WORK
reboot 
H: green blue yellow & P: yellow black blue DOES NOT WORK
reboot
H: blue yellow green & P: yellow black blue DOES NOT WORK

... 

Is there a point trying the other combination of phase wire swapping ?
```

---
## \#14 Posted by: psychotiller Posted at: 2017-03-27T02:42:20.111Z Reads: 187

```
You can switch two phase wires, but then you need to do motor detection again and apply.
```

---
## \#15 Posted by: mt37 Posted at: 2017-03-27T02:44:18.210Z Reads: 185

```
@psychotiller so retry what I just posted above but hit apply every time after I do detect ?
```

---
## \#16 Posted by: psychotiller Posted at: 2017-03-27T02:45:37.683Z Reads: 185

```
Yup! You have to apply and write every change you make or they take no effect.
```

---
## \#17 Posted by: mt37 Posted at: 2017-03-27T03:09:04.086Z Reads: 184

```
@psychotiller I tried your methodology, no improvement : 

H: blue green yellow & P: black yellow blue WORKS (reverse)
reboot (didn’t have to actually write this one, detect worked on the first try)

now swapping phase wires :

reboot detect, apply, write, reboot
H: blue green yellow & P: yellow black blue DOES NOT WORK
reboot detect, apply, write, reboot
H: yellow green blue & P: yellow black blue DOES NOT WORK
reboot detect, apply, write, reboot
H: green blue yellow & P: yellow black blue DOES NOT WORK
reboot detect, apply, write, reboot
H: blue yellow green & P: yellow black blue DOES NOT WORK

Back to the original one, and it works, without detect / apply / write.
H: blue green yellow & P: black yellow blue WORKS (reverse)

Am I missing something ?
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2017-03-27T03:09:15.658Z Reads: 170

```
[quote="mt37, post:12, topic:19738"]
why does everyone else seem very intent that changing phase & sensor wire will work ?
[/quote]

because in 99% of the case that works, motor will reverse is direction and sensor will work. But there always this 1% that won't work.
```

---
## \#19 Posted by: mt37 Posted at: 2017-03-27T07:22:49.319Z Reads: 170

```
That's good to know, weird that I landed on the "magical combination" of H and P first.

After fiddling for the wires for so long I questioned the contacts, but I can always go back to the one that works.

It's tempting to look at the firmware since software is what I'm most comfortable with.
But seems way more dangerous than mirroring my mount.


Edit: 
@JohnnyMeduse @JLabs is it possible that the hall sensor is damaged and will give out on me at some point if it has this weird behavior ?
```

---
## \#20 Posted by: HTownBomber Posted at: 2017-03-27T13:39:18.258Z Reads: 170

```
Hall sensors aren't complicated; if it works to detect spin in one direction, it _should_ work the other. I think maybe you're adding too many variables by monkeying around with the sensor wires in between detection tests.

Maybe a silly question but have you tried changing the phase wires to, say, black yellow blue (or black blue yellow) while leaving the hall sensor wires in the default configuration? When you say "DOES NOT WORK", are you saying that auto detect doesn't detect the motor spin direction, or that the motor doesn't spin? 

If there is a problem with the hall sensor / wire connections within the motor, you ought to be able to find it with a multimeter (spinning the can by hand). I can give you a quick synopsis on how to open that motor up if a wire is loose at the hall sensors.

But before you do that, I think you need to hold one variable constant (in this case the hall sensor wires) and make sure you're testing without incorrect auto-detect presets in order to isolate the failure point. If you already did that above, that I apologize.
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2017-03-27T13:43:25.371Z Reads: 152

```
As I said before they are probably still good but too far from the stator. If they where damage they probably won't ether way
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2017-03-27T13:45:59.867Z Reads: 156

```
[quote="HTownBomber, post:20, topic:19738"]
Hall sensors aren't complicated; if it works to detect spin in one direction, it should work the other.
[/quote]

Not if they are badly place inside the motor, like every sensor they need to be place in a certain rage of the stator... It is not plug and play... and in certain case the factory can F*** the placement since these kind of motor are mostly hand made.
```

---
## \#23 Posted by: Ackmaniac Posted at: 2017-03-27T13:49:01.372Z Reads: 154

```
What is then the perfect position. Can you give an example?
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2017-03-27T13:52:14.786Z Reads: 157

```
The perfect position is most likely to be glue with direct contact on the stator. (Like the picture I post earlier). But It depend on the sensor (they might be diferent sensor that require a certain distance to work at there best)
```

---
## \#25 Posted by: Ackmaniac Posted at: 2017-03-27T13:55:15.673Z Reads: 156

```
Which sensors board is that in the picture?. Did it come with the motor or did you attach it afterwards?
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2017-03-27T14:02:27.540Z Reads: 152

```
It come with the motor.
```

---
## \#27 Posted by: TarzanHBK Posted at: 2017-03-27T14:22:03.076Z Reads: 152

```
http://e0designs.com/documentation/finding-motor-phase-sensor-combinations/

here´s a good article about how to get sensored motors running.
It´s not as easy as going without sensors and maybe you´ll find something new here what you haven´t tested so far ;)
```

---
## \#28 Posted by: HTownBomber Posted at: 2017-03-27T15:21:15.154Z Reads: 141

```
I've pulled apart a couple of the 6374 motors the OP is using and the hall sensors look standard, glued to the stator the way you'd expect. I can snap some pictures later if needed.

I'm not saying that the hall sensor placement/connections aren't potentially the issue but it seems odd that they would sense in one direction but not the other. Just guessing it may be an issue of the BLDC tool (ie auto-detect initializing the hall sensor configuration / spin direction, then maybe he's not properly resetting when he changes phase wires to reverse the spin). Seems like that could be clarified easily if the motor can detect reverse spin when set to ppm w/reverse.
```

---
## \#29 Posted by: mt37 Posted at: 2017-03-27T15:41:45.179Z Reads: 136

```
@HTownBomber What do you mean monkeying around ? Have you read my methodology ?

I've literally tried every combination of phase and hall sensor.
```

---
## \#30 Posted by: HTownBomber Posted at: 2017-03-27T16:09:46.757Z Reads: 140

```
[quote="mt37, post:29, topic:19738, full:true"]
@HTownBomber What do you mean monkeying around ? Have you read my methodology ?

I've literally tried every combination of phase and hall sensor.
[/quote]

Yeah, I read it and tried to make sense of it, but didn't understand what you meant when you said all other combinations don't work. Perhaps you could clarify about what happens when you swap the phase wires from 1/2/3 to 3/2/1 (ie leaving middle phase wire constant, swapping the motor wires connected to the left & right VESC phase wires) after a fresh reset to default settings / no current control? 

My thought was that the sensor detection may be failing after initialization in one configuration and then a change to another if not properly reconfiguring the setup.

To quote myself, [quote]If you already did that above, that I apologize.[/quote]
```

---
## \#31 Posted by: mt37 Posted at: 2017-03-27T17:21:33.821Z Reads: 134

```
@HTownBomber the link seems interesting, I'll try the procedure outlined here.

I've also tried to set in FOC and check "reverse encoder" which reverses everything for a minute (the software reverse I've been looking for!). Except it switches direction after one reboot.
```

---
## \#32 Posted by: mt37 Posted at: 2017-03-28T05:43:56.691Z Reads: 135

```
Ok, I've followed the methodology outlined here [1]

Starting from a combination of hall sensors and phase wires that work. 

I labeled the phase wires coming out of the VESC: U, V, W and the wires going into the motor: A, B, C

So all my combinations, as outlined by 3. are :

UA, VB, WC detection works, rotates reverse
UA, VC, WB, detection fails, rotates forward
UB, VC, WA, detection works, rotates reverse
UC, VB, WA, detection fails, rotates forward
UC, VA, WB, detection works, rotates reverse
UB, VA, WC, detection fails, rotates forward

I've also tried to do what 6. suggests (cyclic shift of all three phases to reverse direction) and it kept the same direction (reverse).

Edit I've also tried swapping some sensor phase wires, the detection actually works but only when the motor rotates reverse during the "start detection" sequence.

[1] http://e0designs.com/documentation/finding-motor-phase-sensor-combinations/
```

---
## \#33 Posted by: laurnts Posted at: 2017-03-28T06:30:10.949Z Reads: 122

```
I didnt seem to have this issue with my sensored motor. I didnt even get to swap the hall sensor around. It should just work by just swaping one of the phase wire and run the motor detection.
```

---
## \#34 Posted by: mt37 Posted at: 2017-03-28T06:31:13.753Z Reads: 128

```
@laurnts thanks for participating in the convo, but please kindly read the above. My testing is rigorous.

Somehow my motor will not detect bldc hall sensor when rotating one of the ways.

Edit. I'm sure it works for some, but not for me. that's the whole point of this conversation, pls comment if you have expert knowledge.
```

---
## \#35 Posted by: laurnts Posted at: 2017-03-28T09:53:52.262Z Reads: 123

```
Ive read the post above. but it didn't make any sense. Phase wire and hall sensor are two different things. They didn't share direct connections. Swapping 2 of the phase wire should be enough to change the directions and the hall sensor should work. Hall sensor contains 6 wires and minimum only requires 5 wires to operate (without the temperature sensor).

1 positive, 1 negative and 3 halls sensing. The hall sensing can be swapped one with another, that shouldn't matter. What is important is not to switch the positive and negative with the halls around.

If in forward / backward direction the hall sensor works, that means that the wiring of the hall sensor works fine. It should also do work for the other way around.

---

Now what I understand is that the motor runs both direction sensorless, that means the motor and esc is fine up to this point.

So what can possibly went wrong is that the ESC sensor area is broken / buggy which I think less of an issue when it can still work for one direction. Hence what I think what is wrong with your setup is one of the hall sensor is faulty.

---

The only way to proof this is to compare / cross check it with another sensored bldc motor.
```

---
## \#36 Posted by: mt37 Posted at: 2017-03-28T17:13:19.734Z Reads: 115

```
I think the sensor is faulty too. Since it only works one way.

@JLabs Any chance for a return of my lemon motor ?

Edit: Also I've found more interesting material on the subject 
Someone in [2] suggests changing the amplification value to the sensor board within the VESC firmware.

[1] http://www.electric-skateboard.builders/t/vesc-motor-detection-failing/6640
[2] http://vedder.se/forums/viewtopic.php?t=637
```

---
## \#37 Posted by: JLabs Posted at: 2017-03-28T18:57:27.927Z Reads: 110

```
I was not aware that it was my motor. I'll converse over PM.

Did you use an adapter or solde to the board? From what I am aware the order of the phase wires does not matter with the VESC. I just suggested flipping them to see if it would help.
```

---
## \#38 Posted by: mt37 Posted at: 2017-03-28T19:18:32.712Z Reads: 110

```
I rewired the original plug into a JST that will plug into the VESC.
```

---
## \#39 Posted by: mt37 Posted at: 2017-03-31T18:29:13.632Z Reads: 103

```
@JLabs was able to confirm with the manufacturer that these motors will run sensored in one direction in BLDC but no problem with both in FOC.
```

---
## \#40 Posted by: JohnnyMeduse Posted at: 2017-03-31T22:10:55.137Z Reads: 100

```
You have to be cautious in FOC, because sensor are manually detect and won't give you a error if they're bad.
```

---
