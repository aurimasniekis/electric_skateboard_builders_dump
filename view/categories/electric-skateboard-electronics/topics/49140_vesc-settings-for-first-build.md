# Vesc Settings for first build

### Replies: 24 Views: 792

## \#1 Posted by: ArsenalMain Posted at: 2018-03-15T00:29:17.321Z Reads: 140

```
Hello esk8 community,
I am on the final push before completing my first board. I have soldered and connected everything and all that remains in setting up my vesc. 

To give some context, my board is made up of a 190kv diy motor, the diy torque vesc and 5x 2s 60c batteries in series. I'm also using a best tech bms. I was reading around and watching videos and wanted to get your guy's opinion on if this would be a viable settings for a non-foc vesc.

![Screenshot (2)|690x387](upload://tBtRvECOQ2MNZa5RExhPGafkL8B.png)

Thanks in advance.
```

---
## \#2 Posted by: ShutterShock Posted at: 2018-03-15T00:45:53.385Z Reads: 129

```
Those look pretty good.  You can feel free to increase the motor max break down to -80 if you feel you need more breaking power.  

I assume you have a 60A capable BMS?
```

---
## \#3 Posted by: ArsenalMain Posted at: 2018-03-15T01:00:18.062Z Reads: 123

```
Ya this is the one I ordered ![Screenshot_2018-03-14-17-58-45|250x500](upload://e0HhrKidte0Z5OerMtgcSmqgBg7.png)

Is there anything else I should consider or change? Any settings?
```

---
## \#4 Posted by: ShutterShock Posted at: 2018-03-15T03:29:45.516Z Reads: 107

```
Awesome, that means you probably have upgrade room for later.  Just make sure you set your voltage cutoff and everything correctly, and perform motor detection.
```

---
## \#5 Posted by: ArsenalMain Posted at: 2018-03-16T01:40:20.891Z Reads: 89

```
Do you know where I can update my firmware?
```

---
## \#6 Posted by: ShutterShock Posted at: 2018-03-16T04:02:27.061Z Reads: 86

```
It should be available on the firmware tab in the VESC tool.  Be sure you select the correct hardware version corresponding to your VESC
```

---
## \#7 Posted by: TeslaAlex Posted at: 2018-03-19T20:18:59.748Z Reads: 78

```
Since im in exactly the same situation, i´ll jump on this topic instead of creating a new one! :slight_smile:  I have currently connected my battery and the BMS and only the VESC-configuration is left. I have read for quite some time but I can´t seem to find a build with the same specs as mine, so im not totally sure on the settings yet. 

Specs:
**12s 8000mAh 240A Lipo** (4x3s 8000mAh 30A)
**Bestech 12s 80A BMS** 
**SK3 6374 168KV** 

What motor max/min and battery max/min should I get?
Would 44V be a good battery cutoff start and 42V (3,5V per cell) a good battery cutoff end? 

Thanks! :slight_smile: 

/Alex
```

---
## \#8 Posted by: RedEagle Posted at: 2018-03-19T20:49:13.557Z Reads: 72

```
Motor min -70a (strength of the brakes)
Motor max +70a (70a is what this motor can handle, I would set this to 40 first and test to see how it handles, then gradually increase the value, same goes for motor min)
Batt min 16a (8a * 2 = 16a, recommended charge rate of your batteries, mostly 2c, this can be higher)
Batt max 30a (not sure, this also depends on the discharge capability, can be a lot higher)

Can you post your battery specs?

There was someone who described the functions of these settings beautifully. Can't remember who it was though. Maybe someone else knows?
```

---
## \#9 Posted by: TeslaAlex Posted at: 2018-03-19T20:53:24.999Z Reads: 65

```
The battery is made out of 4* 3s 8000mAh 30C Lipo batteries. This should give it a discharge rating of about 240A (30C * 8A = 240A).
```

---
## \#10 Posted by: RedEagle Posted at: 2018-03-19T20:54:20.883Z Reads: 61

```
Do you have a link with specs?
```

---
## \#11 Posted by: TeslaAlex Posted at: 2018-03-19T20:55:27.753Z Reads: 60

```
There you go :slight_smile:  [Link](https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack-xt90.html)
```

---
## \#12 Posted by: RedEagle Posted at: 2018-03-19T20:57:21.530Z Reads: 60

