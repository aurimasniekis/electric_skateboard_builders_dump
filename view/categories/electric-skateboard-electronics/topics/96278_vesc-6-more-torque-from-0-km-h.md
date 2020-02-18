# Vesc 6, more torque from 0 km/h?

### Replies: 33 Views: 1071

## \#1 Posted by: Silverline Posted at: 2019-06-10T10:27:18.132Z Reads: 228

```
This is not an esk8 build, but i´m using the Trampa Vesc 6 plus, and have question about this, so hope it´s okay...

The thing is, I have build an Electric Drift Trike, around the trampa vesc 6 plus and a e-bike hub wheel....

**I know this is a Direct Drive, so no transmission, like i use to have on my esk8, giving a lot of torque.**

I run the vesc 6 at 12s lipo, Motor Max at 100amp and Battery Max 100 amp, and newest vesc tool.

**Any settings that could give me more torque/current from 0km/h ??**
I run the vesc in ADC mode, and the setting "current" in the GUI.... is "duty cycle" better ?
When i hit around 10 km/h I got a lot of torque, and very good acceleration. But most of the time, im going slowly and only need the torque/ amp in the bottom, I don't care about the top end.

And oh.... This is how the beast looks, if any interested :slight_smile:
![1|666x500](upload://fZZTSL8mkNMulzaOzOxRqjfreJv.jpeg) ![2|666x500](upload://suju2lZnBvsGJreFegObvm16rdJ.jpeg) ![3|690x388](upload://cgkTJH6Huqp7tNLOLMGN5qj1r6Z.jpeg) ![4|690x387](upload://zcJyZYBGCZTYc9LwUlAKXaoFbnb.jpeg)  


https://www.youtube.com/watch?v=mHIihDoWY0U


Thanks Guys....
```

---
## \#2 Posted by: linsus Posted at: 2019-06-10T11:33:26.201Z Reads: 199

```
what a beast, do you run sensored? Might help with startup torque
```

---
## \#3 Posted by: Silverline Posted at: 2019-06-10T11:34:22.295Z Reads: 195

```
Oh i forgot...
Yes FOC sensored.....
```

---
## \#4 Posted by: linsus Posted at: 2019-06-10T11:35:42.774Z Reads: 191

```
You can play around abit with the throttle curve, change to duty cycle controlled, to see if it tickles you in a better way. Think you pointed out most of the other things I have to say so thats about all ideas I have
```

---
## \#5 Posted by: Silverline Posted at: 2019-06-10T11:36:48.854Z Reads: 181

```
Thanks...

Whats the big difference between current and duty cycle ?
I will look at the throttle curve... This is just at default now....
```

---
## \#6 Posted by: linsus Posted at: 2019-06-10T11:43:02.053Z Reads: 180

```
Current control means targeting a specific max draw. Duty cycle simply put, describes at which rate the controller is running(or rather switching) the motor, 100% beeing absolut max. (which is close to impossible to reach). 

See simplified gif of dutycycle. (its best explained with a PWM)

![](https://upload.wikimedia.org/wikipedia/commons/0/02/PWM_duty_cycle_with_label.gif)

rather then targeting a current level, it tries to apply throttle relative to desired operational duty of the VESC. Its abit hard to explain. Best if you change mode and see for yourself how it behaves.
```

---
## \#7 Posted by: Silverline Posted at: 2019-06-10T11:44:35.882Z Reads: 171

```
I will give some attention to the throttle curve, and give duty cycle a try. Thanks,,,.
```

---
## \#8 Posted by: Drom Posted at: 2019-06-10T14:31:24.170Z Reads: 145

```
Looks cool! I was worried that this motor won't withstand 5000W with such a low KV even if it's big. Does it get hot?
```

---
## \#9 Posted by: Silverline Posted at: 2019-06-10T15:36:35.661Z Reads: 134

```
Not at all, so much potentiale in this motor.  The vesc is the limiting factor. A HV vesc would just be perfect.
```

---
## \#10 Posted by: Drom Posted at: 2019-06-10T15:58:26.718Z Reads: 126

```
May be [FSESC 200A](https://flipsky.net/collections/electronic-products/products/high-current-fsesc-200a-60v-base-on-vesc6) considering that it's cheaper than Trampa. Or no more chinese ESC after experience with MakerX?
```

---
## \#11 Posted by: linsus Posted at: 2019-06-10T16:16:02.390Z Reads: 124

