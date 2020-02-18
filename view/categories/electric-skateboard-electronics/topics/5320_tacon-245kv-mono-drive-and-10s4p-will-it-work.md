# Tacon 245kv mono drive and 10s4p&hellip; Will it work?

### Replies: 45 Views: 2547

## \#1 Posted by: Airmacx Posted at: 2016-06-29T11:58:39.902Z Reads: 158

```
After searching around for other Tacon motor builds, I saw a lot of replies saying that because it's 245kv, it might not be the best in terms of general performance, climbing hills etc ( I don't plan on climbing *very* steep hills, 10-15% at most, but rarely). I'm building a 10s4p with Samsung 18650 batteries, just wanted to make sure everything would be fine, no problems. Will be using an Enertion VESC too.
```

---
## \#2 Posted by: Randyc1 Posted at: 2016-06-29T15:08:51.398Z Reads: 151

```
I have basically same motor 6463-245kv in my setup and it works great ! https://youtu.be/RQ7u_qhJxi0

,... slightly lower Kv would be better not to go over erpm at full charge(42v),  but other than that works great !

You could also get the 6374 192kv which is what i got for next single build.
```

---
## \#3 Posted by: Airmacx Posted at: 2016-06-29T15:40:43.704Z Reads: 141

```
Looks great! Thanks for the info.
```

---
## \#4 Posted by: shred Posted at: 2016-06-29T15:59:53.967Z Reads: 145

```
@Randyc1 what do you mean with "over erpm"? 60.000 or 100.000?

@Airmacx see this thread:
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125

I got a 10S with 190kv and get between 80% and 85% efficiency, wondering if I should upgrade to a 213kv from HK. This way I would end up with erpm 62174.70 while fully charged at 41.7V and guess that would be still fine, not sure higher kv than that is a great idea. I don't really have a clue though, still playing ;)
```

---
## \#5 Posted by: treenutter Posted at: 2016-06-29T16:01:16.157Z Reads: 127

```
@chaka has done the math (and has a lot of experience) and has found that the voltage associated with 10S is too high for a 245KV motor when paired with VESC. It would be more ideal to use a motor 200KV or lower. If you use the 245KV with 10S, use the ERPM setting in VESC to reduce RPM below 60K.  

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#6 Posted by: chaka Posted at: 2016-06-29T16:02:02.121Z Reads: 117

```
Depends on how fast your top speed is. If it is low you can easily exceed 60k coasting down a hill.
```

---
## \#7 Posted by: treenutter Posted at: 2016-06-29T16:04:09.338Z Reads: 115

```
Ha @shred looks like you beat me to it by 2 minutes!
```

---
## \#8 Posted by: Airmacx Posted at: 2016-06-29T16:12:23.919Z Reads: 117

```
So, I can use 245kv with 10s, just have to tone it down a bit?
```

---
## \#9 Posted by: treenutter Posted at: 2016-06-29T16:19:33.018Z Reads: 111

```
[quote="Airmacx, post:8, topic:5320, full:true"]
So, I can use 245kv with 10s, just have to tone it down a bit?
[/quote]


@Airmacx that is what I take away from @chaka's post, but he should confirm before you commit that config.
```

---
## \#10 Posted by: Randyc1 Posted at: 2016-06-29T16:22:15.522Z Reads: 108

```
According to Chaka 60,000 erpm
```

---
## \#11 Posted by: shred Posted at: 2016-06-29T16:42:58.318Z Reads: 109

```
thanks @chaka

I got a 190kv, 10S, 83mm, 15/36 and get a real max of around 38kph fully charged, which is around 85% efficiency, overall I guess efficiency is more like 80%, like 35kph (especially when the battery is at less or around 50% charge). 

A upgrade to 213kv would bring me up to a max erpm of 62174.70 with a theoretical top speed of around 50kph, assuming that I only have between 80% and 85% of efficiency I should as well still be fine in re to the 60k erpm mark right? 

Need to think about it all, guess I just go for a run :) Really wondering where I loose efficiency.
```

---
## \#12 Posted by: Jinra Posted at: 2016-06-29T16:53:02.807Z Reads: 104

```
Keep in mind you can easily reach 100% efficiency speeds during a decline.
```

---
## \#13 Posted by: chaka Posted at: 2016-06-29T17:05:11.475Z Reads: 100

```
254kv at 10s is not a very good idea unless you don't mind drv failures. It will work but it will eventually cause failures and faults during braking.
```

---
## \#14 Posted by: shred Posted at: 2016-06-29T17:07:28.329Z Reads: 104

```
I guess so. Not having many hills here though. 