```
What vesc are you using? 4.xx? 6?
```

---
## \#13 Posted by: TeslaAlex Posted at: 2018-03-19T20:58:14.680Z Reads: 58

```
Im using a FOCBOX, latest version.
```

---
## \#14 Posted by: RedEagle Posted at: 2018-03-19T21:02:37.931Z Reads: 57

```
They didn't specify a max charge rate for your batteries, so:
batt min 8a
batt max 30/40maybe even 50a (test this and see when it delivers adequate power e.g. if 30a is too weak and 40a performs fine then set it to 40a)
absolute max 240a
```

---
## \#15 Posted by: TeslaAlex Posted at: 2018-03-19T21:04:35.435Z Reads: 53

```
Nice, thanks a lot! What do you think about the voltage cutoff settings? Would 3,5V per cell (42V) be a good battery cutoff?
```

---
## \#16 Posted by: RedEagle Posted at: 2018-03-19T21:10:31.316Z Reads: 53

```
You draw current when you move, so at the time you're riding the system is under load. So let's say you set the cutoff at 3.5v. When you stop the voltage bounces back up to around 3.6v. 
You will never overdischarge you lipo's this way. I'd say MAX 3.4v but people have gone as far as 3.3v.
Best to play it safe and set it to 3.5v. Feel free to experiment. Don't blow up your house though. :joy:
Hope this helps.
```

---
## \#17 Posted by: TeslaAlex Posted at: 2018-03-19T21:12:50.886Z Reads: 53

```
Okay, nice to get some good information. :slight_smile: I´ll try these settings out and see how the board behaves.

Thanks for helping me out!  :grinning:
```

---
## \#18 Posted by: RedEagle Posted at: 2018-03-19T21:16:14.367Z Reads: 53

```
One more thing:

Motor min - Braking at low speed
Motor max - Power at low speed
Batt min - Regenerative braking
Batt max - Power at high speed

Settings simplified in a nutshell.
```

---
## \#19 Posted by: TeslaAlex Posted at: 2018-04-04T07:11:28.413Z Reads: 50

```
I got out and tested the board yesterday. Compared to my earlier 6s build, this thing is great! It flies up hills! 

My current vesc settings are:

Motor max: 50A
Motor min: -50A
Battery max: 40A
Battery min: -16A
Absolute max: 130A

These work great, although I would like to have a bit more low speed torque. Could I increase motor max/min up to 70A and battery max to 50A? :grinning: What problems could I encounter?
```

---
## \#20 Posted by: RedEagle Posted at: 2018-04-04T12:39:09.242Z Reads: 41

```
You can increase motor max/min to whatever your motor can handle. Say your motor can handle 100 amps. In this case you can set motor max/min to 100a & - 100a. Same goes for batteries. I would do this in steps to see which setting is right. 
That vesc is known to be quite fragile (not so fragile as maytech) so be careful. Maytech vescs for example can only handle 30a batt max & 27a continuous. I don't know what tb vescs can handle. You can have voltage spikes and overheating issues to name a few.
```

---
## \#21 Posted by: mmaner Posted at: 2018-04-04T14:42:19.612Z Reads: 37

```
I'm not having a dig at you, I honestly want to know if you have you ever owned a TB VESC?  Or if you are just repeating what you've heard, because it's not true.  

I have multiple boards using them with FOC and 60a plus constant.  I've only ever had 1 fail, and it was my fault and @torqueboards still replaced it.   I've never seen an overheating issue on a TB VESC and voltage spikes would be a battery/BMS issue...not the VESC.
```

---
## \#22 Posted by: RedEagle Posted at: 2018-04-04T14:49:08.111Z Reads: 38

```
I'm repeating what I've heard and I've never owned TB's. I do own maytechs however and I can't say anything bad about them. Guess you just have to have some luck.
```

---
## \#23 Posted by: Bjork3n Posted at: 2018-04-04T15:01:02.049Z Reads: 34

```
My tb vesc lasted one testride... not saying they are crap but the quality seems very inconsistent.
```

---
## \#24 Posted by: mmaner Posted at: 2018-04-04T15:07:28.441Z Reads: 34

```
I'm not saying you did anything wrong...but every failure I have personally seen has been due to user error.  Hitting the ERPM limit while on the bench, crappy soldering, shorting phase wires, etc.
```

---