```
well, the HV vesc wouldn't be the limiting factor if u swapped atleast XD
And you could use it for other stuff as well if its too much. Like a hydrofoil or something :stuck_out_tongue:
```

---
## \#12 Posted by: Silverline Posted at: 2019-06-10T17:10:49.110Z Reads: 118

```
@Drom Still only 12s... Higher voltage is the way to go with this motor.

@linsus Yes exactly
```

---
## \#13 Posted by: Andy87 Posted at: 2019-06-10T19:59:35.886Z Reads: 106

```
One thing you can try as well is to set the positive ramping from 0.3 to 0.1sec. It’s in the ppm settings.
```

---
## \#14 Posted by: Resonant Posted at: 2019-06-10T20:08:27.804Z Reads: 103

```
Which hub motor is that? looks fun, may build something ridiculous like that after my MTB
```

---
## \#15 Posted by: Silverline Posted at: 2019-06-10T20:13:04.470Z Reads: 104

```
Oh yes.... forgot about that setting, thanks @Andy87 but i´m using a hand throttle, and the ADC setting in vesc tool....I have a look if this is possible.

@Resonant its a 1500 watt e-bike hub wheel motor from leafbike motors with efficiency of 90,7%  https://www.leafbike.com/products/e-bike-hub-motor/gearless-20-24-26-700c-28-29-inch/20-inch-48v-1500w-front-hub-motor-wheel-1077.html

Just did a test run of the acceleration and top speed. Now i will play with throttle curve, and ramping time..

Imaging what higher voltage could do :heart_eyes:
https://www.youtube.com/watch?v=Jha0naPZP9A&amp;feature=youtu.be
```

---
## \#16 Posted by: adammunich Posted at: 2019-06-11T08:26:48.258Z Reads: 82

```
Wait I don't understand why you'd suspect more voltage is needed for increased stall torque. Motor torque is a function of field strength, which depends on current, not voltage.
```

---
## \#17 Posted by: Silverline Posted at: 2019-06-11T08:42:49.728Z Reads: 82

```
I know.... At the moment my motor max/bat max is 100amp, with higher voltage i could get away with lower Amp and gain more efficiency, or keep 100amp and get more torque
```

---
## \#18 Posted by: Darkie02 Posted at: 2019-06-11T09:33:14.063Z Reads: 79

```
Do you have any way of showing what ampage you are drawing from the battry and voltage sag? I’m guessing that the limiting factor is the battry. Lipo company’s have a habit of  drastically overestimating what thay can output in the real world.
```

---
## \#19 Posted by: Silverline Posted at: 2019-06-11T09:35:54.012Z Reads: 77

```
Yes... I will log with metr module.
```

---
## \#20 Posted by: Drom Posted at: 2019-06-11T11:10:39.572Z Reads: 79

```
As far as I know, more Voltage gives you more max RPM/speed. Because if your motor is 10KV and wheel is 20", with 50V it will give you max 500RPM / 48kph, and with 70V it will be 700RPM / 67kph.
To keep the same max speed and increase the torque, you need lower KV or smaller wheel size, or higher gear ratio (not applicable in this case)

I could be wrong :grin:
```

---
## \#21 Posted by: Silverline Posted at: 2019-06-11T14:44:04.504Z Reads: 69

```
What do you think is the most fun. 12s @ 100amp  (around 4400watt) or 20s @ 100 amps (around 7320 watt) :-P ?? 
But other than that, you are right :-)
```

---
## \#22 Posted by: FranciscoV Posted at: 2019-06-11T14:54:37.729Z Reads: 66

```
@Tello1969
```

---
## \#23 Posted by: Drom Posted at: 2019-06-11T16:26:15.822Z Reads: 61

```
Definitely more power is better, but if you want more torque you should reconfigure your equipment (motor with lower KV or smaller wheel size). Otherwise, you increase max speed but torque will remain the same. Again, if my calculations is correct. I'm not sure cuz I'm new to this. I hope someone will correct me if so.

Anyway, the main thing right now to make sure that your power when accelerating is really 4440W
```

---
## \#24 Posted by: adammunich Posted at: 2019-06-11T17:32:56.804Z Reads: 60

```
@Drom is right. You will not expect more torque with more voltage. You need to force more current through your motor.
```

---
## \#25 Posted by: Drom Posted at: 2019-06-11T17:54:02.870Z Reads: 59

