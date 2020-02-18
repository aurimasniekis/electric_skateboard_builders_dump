# Nyko Kama VESC settings (too sensitive!) Solved

### Replies: 31 Views: 5046

## \#1 Posted by: Ross Posted at: 2016-01-11T08:47:39.782Z Reads: 272

```
Hi Everyone!

I i have 2 VESCs connected via CAN BUS and connected to a Nyko Kama nunchuck. All is working well except the throttle / break response is way too sensitive. When i display the input from the Kamas y axis i can see the range of motion from min to max acceleration which is great, but the motors only respond to a small fraction of that full range.  Looking at the throttle input on the BLDC screen full motor speed occurs at like 20% input but 15% is dead band, so min to max is only about 5 percent, which is about 1mm of thumb movement. When i break it just comes on full instantly with no proportional respect to throttle position. I've had a good look around the settings but can not figure out how to adjust it to make the full throttle range usable. also i have tried using 14 volt input from a supply and with 12S lipo. Throttle response is no different between the  two (with respect to minimum and maximum throttle position that is)

Could anyone help me? Thanks!
```

---
## \#2 Posted by: trbt555 Posted at: 2016-01-11T09:09:10.524Z Reads: 267

```
What are your ERPM limits ?
What is your dead band setting ?
Can you post screenshots of the relevant BLDC tool screens ?
```

---
## \#3 Posted by: Ross Posted at: 2016-01-11T10:05:57.152Z Reads: 256

```
Hi,

Thanks for your reply. I'm not sure how to post a screenshot on this forum? sorry :-/ But the VESCs are from Enertion V4.10 Im using BLDC Tool 2.8 and 2.8 firmware.

Settings under the App configuration > Nunchuck tab

Dead band: 0.15
ERPM limit start: 150000
ERPM limit end: 200000 (but it wont let me adjust higher)

Same settings on both VESCs
```

---
## \#4 Posted by: treenutter Posted at: 2016-01-11T14:58:46.191Z Reads: 234

```
@Ross I have this same issue! The throttle and braking when using the nunchuck isn't smooth or progressive like it when I use GT2B with VESC. The way I've tamed it is by limiting RPM so that I don't end up tripping the voltage cutoff on VESC, but that is a lame solution because the throttle is almost "all or nothing." This is a part of why I started using GT2B.
```

---
## \#5 Posted by: trbt555 Posted at: 2016-01-11T15:04:03.851Z Reads: 232

```
Maybe it's someting to do with your Nyko Kama, is it the same receiver as the one shown in the relevant VESC FAQ thread ?
```

---
## \#6 Posted by: treenutter Posted at: 2016-01-11T15:39:45.884Z Reads: 229

```
@trbt555 I have two transmitters that I've tried, but only one receiver. Same results either way. I'll post my screens.
```

---
## \#7 Posted by: trbt555 Posted at: 2016-01-11T15:45:51.850Z Reads: 225

```
VESC firmware version ?
VESC hardware version ?
```

---
## \#8 Posted by: Ross Posted at: 2016-01-11T16:05:15.264Z Reads: 224

```
@treenutter & @trbt555  Yes its certainly frustrating, especially with 12S! Basically on / off. I don't believe its a problem with the remote or receiver though because they seem to sending and receiving the correct data. In the BLDC tool display the input bar moves smoothly from full reverse to full forward as it should with respect to the joysticks position. Its just that only the very middle couple of mm either side of neutral (on the controller) is actually useful to modulate the throttle / breaks. On the input display bar you can also see that this is only a very small range around neutral that the motors respond to. And yeah, the break just comes on like an anchor, will lock the wheels even at walking pace.
```

---
## \#9 Posted by: Ross Posted at: 2016-01-11T16:08:42.024Z Reads: 221

```
VESCs are V4.10 and firmware is 2.8
```

---
## \#10 Posted by: treenutter Posted at: 2016-01-11T16:30:46.948Z Reads: 222

```
@Ross @trbt555 My VESC is HW version 4.7 and Firmware 2.8. I'm now exclusively using the Linux version of BLDC Tool. BLDC motor control (haven't tested the nunchuck with FOC yet).
```

