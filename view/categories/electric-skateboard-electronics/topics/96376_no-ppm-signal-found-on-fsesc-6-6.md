# No PPM signal found on FSESC 6.6?

### Replies: 15 Views: 280

## \#1 Posted by: SeVeSeventyOne Posted at: 2019-06-11T18:10:55.711Z Reads: 64

```

Hi, 

Just received my FSESC 6.6 and connected it to the battery, motor and PC. Updated the software to ESC and used the wizard to spin the motor. Then next to input settings, I use hobby receiver and connected it to the servo port of that ESC, I bind the receiver to TX and set up the VESC Tool for mapping, but I receive nothing. I connected the oscilloscope and see a clean PWM signal from my receiver going to the ESC. What is wrong? Settings are in the pictures.![pic1|548x500](upload://pkOaXyWBypN1MxyWc2pjxTVLrjG.png) ![pic2|548x500](upload://cwtXwDX31zqkuCvUwzosBJmswBc.png) 

I have red few topics of this same issue but nothing has solved this. Even a topic where "something unknown" happened and it started to work suddenly. What excactly I should try to make this to work ?
Is the new board already fried, broken from the factory ?

![IMG_20190611_205242_resized_20190611_085313018|690x345](upload://rQabUFlKqcQuwTuNSlKmerOTaH4.jpeg)
```

---
## \#2 Posted by: sofu Posted at: 2019-06-11T18:38:23.947Z Reads: 54

```
Change your control type under ppm general to current no reverse braking and apply your app settings.
```

---
## \#3 Posted by: SeVeSeventyOne Posted at: 2019-06-11T19:19:37.292Z Reads: 48

```
Hi, I did that now, settings are now like this, updated the app, but no change, no PPM signal when I move the throttle up and down. What is the signal amplitude requirement?, is 3,3V signal level high enough ?

![pic3|548x500](upload://wWq3LiIRtEfUGeKmjV5a76HaPfm.png) 

![IMG_20190611_221312_resized_20190611_101335247|690x345](upload://rKXhdHfgqShKMBJtrYHbMXKNynI.jpeg)
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-06-12T04:00:26.538Z Reads: 38

```
Are you sure your on the right channel? And have you tried flipping the ppm cable on the receiver?
```

---
## \#5 Posted by: SeVeSeventyOne Posted at: 2019-06-12T10:25:13.275Z Reads: 27

```
"right channel" ? You mean right channel on my receiver? The scope picture is taken from the ESC PPM connetor and it responses to my throttle on my TX, so yes I'm sure it is the right channel.
"Flipping the cable"?? other way around?, so GND to signal and vice versa? No I did not do that, why would that help? that would mean that the documentation on FSESC is incorrect, so signal pin is not the pin which is marked on their documents ?
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-06-12T11:49:23.922Z Reads: 25

```
[quote="SeVeSeventyOne, post:5, topic:96376"]
You mean right channel on my receiver?
[/quote]

Yeah have you tried plugging the cable into the other channels yet?
```

---
## \#7 Posted by: SeVeSeventyOne Posted at: 2019-06-12T11:56:14.402Z Reads: 22

```
No I did not see that necessary as my current (throttle) channel produces the PWM signal identical as I expect to get from other channels. But I will try that for curiosity.
I wonder since the FSESC specification is so simplified, what is the threshold voltage of that PPM port on ESC. I have 3V3 signal, assuming it is enough, but is it? I will try to use a receiver which output 5V signal... if I have any.. else I need to build a converter..
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-06-12T12:03:05.633Z Reads: 20

```
Did you turn ppm pulsemapping on?

It seems it's still off on the picture.
```

---
## \#9 Posted by: vladaxon Posted at: 2019-06-12T12:07:04.043Z Reads: 20

```
That's because PWM and PPM are different types of signal. You receiver produces PWM signal, it has outputs for each channel. PPM signal encodes multiple channel in one and than transmits by one signal wire. You need a PWM to PPM converter.
```

---
## \#10 Posted by: SeVeSeventyOne Posted at: 2019-06-12T12:07:31.327Z Reads: 20

```
hmmm..good question.. based on my study, that means the output drive to be off not the mapping, is that correct ? However I tried many combinations and couldn't find that have any nfluence.
```

---
## \#11 Posted by: SeVeSeventyOne Posted at: 2019-06-12T12:13:27.000Z Reads: 20

```
According to Flipsky web page, they had an example how to control their ESCs with Arduino, and they presented simple PWM signal produced by arduino to control FSESC.
https://flipsky.net/blogs/vesc-tool/how-to-control-fsescbase-on-vesc-with-arduino

Just my thought, first,  why would ESC need a PPM signal, they only use one channel for throttle information... and second, their documentation says "servo" signal which is always PWM to directly control servos.
```

---
## \#12 Posted by: vladaxon Posted at: 2019-06-12T12:43:33.928Z Reads: 19

```
In that page they use 5v signal level. So this might be a reason, as you mentioned before.
```

---
## \#13 Posted by: AlanZhou Posted at: 2019-06-12T12:47:42.060Z Reads: 19

```
The esc outputs 5v....
```

---
## \#14 Posted by: SeVeSeventyOne Posted at: 2019-06-12T12:54:59.969Z Reads: 19

```
FSESC outputs 5V yes, but when you feed the receiver with 5V its inner regulation regulates it down to 3V3 or at least lower to get a proper voltage for its receiver circuitry. Therefore it produces 3V3 on its output as well.
I dont have VESC schematics right now, nor I have FSESC schematics, is their input stage somehow altering the input signal, or is their MCU running on 5Volts ? Typically 5V MCU can read 3V3 signals as "HIGH" but perhaps there is some sort of stage that damps the signal...
```

---
## \#15 Posted by: SeVeSeventyOne Posted at: 2019-06-12T19:37:18.812Z Reads: 18

```
Well at least a small progress. I made a converter that converts 3V3 signal to 5V and now ESC reads the pwm signal input. But that's not all...

I used previously the wizard to read the motor parameters and could spin the motor via the wizard, and now I did it again, stored the settings, configured all voltage, current and wattage limits as my system is. Now that input signal is present and set; low = 1ms and high = 2ms motor won't spin. It gives knurling, whining sound but no spinning no matter where the throttle position is, not really pulling any current either. Now what can this be ? If I use the arrow keys to operate the motor, the same thing.

update1:
I help the motor to spin it with my hand and suddenly wheel chopped quite violently, once, twice and then halted... then I tried it again and same repeats.

update2:
Motor wizard has detected my motor to have 46 poles ! How could I verify this,,,
My motor doesn't have any printed info whatsoever. I tried to change it to 14, and it gets wild, cogging and bursting but yea it does something different.. what next ?
```

---
