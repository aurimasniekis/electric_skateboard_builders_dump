# Sensor short by water&hellip; Thought?

### Replies: 24 Views: 374

## \#1 Posted by: onepunchboard Posted at: 2018-07-31T16:40:52.670Z Reads: 120

```
So, I just went past the water puddle. 
my board is watertight, like pressure watertight. except motors.
my torq motor used with water before, but this time I connected sensor cuz I have it why not use it right?

now it shorted and took my focbox with it. Prob DRV death. (there goes my lunch money FML)

I'm going back to sensorless. trying to mess up with startup boost, I usually do 0.04 but thinking increase to 0.05 or 6 for better stand start

what u gys think?

Any input is appriciated.
```

---
## \#2 Posted by: briman05 Posted at: 2018-07-31T16:44:45.221Z Reads: 117

```
To me I would think that it would short at the plug on the focbox.  I would not think that the sensor would short in the motor
```

---
## \#3 Posted by: b264 Posted at: 2018-07-31T16:46:41.713Z Reads: 114

```
I had this happen 3 times.  The solution is to take the motor apart and put silicone conformal coating on the sensors and all the electrical connections inside the motor.
```

---
## \#4 Posted by: onepunchboard Posted at: 2018-07-31T16:47:56.634Z Reads: 109

```
I was thinking maybe there was some not-coated area on sensor on motor. @b264 thought the something but I guess no going back at this point I prob killed the sensor already. I trusted too much of this company to do right QC. (No offense, shits happen. it's the factory that makes this after all)
```

---
## \#5 Posted by: briman05 Posted at: 2018-07-31T16:49:25.379Z Reads: 102

```
yeah possibly but you could take the motor apart and coat everything like @b264 suggested and see if it comes back
```

---
## \#6 Posted by: onepunchboard Posted at: 2018-07-31T16:50:33.712Z Reads: 100

```
TBH I don't know if the sensor is still shorted or not. I don't want to risk another drv tho.
unless u know how to check it...
```

---
## \#7 Posted by: briman05 Posted at: 2018-07-31T16:56:23.887Z Reads: 94

```
I have seen shorts caused by bridges created between solder joints in your case I would think this bridge would be water.  Does the motor still work?
```

---
## \#8 Posted by: onepunchboard Posted at: 2018-07-31T17:00:15.011Z Reads: 89

```
I haven't check it. focbox is dead so can't confirm rn but I will take apart the motor. I will take a look the solder on the sensors
Tnx
```

---
## \#9 Posted by: b264 Posted at: 2018-07-31T17:40:18.719Z Reads: 77

```
I think if you apply ground and 5V to the sensor board you should see the lines going near 0V and near 5V as you turn the rotor
```

---
## \#10 Posted by: onepunchboard Posted at: 2018-07-31T18:07:20.316Z Reads: 76

```
So I check line btw 5v and ground and turn motor with multimeter?
```

---
## \#11 Posted by: b264 Posted at: 2018-07-31T18:12:48.286Z Reads: 72

```
Turn the rotor with your hand
```

---
## \#12 Posted by: onepunchboard Posted at: 2018-07-31T18:24:37.516Z Reads: 68

```
srry i ment turn motor with hands, and use multi meter to detect voltage.
turn with multimeter sounds really stupid haha XD
```

---
## \#13 Posted by: b264 Posted at: 2018-07-31T18:32:43.366Z Reads: 75

```
There should be 5 or 6 wires

Ground, Power, A,B, C

or

Ground, Power, A, B, C, Temp

You'll have to figure out what they are.  Red is generally a color used for +5V and black is generally a color used for ground but you'll have to trace them back to the ESC and see which is which

Ground and Power need 5V or 3.3V and then A, B, and C should alternate between true and false (on and off / high and low / 0V and 5V) as you turn the rotor
```

---
## \#14 Posted by: onepunchboard Posted at: 2018-07-31T19:09:34.823Z Reads: 69

```
I opened my board. Sensor is fine but focbox blew L damn....
@JohnnyMeduse do u think u can fix it or toss... ![20180731_150855|281x500](upload://iDNk0qIQ2dg7N6DAN2arRsvpzPo.jpg)
```

---
## \#15 Posted by: Battosaii Posted at: 2018-07-31T19:15:05.213Z Reads: 68

```
Hmm you blew a direct fet, you can try to repair it but it depends how bad the PCB is damaged. Worst case they say it can't be repaired and it gets tossed anyway so why not try.
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2018-07-31T19:45:43.122Z Reads: 65

```
Sorry the PCB is completely damage, there is not really a safe way to repair it.
```

---
## \#17 Posted by: Brdchris Posted at: 2018-07-31T20:26:03.560Z Reads: 65

```
Just curious, would it be worth it/ do you recommend saving this board to use as spare parts for his next fox box?
```

---
## \#18 Posted by: onepunchboard Posted at: 2018-07-31T20:39:28.102Z Reads: 64

```
Well I don't plan to buy focbox anymore as there are more option now including the new unity. I'm just ganna wait for next Gen vesc. At 12s, power isn't an issue...

But yeah if anyone wanna buy this focbox I'll sell it really cheap
```

---
## \#19 Posted by: Brdchris Posted at: 2018-07-31T20:47:27.919Z Reads: 62

```
I guess I was mostly interested in if it would be worthwhile in general. I do industrial automation and have rebuilt a few drives in place do to lack of spares etc. also I’ve read there is a direct fet shortage.
```

---
## \#20 Posted by: deucesdown Posted at: 2018-07-31T21:02:36.458Z Reads: 60

```
Oscope so cool for this

![IMG_20171029_221924|666x500](upload://tQShYRLNu3OaS4ICLRzfKEkir5y.jpg)

But so far hall sensors have given me lots of pain and not that much gain. No mas for me.

EDIT btw i never got bldc mode sensor detection to work on that motor. Tried every permutation of phase wires too. Grr!!!
```

---
## \#21 Posted by: onepunchboard Posted at: 2018-07-31T21:09:04.466Z Reads: 59

```
Yeah my build became overly complicated over powered and expensive. I need to draw a line here for this board I think. Just single foc. It's a cruiser board anyways. I don't know why I thought 45mph was a good idea lol.
All I wanted was just a comfort ride home to work initially.
```

---
## \#22 Posted by: briman05 Posted at: 2018-08-01T02:09:37.283Z Reads: 49

```
Did you use bldc tool or esc tool by ack?
```

---
## \#23 Posted by: deucesdown Posted at: 2018-08-01T02:18:07.071Z Reads: 48

```
ack's bldc tool. But my main issues are not with detection, but failures on the road, being stranded, blowing vesc, that sort of stuff. Most of the issues are with making strong yet small splices to those delicate wires, and how delicate the PH connector is. I think I have a handle on how to deal with it, but again, not worth all the risk and trouble. I think I've learned a hip shake that gets me past the startup shudders :slight_smile:

The temperature sensor on hub/DD motors, I think they might get me back to playing with the sensors again.
```

---
## \#24 Posted by: briman05 Posted at: 2018-08-01T12:46:30.561Z Reads: 36

```
I would make sure you have slack in the wires as not having slack can cause them to fail because they get yanked on when turning
```

---