But that basically means what you guys are saying is: better stay low KV and pimp your gearing and wheels if needed.
```

---
## \#15 Posted by: Jinra Posted at: 2016-06-29T17:12:00.193Z Reads: 105

```
yep! There's a reason the big players are staying under 200kv. My Evolve GT runs a 130kv motor with a very low 2.13:1 reduction.
```

---
## \#16 Posted by: willpark16 Posted at: 2016-06-29T17:18:48.868Z Reads: 102

```
go 8s 4p or 5p and ur good to go it will also be easier to find a charger if u wanted that instead of a bms
```

---
## \#17 Posted by: Airmacx Posted at: 2016-06-29T17:27:35.219Z Reads: 101

```
Well, I already have the motor, so do I just build a smaller battery pack?
```

---
## \#18 Posted by: willpark16 Posted at: 2016-06-29T17:32:37.565Z Reads: 101

```
im running the same setup as u
```

---
## \#19 Posted by: Jinra Posted at: 2016-06-29T17:33:45.732Z Reads: 102

```
either smaller pack, or limit the eRPM on the VESC
```

---
## \#20 Posted by: Airmacx Posted at: 2016-06-29T17:36:38.068Z Reads: 102

```
Okay, probably limit the eRPM, since I already have all the batteries. So what exactly does it do? It limits the RPM of course, but physically, what will it do, just slow down the general speed of the board?

Also, how do I limit it? Software? Can it be done on the VESC itself?
```

---
## \#21 Posted by: Jinra Posted at: 2016-06-29T17:37:33.881Z Reads: 95

```
Yea, the VESC won't accelerate past the limit. You do it through BLDC tool (VESC program)
```

---
## \#22 Posted by: Airmacx Posted at: 2016-06-29T17:41:23.485Z Reads: 93

```
Ah cool, what should I limit it to? Luckily this is an option, I don't think I had an option to return my motor haha, so this kinda saved me.
```

---
## \#23 Posted by: Jinra Posted at: 2016-06-29T17:42:57.912Z Reads: 92

```
60,000 erpm. It is more preferable to get the right motor, but if you don't want to this will work as well.
```

---
## \#24 Posted by: Airmacx Posted at: 2016-06-29T17:47:49.257Z Reads: 93

```
Yeah, unfortunately I got my whole deck, trucks and motor in one 'deal' that costs around the same as just one of the Enertion 2.0 motors. I could get the less expensive one. How much different is it? One is $159 and the other is $219, other than the size and wattage, I don't see there's that much of a difference? Is the more expensive one worth it?
```

---
## \#25 Posted by: willpark16 Posted at: 2016-06-29T17:48:56.218Z Reads: 91

```
since its a tacon u can sell it and get a 190kv motor which is now in stock or go 10s with the tacon but there have been multiple drv failures when running 245kv or higher motors on 10s. or u can simply run 6 or 8s with your current motor

