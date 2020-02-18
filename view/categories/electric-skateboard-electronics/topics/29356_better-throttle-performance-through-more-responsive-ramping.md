# Better throttle performance through more responsive ramping

### Replies: 31 Views: 2298

## \#1 Posted by: Jinra Posted at: 2017-08-02T00:44:06.336Z Reads: 225

```
I've been playing around with some of the vescs other settings to get more "oomph" in my torque and acceleration and I've found an often overlooked setting that will virtually double your acceleration AND deceleration response (keyword *response*).

**The Problem:**
With all the vescs I've used, I've noticed my full-throttle-from-stand-still (let's call this dragster performance) was lacking compared to my previous Evolve GT. The GT's dragster performance nearly knocked me off my feet. I wanted the flexibility to do that on my vesc driven board as well, and after researching and toying around with it enough, I've found a great solution, which brings us to...

**Max Current Ramp Step (at 1khz):**
For Vesc veterans, this should be a very familiar term. Last year (and still some today), nearly all vescs were plagued with a buggy version of the 2.18 fw which caused this value to multiply itself by 10 every time you wrote to the vesc [noted here](http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262). This has led to a bunch of burnt DRV chips and tears. Though there issue has been solved for newer 2.18 firmwares, Ive always been curious about the setting since it sounds like exactly what i want to mess with to get the performance i wanted. And i was right.

**What does it do?**
Credit to @Ackmaniac for explaining this one to me in another thread. The value indeed does affect acceleration response performance by controlling how fast the vesc ramps up from a given current to another. The math is as follows..

Given current / <"value"> / 1khz == time in seconds of how long it'll take to get from 0A current to given current in the motor.

[quote="Ackmaniac, post:7, topic:9249"]
To be a bit more precise what it means. It is only allowed for the VESC to increase or decrease the current settings by this value for every step. And there are 1000 steps each second (1000 Hz = 1 kHz). 
[/quote]

For example, assume the following:

* Motor Max = 50A
* Max Current Ramp Step (at 1khz) = .04 (default)

[quote="Ackmaniac, post:7, topic:9249"]
So to go from 0 to 50 Amps it needs 1250 Steps (50 / 0,04 = 1250 Steps / 1000 per second = 1,25 seconds).
[/quote]

In this case it would take 1.25 seconds to go from 0 to 50 amps of current in the motor, which is what I've noticed when doing dragster throttling at street lights. If you simply double the value (.08) you'll effectively cut that amount of time in **half**. Let's try this again.

50A / .08 / 1000 = .625 seconds!

Before going crazy with increasing Motor Max current to insane levels, try playing around with this setting to see if it'll suit your needs for better accelerating/braking performance. Just be careful not to set the value too high as it may cause the vesc to ramp up way too quickly and burn out the DRV or other components
```

---
## \#2 Posted by: BigBoyToys Posted at: 2017-08-02T00:55:25.648Z Reads: 196

```
I had to make substantial adjustments to these as well to get my 4wd board to ride smoothly with the high battery and motor amp settings I am running. I cut the ramp up in half and doubled the ramp down and it tamed the beast! Ramp down was an was especially big improvement. Prior to the adjustment if you let off the accelerator abruptly it would almost buck me off. Now its much more manageable but will still try to rip you a new one if you try and bury the throtttle.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-08-02T01:00:06.450Z Reads: 191

```
Awesome thread @Jinra
This kind info is gold.
So what would you call a safe ramp up limit and does it depend on motor max current?
And what about the Duty Ramp Step? What's the story with that setting?
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-02T01:38:41.237Z Reads: 182

```
@evoheyax You might want to try this out sometime. You can probably get similar throttle performance without the crazy current settings.
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-08-02T02:10:19.644Z Reads: 170

```
Be aware that this is only the case for BLDC Mode. FOC doesn't use the parameter.
```

---
## \#6 Posted by: Jinra Posted at: 2017-08-02T02:44:43.581Z Reads: 162

```
True, is there an equivalent calculation on the vesc for FOC?
```

---
## \#7 Posted by: Randyc1 Posted at: 2017-08-02T02:53:38.311Z Reads: 161

```
Is your accelaration as good as the GT now?

Wonder what the setting on the Vesx X is on the Raptor2 ?, which from tests i've seen on youtube accelarates faster that the GT ?
```

---
## \#8 Posted by: Namasaki Posted at: 2017-08-02T03:13:48.975Z Reads: 154

```
isn't the Raptor 2 running on FOC?
```

---
## \#9 Posted by: treenutter Posted at: 2017-08-02T03:38:24.955Z Reads: 151

```
@Jinra thanks for unpacking this setting! I had been ignoring it but now I'll explore!
```

---
## \#10 Posted by: jmasta Posted at: 2017-08-02T04:39:24.017Z Reads: 150

```
Shiiiit. I unknowingly ran a current ramp step maxed out at **50**, instead of the default 0.04, for months
```

---
## \#11 Posted by: Eboosted Posted at: 2017-08-02T04:42:12.778Z Reads: 146

```
At what point would it become dangerous? I'm gonna decrease the current value by half as you suggested and will report back.