---
## \#11 Posted by: chaka Posted at: 2016-01-11T17:23:15.316Z Reads: 226

```
You can adjust the throttle ramping in the app config>nunchuk menu. You also need to know that while running in "current" control the motor will spool up to full rpm if not under any load.
```

---
## \#12 Posted by: treenutter Posted at: 2016-01-11T17:33:12.748Z Reads: 227

```
Thanks @chaka. In BLDC 2.8 there are settings for Positive and Negative "ramping time constant" The default settings are  .9 and .3 respectively. How will changing these impact control? Would we increase or decrease them to modify sensitivity? I think it would be to increase ramping time to decrease sensitivity. Do you have a sense of how much they should be edited?
```

---
## \#13 Posted by: chaka Posted at: 2016-01-11T18:17:38.282Z Reads: 224

```
Increasing the time will make it feel "softer"

Vedder addressed this here: [https://youtu.be/G8f0xg7DNmM?t=154][1]


  [1]: https://youtu.be/G8f0xg7DNmM?t=154
```

---
## \#14 Posted by: treenutter Posted at: 2016-01-11T20:14:16.146Z Reads: 217

```
Thanks @chaka I'll try these out and report back. I'll start w 2.0 and 1.0. At some point, someone needs to author a configuration guide for VESC. Maybe it's a good community project for everyone on this forum!
```

---
## \#15 Posted by: sk8ace Posted at: 2016-01-11T21:50:46.256Z Reads: 211

```
I adjusted mine to 10 on the positive ramping and though very smooth, it wasn't quick enough. I was about to try 5 but I shorted out the nunchuck receiver.. lol. Picked up a gt2b and it's way smoother than the nunchuck. It's huge so I will eventually mod it to a smaller case. 

Don't be afraid to set it higher than 2 on the positive. You may have to give it an initial pushoff though but once you are moving, it's great.
```

---
## \#16 Posted by: Ross Posted at: 2016-01-11T23:15:37.664Z Reads: 200

```
Ramping is really only delaying the problem a little. The problem is that it would still be impossible to hold your thumb at say 35% throttle. you would still basically have to modulate on and off which is a horrible way to control anything! What we need is a "full speed (or) current @ "x" % throttle input" setting. So many people seem to be using the Kama, surely there not all using it like this. Might have to get an RC receiver and use PPM? I really like the Kama, and i know its just a number value somewhere causing the problem!
```

---
## \#17 Posted by: chaka Posted at: 2016-01-11T23:21:13.256Z Reads: 194

```
I gotta ask, have you ridden it yet?
```

---
## \#18 Posted by: Ross Posted at: 2016-01-11T23:58:52.112Z Reads: 190

```
A little yes, but its pretty much unridable... Breaks are certainly useless.
```

---
## \#19 Posted by: chaka Posted at: 2016-01-12T00:31:54.027Z Reads: 188

```
Once you dial back your max current and add a bit of throttle ramping you find it easy to ride at a constant speed.

If you switch to an rc controller aka ppm, you can use duty cycle and have total control but it is much more raw and unregulated.
```

---
## \#20 Posted by: lowGuido Posted at: 2016-01-12T01:03:41.071Z Reads: 185

```
do you hold down the C button while riding?
```

---
## \#21 Posted by: Ross Posted at: 2016-01-12T02:26:03.504Z Reads: 181

```
No I have not tried the C button yet, but how would this effect things?
```

---
## \#22 Posted by: psychotiller Posted at: 2016-01-12T03:05:07.363Z Reads: 171

```
The c button rules! But you have to let off of it before you can brake. With it pressed you would just be adjusting cruise control.
```

---
## \#23 Posted by: Ross Posted at: 2016-01-12T03:06:37.683Z Reads: 168

```
If i buy a Wiiceiver can i use the PWM settings instead, Is that how it works?
```

---
## \#24 Posted by: trbt555 Posted at: 2016-01-12T06:23:10.109Z Reads: 169