edit this would be the 190kv hobbyking motor which is considered one of the best setups for the vesc
```

---
## \#26 Posted by: Airmacx Posted at: 2016-06-29T17:50:58.487Z Reads: 90

```
Hmm. Would anyone want to buy the motor? How much would I sell it for? I'd like to get atleast half of what the Enertion motor costs. Would 100 USD be an okay price?
```

---
## \#27 Posted by: willpark16 Posted at: 2016-06-29T17:51:35.745Z Reads: 93

```
if u go 60- 70 then id take it off ur hands
```

---
## \#28 Posted by: willpark16 Posted at: 2016-06-29T17:52:12.264Z Reads: 97

```
the enertion motor is great but why not just pay 70 for the hobbyking motor thats just as great for half that
```

---
## \#29 Posted by: Jinra Posted at: 2016-06-29T17:54:10.634Z Reads: 100

```
You have plenty of options. I'm getting 2x Ollinboards (chaka) motors in 200kv myself. Torqueboards also has good motor options. I've heard from Chaka that 50mm motors run more stable than the larger 63's which is why I chose his.
```

---
## \#30 Posted by: willpark16 Posted at: 2016-06-29T17:55:49.333Z Reads: 97

```
i heard the same about the 50mm vs the 63mms but is it just the mount thats an issue, the vesc, or the motors themselves
```

---
## \#31 Posted by: Airmacx Posted at: 2016-06-29T17:55:50.973Z Reads: 88

```
Has the bigger motor thing got anything to do dual motors? I'm only running single motor.
```

---
## \#32 Posted by: Jinra Posted at: 2016-06-29T17:56:59.146Z Reads: 84

```
I wouldn't think so, but I'm not sure.
```

---
## \#33 Posted by: Airmacx Posted at: 2016-06-29T18:00:28.650Z Reads: 84

```
I see. Ollin looks super nice, all black. I'm seriously thinking about that one 200kv. I'll get a slower top speed, but still, I never go fast anyways. Will a single one go up hills okay?
```

---
## \#34 Posted by: Airmacx Posted at: 2016-06-29T18:01:26.982Z Reads: 83

```
Well it's an Australian business, so fast shipping, easy warranty stuff, same time zones etc, it's easier to buy nationally, rather than internationally.
```

---
## \#35 Posted by: Jinra Posted at: 2016-06-29T18:01:57.891Z Reads: 85

```
Chaka seems pretty confident on them with 14/36 gearing (recommended). I'm using very similar motors on my Evolve GT and it completely eats hills; I go up hills at 18mph.
```

---
## \#36 Posted by: Airmacx Posted at: 2016-06-29T18:04:11.214Z Reads: 87

```
Oh sweet. You're talking about single drive going up hills? Or two motors? It might be a bad move, but I used the calculator and says I should get around 20mph. I'm gonna use Boosted's drive wheels, since I had them, got them for free from a friend, and didn't have to put money into hub and all that. Bought the pulley, and 15mm belts. So 14/50 ratio? I think. 14 teeth on the pulley, and 50 on the wheels.
```

---
## \#37 Posted by: Jinra Posted at: 2016-06-29T18:07:41.213Z Reads: 90

```
Oh sorry, Evolve GT has 2 motors. That's quite a big reduction. I think you should be fine for most hills though. My gearing for my build will get me to 30mph with the 200kv ollin motors.
```

---
## \#38 Posted by: Airmacx Posted at: 2016-06-29T18:09:57.524Z Reads: 90

```
I see. Well how does this sound so far: My option is to sell the Tacon, or just keep saving for a new one. 

10s4p battery, 14/50 gearing ratio, with the 200kv Ollin motor (single drive)- 20mph with a 76mm wheel size (Orangatang in heat) Sounds pretty okay to me. 

Edit: I think I'll go with Enertions. With shipping ($60) and conversions it'll cost me $170, may as well just get the Enertion one.
```

---
## \#39 Posted by: Jinra Posted at: 2016-06-29T18:12:57.146Z Reads: 87

```
Sounds good :)
```

---
## \#40 Posted by: Airmacx Posted at: 2016-06-29T18:25:34.257Z Reads: 85

```
So, there's two Enertion ones, one has 2400W and the other has 3200W. Is it worth spending the extra $70 on the one? 3200W?
```

---
## \#41 Posted by: Jinra Posted at: 2016-06-29T18:27:34.832Z Reads: 83

```
If you're going single drive, you should probably go with the 6374 (3200w). If you want to go dual get the 6355 (2400w).
```

---
## \#42 Posted by: Randyc1 Posted at: 2016-06-29T20:34:18.597Z Reads: 78

```
Can you explain how this happens during braking chaka ?

Thanks.
```

---
## \#43 Posted by: chaka Posted at: 2016-06-29T21:38:41.889Z Reads: 78

```
When brakes are applied you can get a high current spike that can potentially damage the VESC or BMS modules. This is less of an issue on smaller motors but it is exacerbated by high erpm values at the time of initial braking on 63mm motors.
```

---
## \#44 Posted by: Randyc1 Posted at: 2016-06-30T02:35:34.188Z Reads: 71

```
So using brakes at high speeds causes high Amp load, ..how high can it reach ??...is'nt the vesc good for 240A for a few seconds ?
```

---
## \#45 Posted by: chaka Posted at: 2016-06-30T03:17:17.386Z Reads: 71

```
I have only noticed this behavior when pushing the erpm really high on larger motors.
```

---
