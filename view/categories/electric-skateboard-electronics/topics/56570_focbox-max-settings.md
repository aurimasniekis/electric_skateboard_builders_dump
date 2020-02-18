# FOCBOX Max settings?

### Replies: 9 Views: 1168

## \#1 Posted by: Pingo03 Posted at: 2018-05-24T06:17:12.535Z Reads: 287

```
Hello,
Nobody seems to know the really answer but how high can I set my different Amps and still be safe on a Focbox on a single 6374 Motor setup and 10s4p 30q pack?

I want no experimenting but the max settings proven to be ok

Thanks!
Ben
```

---
## \#2 Posted by: lrdesigns Posted at: 2018-05-24T07:58:06.882Z Reads: 278

```
This topic is beaten around all the time I'm sure the answers are searchable. But I will throw you a bone. 

Leave them all at stock settings and try it out first to see if the power is enough for you. 

After that you can set the battery max at 60 amps which is the max your battery can handle and will limit max system power.

Motor amps can be turned up if you need more low speed torque. Maybe 90 amps max for this size motor but check its not getting hot to confirm its ok.
```

---
## \#3 Posted by: b264 Posted at: 2018-05-24T08:45:15.811Z Reads: 270

```
The reason it's not straightforward is because the maximum settings are all based on semiconductor junction temperature, and not amount of amperes.  So, it depends on a lot of things specific to your ESC and specific to how it's mounted and the weather outside.
```

---
## \#4 Posted by: Pingo03 Posted at: 2018-05-24T09:01:01.511Z Reads: 261

```
yes I did my research and nobody really confirmed that it would be save running the battery max up higher then 40.

Has anyone been running on a Batt max on 60 without having troubles?
Can I adjust it to 60 with a bestech bms rated to 60ps or should I stay below and if yes how low?

How high do you run your motor max up, up to the limit maytech is providing for their motors? What should be Max temperature?


Thanks Ben
```

---
## \#5 Posted by: Sebike Posted at: 2018-05-24T10:09:04.580Z Reads: 240

```
Been running with batt max at 60Aish through SuPower 60A BMS and focbox on single motor (and later 2x30A batt max for dual motors). 

Haven't had a problem with heat or anything else related to these settings.
```

---
## \#6 Posted by: Hummie Posted at: 2018-05-24T18:42:55.439Z Reads: 217

```
how bout motor amp setting possible?  havent found that for the focbox.
```

---
## \#7 Posted by: cypa9904 Posted at: 2018-07-22T22:11:11.503Z Reads: 172

```
[quote="Sebike, post:5, topic:56570, full:true"]
Been running with batt max at 60Aish through SuPower 60A BMS and focbox on single motor (and later 2x30A batt max for dual motors).

Haven’t had a problem with heat or anything else related to these settings.
[/quote]

Hi! May I ask you a question? 
Why is that "and later 2x30A batt max for dual motors"?

That mean you did not want to get more power OR it gave you twice the power because the battery current sums up or something like that?
 I do not understand it and I could not find the answer why is that because I was pretty sure that I saw this a few months ago :slight_smile:

Because what I do not know is what batt max should I have on 2 focboxes and 1 power supply because I am not sure how it works now.... 

Here are 2 possibilities:
I should go 2 motors max amps 80 and 2 batt max 80 amps 

or

I should go 2 motors max amps 80 and 2 batt max 40 amps. 

(and then it will 'suck' 80 amps for each focbox or 40?)


Will you help me, please? :D I am a mountainboard user and I want to have quite much power but I do not want to burn my focboxes :smiley: 


Regards :grin:
```

---
## \#8 Posted by: professor_shartsis Posted at: 2018-07-22T22:42:39.822Z Reads: 152

```
[quote="cypa9904, post:7, topic:56570"]
I should go 2 motors max amps 80 and 2 batt max 40 amps.

(and then it will ‘suck’ 80 amps for each focbox or 40?)
[/quote]


Both.

Suppose at a certain point during your acceleration you have the 80a motor max setting and 40a battery max setting per vesc.

At a certain specific RPM (depending on your winding resistance and KV) it will require exactly 50% duty cycle to "draw" 40a from the battery.

The 50% duty cycle means power is drawn from the battery 50% of the time. (a different duty cycle is required to sustain 40a battery at every different speed -- this is done automatically by the VESC.)

In this case with BLDC, what 40a battery @ 50% duty cycle literally means is 80a battery current half (50%) of the time (averaging to 40a) -- switching on and off approximately 20,000 - 30,000 times per second frequency.

That is what the battery "sees" but on the motor side things are different.

On the motor side, due to the inductance of the winding and the fact the motor leads are shorted to themselves during the battery off time, the current generated during the battery on time continues to flow inductively through the motor winding during the "battery off" time and the motor current changes very little during each on/off cycle. This means the motor will "see" 80a motor current the entire time at half (50% duty) the battery voltage (duty cycle lowers effective voltage), while the battery sees 80a half (50%) of the time (averaging to 40a) at the full pack voltage.

40a battery * 25v battery = 1000w = 80a * 12.5v effective voltage

80a motor * 50% duty cycle = 40a battery

25v battery * 50% duty cycle = 12.5v effective voltage
```

---
## \#9 Posted by: Sebike Posted at: 2018-07-22T22:44:49.761Z Reads: 133

```
my battery can deliver 60-80 amps without overheating, but my bms is rated at 60a discharge, so I don't want to exceed this amp draw (60A) which is either batt max 60A for one vesc or 2x 30A batt max if running 2 vescs.

if you run 2 vescs and your battery can deliver 80A (and you use a bms for discharge and it's rated 80+) you can run batt max 40A per vesc and 80 motor max if that's the setting you prefer.
```

---