```
The reason why I'm not sure is that VESC is positioned as a controller with a constant voltage and throttle changes the frequency (technology that distinguishes it from the usual ESC, besides programmability), but I haven't learned much about it.
And if so, then the power during acceleration from 0 km/h directly depends on the voltage, but it seems strange to me
```

---
## \#26 Posted by: adammunich Posted at: 2019-06-11T17:59:13.778Z Reads: 58

```
@drom The VESC uses https://www.google.com/search?q=space+vector+modulation. Think of it like a buck converter. If your motor has a 0.1 ohm coil, then at most you can put 100A through it, at only 10V.
```

---
## \#27 Posted by: Silverline Posted at: 2019-06-11T18:24:25.173Z Reads: 50

```
Thanks guys... I know i'm on the edge with 100amp right now(If i want my vesc to last) Thats why i follow threads like this, wich will most likely allso be able to handle more current (and voltage = speed) https://forum./t/some-new-focers-84v-vesc-6-based-controllers/1513/106
```

---
## \#28 Posted by: Drom Posted at: 2019-06-11T21:03:35.763Z Reads: 44

```
I still don't figure out if it's possible to apply 50 Volts to the motor immediately from 0 RPM or voltage increases with increasing RPM only :thinking:
```

---
## \#29 Posted by: Drom Posted at: 2019-06-11T21:47:33.107Z Reads: 42

```
You can do a very demonstrative test, it looks like you have two 6S li-po batteries in series (right?)
If you set VESC to 6S with same current (100A), unplug one of battery, and if you'll get same torque from 0kpm and max speed 24kpm then i was right :grin:
```

---
## \#30 Posted by: Darkie02 Posted at: 2019-06-12T00:39:47.196Z Reads: 36

```
[quote="Drom, post:28, topic:96278, full:true"]
I still don’t figure out if it’s possible to apply 50 Volts to the motor immediately from 0 RPM or voltage increases with increasing RPM only
[/quote]

A VESC is a switch that’s clever that turns on and off very fast in different ways a switch dose not care what’s after it it still sends the volts thro it

Voltage is how hard and fast the power is pushed through a circuit.

If you turn the kettle on it uses the full amps and voltage but takes time to heat up (ignoring the added resistance heat creates) vesc volts, amps and rpm Works in the same way

Taking them basic things if a 10v circuit was switched on 1/2 the time and off the other 1/2 the average is 5v but there was 10v when it was switched on 

Volts do not make speed on there own it’s like saying a shoelace walks down a road also needs a animal to move it a trainer to lace it through and a partner to work in harmony with 

Hopefully this helps with your and have some ideas on what you might need to research to get a better understanding on electricity and it’s effects and how different things interact and relate with it.
```

---
## \#31 Posted by: Drom Posted at: 2019-06-12T06:14:05.507Z Reads: 24

```
Few years ago I needed a device with stepper motor (12V) and programmable parameters for shooting timelapse.
Some guy made it for me using Anduino, display and buttons.
So I could set the RPM of the stepping motor, pulse interval in milliseconds, and the pulse length in milliseconds. At the time when the motor didn't turn, it was still under voltage, so that the motor could resist the load and pull my camera.

Theoretically, current and voltage should remain constant, but when I set up short intervals / pulses (for example, 20ms/10ms) in practice, this led to the motor having much less torque than at 100ms/50ms, as if power was 5 times less :thinking: I know it's different motors types and principle of operation, but that's what confuses me.

So VESC with a 12S battery immediately go with 50V, but does it mean, that the torque from 0kpm will be 2 times higher than with a 6S battery?

Btw, sorry for my English, i'm still learning :slightly_smiling_face:
```

---
## \#32 Posted by: Drom Posted at: 2019-06-12T07:13:01.014Z Reads: 24

```
Finally, the complete response :grinning:
https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559/7421
https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559/7422
```

---
## \#33 Posted by: Darkie02 Posted at: 2019-06-12T08:39:44.427Z Reads: 21

```
[quote="Drom, post:31, topic:96278"]
fTheoretically, current and voltage should remain constant, but when I set up short intervals / pulses (for example, 20ms/10ms) in practice, this led to the motor having much less torque than at 100ms/50ms, as if power was 5 times less :thinking: I know it’s different motors types and principle of operation, but that’s what confuses me.
[/quote]

Stepper Monterey are designed to have loads of tork to start moving with the trade off of been bad at continued movement (why thay miss steps and there’s no feed back to tell the controller thay have) the issue sounds as tho it’s bade coding or the controller was unable to micro control the step intervals to me.
```

---