```
This is weird, I'm also running a nunchuck without problems and I have the default time ramping settings set.
Have you tried re-flashing the firmware and doing a fresh setup of the VESC ?
As you're both using different hw versions I'd be surprised it was the VESC itself.
You could also try a second Nunchuck/receiver combo. They're cheap on amazon and if it diesn't work you could just return it.
```

---
## \#25 Posted by: trbt555 Posted at: 2016-01-12T06:31:19.448Z Reads: 167

```
@Ross If you buy Wiiceiver you connect to the PPM pins just like you would with an ordinary RC rx. You would use the PPM app settings instead of the Nunchuck application.
But it adds another layer of complexity for no real gain.
```

---
## \#26 Posted by: lowGuido Posted at: 2016-01-12T07:22:59.919Z Reads: 172

```
Wiiceiver will not solve your problem.  You need to use the perpetual steez button (C) to engage your steez and then control acceleration with the thumb stick by flicking it up or down for deceleration.
To brake simply release the perpetual steez button and gently bring the thumb stick back.

watch me in this video and pay attention to my thumb.
https://youtu.be/Xe_WowHbwmE?t=1m5s
```

---
## \#27 Posted by: Ross Posted at: 2016-01-12T11:47:56.077Z Reads: 168

```
PROBLEM SOLVED!!! :-D 

I reflashed both VESCs with the SAME firmware as already installed (2.8). I then chose the same CAN, general and nuchuck settings on each VESC the same as before. The only thing i did differently was run the auto motor parameter detection immediately after reflashing. I had not yet run the auto detection when i was having the problems, but parameters were so close that i don't think that this was the issue. But yeah that worked...

Anyway, this thing is ridiculously powerful!!! Soooooo much better than i expected! I just reduced the max amperage to 40 to each motor (from 60 default) so ill see how that goes. There is no way i could have possibly used all the torque before. Breaking was also basically flawless, but no more than half could be applied before locking the wheels. So i have reduced breaking current to -30 amps (from 60 amps default)

By the way I'm running;

Gravit Drop Kick 43" (1/2" drop deck)
Batteries 12S (2 x Turnigy Zippy 6S 4500mah 45C in series)
Caliber standard trucks
3/16 shock pads (nice n low)
2 x VESC 4.1 With heat sinks mounted to each FET
Custom enclosure with active cooling (printed in PLA)
5v 0.5 amp centrifugal cooling fan (50mm in diameter)
2 x Enertion r-spec 190 KV 63-55s
Torqueboards V1 rotatable mounts
Alien Drive Systems Abec 11 hub drives (36t)

Works very nicely together indeed!
```

---
## \#28 Posted by: lowGuido Posted at: 2016-01-12T22:57:41.955Z Reads: 157

```
good to see you got it sorted!
(I still recommend the use of perpetual steez though.) :smiley:
```

---
## \#29 Posted by: treenutter Posted at: 2016-01-13T00:33:55.413Z Reads: 154

```
@Ross do you have a build thread on this forum w pictures? If not, I bet everyone would love to see your build. I'm interested in the custom enclosure in particular.

Above you've noted that you adjusted the motor and brake currents; do you have any advice on how to dial them in? Right now I'm using the default brakes and 70A (based on the max current my motor can handle). My build thread is [here][1]


  [1]: http://www.electric-skateboard.builders/t/the-village-build-s9-faultine-paris-195mm-sk3-6764-diyes-mount-8s-vesc-127mm-pneumatic-wheels/292
```

---
## \#30 Posted by: Ross Posted at: 2016-01-13T01:37:49.926Z Reads: 148

```
Haven't taken her for a run since the adjustments but i will tonight and let you know how i go.
```

---
## \#31 Posted by: Ross Posted at: 2016-01-13T01:42:40.037Z Reads: 146

```
No build tread yet, still got mu ugly test batteries strapped to the top of the deck :-\ But i just had 4 x Nano-tech A-spec 3S 4500mah  65 - 130c arrive :-) They are so slim (19.5mm) going to look awesome! Ill take photos once its finished. How do you upload photos to this forum? i cant figure it out.
```

---