@ackmaniac any possibility to include this parameter on  Vesc Monitor?
```

---
## \#12 Posted by: Jinra Posted at: 2017-08-02T04:45:08.178Z Reads: 144

```
I actually doubled mine, not cut off half
```

---
## \#13 Posted by: evoheyax Posted at: 2017-08-02T05:33:53.010Z Reads: 140

```
Thanks for the advice. Will look into it. I do miss the few mph top speed I lose from FOC. Would really like to get to at least 30 mph. I'm going to rewind all of my motors this week to hopefully about 100 kv. Will give me a slight boost in top speed. If all goes as planned, I'll be ready with rewound hummie motors by Sunday.
```

---
## \#14 Posted by: Titoxd10001 Posted at: 2017-08-02T05:38:25.059Z Reads: 136

```
We need DUTY CYCLE to get good acceleration and speed based control. It doesn't have neutral though in vesc 😭
```

---
## \#15 Posted by: trancejunkiexxl Posted at: 2017-08-02T07:47:08.778Z Reads: 131

```
afraid to try this on BLDC w/ FOCBOX will wait for other vesc to arrive to try.. did anybody run bldc on BOX yet?
i thought they were specifically designed to run in FOC mode best
```

---
## \#16 Posted by: Jinra Posted at: 2017-08-02T13:16:06.083Z Reads: 127

```
people run bldc all the time, it's safer than foc
```

---
## \#17 Posted by: pshaw Posted at: 2017-08-07T16:20:41.769Z Reads: 110

```
@jinra where did you ever end up with your ramping? did you keep it doubled at .08? Any issues or concerns since you have been running it?
```

---
## \#18 Posted by: Jinra Posted at: 2017-08-07T16:23:48.794Z Reads: 112

```
I use .1 now. No issues so far
```

---
## \#19 Posted by: pshaw Posted at: 2017-08-07T16:24:53.465Z Reads: 111

```
What about the ramp down? Did you mess with that any? Are these settings in the advanced tab as I haven't seen these anywhere I don't think...
```

---
## \#20 Posted by: Jinra Posted at: 2017-08-07T16:31:49.139Z Reads: 109

```
max current ramp step also controls ramp down
```

---
## \#21 Posted by: Randyc1 Posted at: 2017-08-07T18:07:35.612Z Reads: 104

```
Is your accelaration as good as the GT now?

Wonder what the setting on the Vesx X is on the Raptor2 ?, which from tests i've seen on youtube accelarates faster that the GT ?
```

---
## \#22 Posted by: Jinra Posted at: 2017-08-07T18:11:06.625Z Reads: 103

```
Settings for the raptor 2 are..

> Motor max 60
Motor min -60
Battery Max 30
Battery Min -8

My board doesn't out accelerate the GT or Raptor 2 as my kv is too high and my motors are shorter than both the aforementioned boards. Though my board does go faster than both. The acceleration on mine is definitely enough for me though, and the max current ramp step adjustment did help with that.
```

---
## \#23 Posted by: Randyc1 Posted at: 2017-08-07T18:14:57.303Z Reads: 101

```
For a fair test each would have to be geared for same Top Speed maybe?
```

---
## \#24 Posted by: Jinra Posted at: 2017-08-07T18:17:26.318Z Reads: 101

```
For a test of acceleration? Yea I'd agree. I had 190's on there before but swapped them out for 230's a couple months ago. I really want to see a dual 6374 170/190kv build go against the Raptor 2.
```

---
## \#25 Posted by: Bloop Posted at: 2017-08-07T18:38:03.172Z Reads: 99

```
so making the max current ramp 0.08 will make my board accelerate to max faster is that what it is? Will this help with the motor not starting from still or starting really hard ?? or for that i only need to play with startup boost ?

What would be good values for both so i can start faster at street lights ? 

Thank you
```

---
## \#26 Posted by: Jinra Posted at: 2017-08-07T18:40:45.969Z Reads: 100

```
If you want to start smoothly from standstill you'll need sensors. It'll help with response time for fast acceleration. With .08 value you'll acclerate from 0 to 80 amps in 1 second.
```

---
## \#27 Posted by: Crossfire Posted at: 2017-08-08T07:17:34.847Z Reads: 92

```
Out of curiosity - what setup do you ride these days? Sounds like dual 230kV's on 10S?
I'm currently on a single SK3 245kV on 8S. Feels great to start with. I'll upgrade it to focbox later on, maybe add 2S to it or even go 192kV route. But 245kV on 10S with focbox might be quite a ride :)
I'll probably ramp it up to .08 for a more responsive acceleration.
```

---
## \#28 Posted by: Jinra Posted at: 2017-08-08T07:21:05.249Z Reads: 91

```
yep dual 230kv on 10s. It puts me right at the erpm limit. You may go over with 245kv, but who knows maybe the focbox can take it.

I actual want to do a 12s4p dual 6374 190kv build for maximum torque
```

---
## \#29 Posted by: Crossfire Posted at: 2017-08-08T07:30:19.965Z Reads: 95

```
I'll definitely limit it to 60,000 erpm if I go down that route or else that transistor should do it's job protecting the DRV's.

Well, idea of adding another 4S to the build on dual sensored 190 kV with focboxes, 12mm drives, 210mm trucks and 97 abecs is a right way to wet them pants. :slight_smile:
Maybe even lower kV for 12S? like 170?
```

---
## \#30 Posted by: Jinra Posted at: 2017-08-08T07:37:01.387Z Reads: 94

```
That's an option, you can always compensate for lower kv with more aggressive gearing for better top speed.
```

---
## \#31 Posted by: Cobber Posted at: 2017-08-08T07:54:08.474Z Reads: 93

```
Cool, if the VESC's had more horse power I'd give them a go.
My scorpion speed controllers have a similar function
"MAT= MOTOR ACCELERATION TIME DELAY: 1: 0.15 Seconds* (recommend for AIR 2), 2: 0.3 Seconds, 3: 0.45 Seconds, 4: 0.7 Seconds, 5: 1.3 Seconds"
essentially it takes the selected amount of time to deliver the change in throttle position...
```

---
