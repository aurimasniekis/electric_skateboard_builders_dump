# How to get more braking force with a weak battery?

### Replies: 49 Views: 733

## \#1 Posted by: rusins Posted at: 2018-09-12T06:46:04.233Z Reads: 218

```
_Situation:_ I have a 12s2p battery made from LG HB6 cells, which I thought would be perfect for my needs, because then I could safely draw 60A continuously from them. (The cells are low-capacity high power draw :slight_smile:) However, the cells are rated for a maximum charge rate of 4A each, meaning my pack can safely only support 8A regenerative breaking. Now, unfortunately I don't have a bluetooth module, so am not fully certain this is the limit I'm reaching, but it sure feels like it! Actually stopping at stop signs is nearly impossible, and the breaking distance is way too long for me to feel safe cruising in traffic.

So: Have I messed up with my battery choice? Is this charge rate limit just a guideline? How does breaking work for people that don't have an integrated BMS with charging support? Perhaps there's large enough capacitor or something that I should add in series to the battery to take this charge? (And that could reduce voltage sag, but my battery is powerful as is tbh :smiley:)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-12T06:49:23.934Z Reads: 214

```
which motor (s) you have?
what your motor min settings
things which have more influence on your breaking than the bat min setting
```

---
## \#3 Posted by: Acidfie Posted at: 2018-09-12T06:50:26.668Z Reads: 209

```
Brake Force ≠ Regenerative Braking
```

---
## \#4 Posted by: rusins Posted at: 2018-09-12T06:50:38.257Z Reads: 203

```
I have dual DIYelectric 6355 190KV sensored motors running in FOC mode
Motor min is -49A, motor max is 49A (They're 2500W, so I divided that with 50.4V)
```

---
## \#5 Posted by: Acidfie Posted at: 2018-09-12T06:51:05.808Z Reads: 198

```
your motor is easily rated for min 60a to about 80 amps
```

---
## \#6 Posted by: rusins Posted at: 2018-09-12T06:52:31.879Z Reads: 195

```
Hmmm, that is true, but wouldn't the VESC take the minimum of my motor limits and my battery limits?
```

---
## \#7 Posted by: Andy87 Posted at: 2018-09-12T06:55:17.016Z Reads: 191

```
you should get a good breaking with your actual settings
already. 
You can set up your bat min to about -16 (so -8, -8)
it´s not a problem as long as you don´t go down a 3km hill while breaking all the time.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-09-12T06:56:13.923Z Reads: 188

```
[quote="rusins, post:6, topic:67786"]
VESC take the minimum of my motor limits and my battery limits?
[/quote]

what you mean with it? don´t really understand
```

---
## \#9 Posted by: rusins Posted at: 2018-09-12T06:57:32.161Z Reads: 186

```
As in: it doesn't matter if the motor minimum is set to -49A, if the battery minimum is set to -4A, then it will only break so much that 4A get generated from the motor and put back into the battery.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-09-12T07:01:21.188Z Reads: 178

```
no that´s not right.
only 4A will go back to your battery as reg. breaking and charge up the battery.
but your motor produce heat and magnatic fields which result in the breakforce
```

---
## \#11 Posted by: Acidfie Posted at: 2018-09-12T07:01:39.484Z Reads: 170

```
ever wondered why the motor gets hot while braking? Rotational Force -> electrical force -> heat
```

---
## \#12 Posted by: rusins Posted at: 2018-09-12T07:02:28.718Z Reads: 170

```
Ah, so the heat gets directly dissipated in the motor! Interesting! I guess my throttle curve might not be strong enough in that case... (Unless someone can come up with a better explanation)
```

---
## \#13 Posted by: lrdesigns Posted at: 2018-09-12T07:04:23.660Z Reads: 174

```
[quote="rusins, post:1, topic:67786"]
LG HB6
[/quote]

You can increase your gear ratio for more braking power without adding more amps to your battery!! With a slight hit to your top speed being the only downside. 

While your max battery charge rate on the data sheet is 4amps, that is for a full charge from empty not a very quick bust of power you get stopping at a traffic light. Most of the users here would prefer to shorten there battery life then have a serious crash so will run more than the data sheet suggests. So long as the batteries do not get hot during charge there should not be much of an issue. Except for slightly shorter life span, but I have never seen any data on this.
```

---
## \#14 Posted by: rusins Posted at: 2018-09-12T07:06:49.634Z Reads: 162

```
Was thinking the same about life-span, thanks! I am running 14:36 already on 80mm wheels, so I don't think I'd want to sacrifice my top speed any more than it already is :smiley: (A bit off topic:) I have Orangutang wheels unfortunately, so upgrading to something bigger means buying new pulleys as well :confused: (they really need to release larger wheels)
```

---
## \#15 Posted by: rusins Posted at: 2018-09-12T07:09:18.891Z Reads: 159

```
Hold on, but if I understand correctly that all the energy that cannot be used to charge up the battery gets dissipated into heat anyway, then why even raise the charging limit? Just for more juice on the go? (I also read here on the forums that anything more than 0.1 seconds already counts as "continuous charge/discharge, so is it really safe?)
```

---
## \#16 Posted by: lrdesigns Posted at: 2018-09-12T07:14:01.414Z Reads: 150

```
If your motors can make 20amps under braking, and your vesc setting is -20a, then the vesc will try to put all of that into the battery. The vesc does not bleed of excess energy as heat intentionally. Although your battery might get annoyed and hot if you charge it too high for too long. But for 4 seconds your slowing down, double the data sheet of 8 amps should be fine. 

[Data sheet for LG HB6 for those interested.](https://keeppower.com.ua/download/01-2016/20130719-18650HB6-Rev1.pdf)
```

---
## \#17 Posted by: lrdesigns Posted at: 2018-09-12T09:28:15.861Z Reads: 139

```
[quote="rusins, post:14, topic:67786"]
I am running 14:36 already on 80mm wheels
[/quote]

Yeah, its pretty much low as you can go with 80mm wheels. How many mm between the ground and your belts on the wheel pulley? Also normally I don't recommend below 15t motor pulley, which motor mounts you using?
```

---
## \#18 Posted by: Kug3lis Posted at: 2018-09-12T09:30:05.515Z Reads: 141

```
Battery minus is basically your braking power, motor minus is basically maximum braking current so if you going full speed you will not have motor max as voltage will be the same as input so applying power formula you will have max braking power your battery minus. Everything else will go into heat as you shortening mosfets which means they connect phases and work as resistors so they also will produce some heat from their resistance, wires will heat up and motor coils too as you basically shortening you phase wires but that will not be as much braking force as you would drain that energy into battery.

EDIT: If you have -20 At battery and -50A at motor it will be like if at half speed your motor voltage is 25V so (20A * 50V = 1000W your maximum power capacity) so at half speed you will be able to brake with (1000W/25V = 40A)
```

---
## \#19 Posted by: rusins Posted at: 2018-09-12T10:55:54.579Z Reads: 127

```
Yeah, clearance with 85mm is not great at all :/ I usually step off and lift my board when going down / up a ledge. Although these wheels (Orangutang Caguamas) are amazing for a non-electric board (really great for going up/down ledges), at 40+ kmph the bump you feel with these 80A wheels is very unpleasant and worrying. Will try upgrading to the softer versions as they become available.

I'm using TB mounts, and TB motor pulleys. Belt hasn't slipped so far, and I don't use any idlers, so I think it's good.
```

---
## \#20 Posted by: rusins Posted at: 2018-09-12T10:57:43.280Z Reads: 124

```
Very interesting; I guess that explains why the breaks get stronger the slower I'm going, i.e. the breaking curve is very smooth, despite not having tinkered with it at all yet.
```

---
## \#21 Posted by: Kug3lis Posted at: 2018-09-12T11:00:25.189Z Reads: 118

```
I am running lipos with all currents set either +90 or -90 so I have good brakes all time maybe sometimes too good :D
```

---
## \#22 Posted by: Sender Posted at: 2018-09-12T11:36:23.431Z Reads: 113

```
Yeah, I set mine at -18 or -20 per Vesc on 10s6p.  I would go to -8 per VESC on your battery and feel just fine about it.  Like many have pointed out, it is only in short bursts, and brakes are nice..... even if it does *slightly* reduce battery life.  Worth it.
```

---
## \#23 Posted by: rusins Posted at: 2018-09-23T13:32:44.320Z Reads: 102

```
Alright, so I set my motor limits to +-80A each, and then limited total power per motor to +-2500W (so that I don't go over the specified limits collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-190kv)

What I noticed was that acceleration is even crazier now, but slowing down from top-speed is still very bad. Here's a video, where I'm going full-throttle, and then start breaking with full-throttle as I go over that speed-bumb:

https://www.youtube.com/watch?v=kJY_GhjOorI

See all the parked cars I passed? Well, that happened to me the other day in a traffic jam, and let me say – having to thread the needle between cars with no space to put your foot down to mechanically break is very scary :grimacing:
```

---
## \#24 Posted by: rusins Posted at: 2018-09-23T13:37:57.272Z Reads: 97

```
Here's a dump of screenshots from vesc tool, in case someone wants to look into them. (I haven't messed with anything except the very basics, that get set with the wizzards)

[details="Screenshots"]
General motor settings:
![image|690x143](upload://1J4BXejK5sVrg64F5sosQ2Meim4.png) 
![image|690x309](upload://1iJK8U5R2xUcccPwlxTmmBWB3v.png) 
![image|690x473](upload://qUILBHkSDomCTlvAJRW62w9rLkI.png)
![image|690x118](upload://3DSFA4j4GDJPcu9oMJ1hmeUt5Wa.png)
![image|690x105](upload://z7u0asJUJLqva50qkoEk5ldwA7P.png)
![image|690x230](upload://rNsN8z6dhFX5xNHQzJ3y8OZCNK8.png) 
![image|690x249](upload://8rSIf7xkf6gk3qpmZFoy24OFJHD.png) 
FOC settings:
![image|690x236](upload://mYqwBoad0q6LyMik9GqbOY1mELV.png) 
![image|690x272](upload://3sf6U1bDR8vVcYzFmtqORqrJLXM.png) 
![image|690x142](upload://dVeCQ914y6rlQEx0PeebmFFf5J9.png) 
![image|690x351](upload://95MSvhjzmuZrb9Uds2QFMGE9wQU.png) 
[/details]
```

---
## \#25 Posted by: Pedrodemio Posted at: 2018-09-23T14:02:25.714Z Reads: 93

```
You can increase the negative braking current until you are satisfied with it, as I always said, it’s better to have the battery last less due to to high braking current then need to brake one day in an emergency and don’t have enough power 

Do you have a Bluetooth module ? If so do a full brake from top speed to zero so we can see what’s happening
```

---
## \#26 Posted by: Kug3lis Posted at: 2018-09-23T14:06:42.273Z Reads: 93

```
Just be carefull overcharging Lions can lead to fire :) Always change a small bit and do testing and see how battery handles :)
```

---
## \#27 Posted by: Pedrodemio Posted at: 2018-09-23T14:07:51.228Z Reads: 92

```
Yeah, don’t go to crazy, but if it’s almost good you can increase a bit more

But if even with this settings is really weak then there’s is something wrong
```

---
## \#28 Posted by: Kug3lis Posted at: 2018-09-23T14:08:57.347Z Reads: 92

```
The idea is that at top speed because of Duty cycle your reach max voltage and braking is basically by bat min current so at top speed you only allowed to brake with 8A current, at slows speeds because duty is low you can brake a lot more ;)
```

---
## \#29 Posted by: rusins Posted at: 2018-09-23T14:21:13.621Z Reads: 90

```
That's for regenerative breaking, I was told in this very thread that battery limits shouldn't affect breaking, since it would just result in heat, and that's what I expected setting my motor min to -80A would do... :confused:
```

---
## \#30 Posted by: rusins Posted at: 2018-09-23T14:25:18.192Z Reads: 90

```
Speaking of which, is there other VESC firmware available that would be smart enough to raise these current limits when the voltage is low? I'm surprised it doesn't do that already, as -8A for the battery logically (at least to me) means that when it's breaking at low voltages, it should apply that current limit to the upscaled voltage it uses for charging the battery. :/ I guess I'll go out and buy a bluetooth module for further testing.
```

---
## \#31 Posted by: Kug3lis Posted at: 2018-09-23T14:31:48.507Z Reads: 88

```
Well that's for general braking, because of internal resistance of motor you will not have any much braking force so it would be even worse than without regenerative braking. Without load motor (which when braking turns into generator) doesn't have any load and spins almost freely.

There is no other firmwares as it works for everyone normally :) Just your battery is too small for this kind of application It would had made more sense going with lipos

EDIT: If you want shorten motor wires and try to spin... that's how much brake force you will have
```

---
## \#32 Posted by: Pedrodemio Posted at: 2018-09-23T14:35:42.169Z Reads: 88

```
The vesc only do regenerative braking with the exception in really slow speeds that it shorts all phases together, that happens because even at full pwm (95%) it can’t apply the current you want because of the low backEMF generated at low speed
```

---
## \#33 Posted by: rusins Posted at: 2018-09-23T15:21:14.602Z Reads: 86

```
Set min batery current to -10A per motor (-20A is the max my ESC can handle, and I definitely don't want to blow that up). Didn't help really, but I guess it's better than before. Lesson learned then: need to have more cells in parallel/different cell technology for future builds, so that I can break more.

Sidenote: 80A per motor sends me flying off (front of the board lifts up + belt skips) even when holding on with with my hand. Amazing :smiley:
```

---
## \#34 Posted by: danielz Posted at: 2018-09-23T20:23:45.737Z Reads: 74

```
This is incorrect. All braking is via regen only. (Check the vesc designers explanation over at the vesc tools forum.)
```

---
## \#35 Posted by: Andy87 Posted at: 2018-09-23T20:26:22.139Z Reads: 75

```
Only 4a goes back as charge to the battery...
What’s wrong with it?
```

---
## \#36 Posted by: Andy87 Posted at: 2018-09-23T20:40:02.057Z Reads: 71

```
Man...for sure it’s all regenerative...how else you wanna get a break force.
Sorry if my English is not good enough, but not all of your break energy goes as charge back to your battery that’s what I tried to say there.I have never seen a motor with 100% efficiency.
```

---
## \#37 Posted by: Tijmen Posted at: 2019-02-02T23:28:25.163Z Reads: 58

```
From the short video you posted + the comments you've been writing I'm getting the feeling you're dealing with belt slip here. How tight are your belts? It might be worth putting them tighter to get more grip when braking. I tend to go max speed, and then I hit full brakes, and if the belt doesn't slip then I increase the regen by 1A until I reach the point where it slips, and I back down again and then leave it there so I'm just at its limit
```

---
## \#38 Posted by: rusins Posted at: 2019-02-02T23:32:23.550Z Reads: 61

```
It's not belt slipping, that I would feel. (I once nearly fell off in front of a car do to one of my belts slipping – sent my board to the side instantly :smiley: 

The current breaking limits are manageable, I just need to try really hard to not ride aggressively XD (keeping my distance before cars, slowing down before I need to make a turn, etc.)
```

---
## \#39 Posted by: Tijmen Posted at: 2019-02-02T23:36:31.494Z Reads: 60

```
I too am not super satisfied with how hard I can brake, especially at high speeds, but as you mentioned I feel the most important thing is to ride safely and preemptively by slowing down a lot way before a turn or dangerous areas
```

---
## \#40 Posted by: pjotr47 Posted at: 2019-02-03T00:02:04.050Z Reads: 66

```
Maytech is selling a R-brake. With that you can have a better braking result.
```

---
## \#41 Posted by: rusins Posted at: 2019-02-03T00:10:48.776Z Reads: 64

```
I'm assuming you're talking about this?
https://www.aliexpress.com/item/Maytech-Rheostatic-Brake-Dynamic-Brake-for-ESCs-VESC-controllers/32967134495.html

Seems like that is meant for converting voltage too high for your ESC to a lower voltage that you can handle. I think that would only help if you were going down a hill faster than you'd go on a 12S setup, and wanted to break. Doesn't help in my case unfortunately. I need a capactior / battery thing that would allow me to charge it up with a lot of current :smiley:
```

---
## \#42 Posted by: pjotr47 Posted at: 2019-02-03T00:15:19.086Z Reads: 60

```
I thought it is just a big resistor that takes the extra ampères and burn it into heat. But I can be wrong. I have orderd one. So if I have it I can test it and let you know. 

Wikipedia definition off Rheostatic Braking:
The electrical energy produced by the motors is dissipated as heat by a bank of onboard referred to as the  *braking grid* . Large cooling fans are necessary to protect the resistors from damage. Modern systems have thermal monitoring, so, if the temperature of the bank becomes excessive, it will be switched off, and the braking will revert to friction only.
```

---
## \#43 Posted by: rusins Posted at: 2019-02-03T00:18:12.630Z Reads: 59

```
Oh, perhaps! I was just going off by what the aliexpress listing said. If it really is meant for dissipating electrical energy into heat, then that would be perfect! Do let me know how your testing goes! :slight_smile:
```

---
## \#44 Posted by: mishrasubhransu Posted at: 2019-02-03T00:31:16.903Z Reads: 55

```
I tried looking for a link but was unsuccessful. Could you point me?

It doesn't make sense that all braking is regen. Because the mosfets are used to create a shortcircuit of phase wires and when the short is removed, a voltage spike(>batt voltage) happens across the phase windings that is used to charge the battery(This is the principle behind boost regulators). So when shorted, it is still braking and it is **definitely not regen.**

Also, **braking has to happen at a higher speed** for regen to work properly. If the voltage spike that happens after the short is removed is not higher than the battery voltage, then no current flows into the battery. Only braking that happens then is because the mosfet is shorting the phase wires.
```

---
## \#45 Posted by: rusins Posted at: 2019-02-03T00:32:25.550Z Reads: 56

```
+1, would also like a link to read more about this
```

---
## \#46 Posted by: mishrasubhransu Posted at: 2019-02-03T00:32:55.829Z Reads: 56

```
It is going to work for you, until it reaches a high max temperature. Also it has 20AWG wire, so won't be able to push a lot of current through it.
```

---
## \#47 Posted by: rusins Posted at: 2019-02-03T00:34:48.998Z Reads: 52

```
Yeah, it says max 5A on the aliexpress page. Then again, having 25 rather than my current 20 would still be nice :smiley:
```

---
## \#48 Posted by: mishrasubhransu Posted at: 2019-02-03T00:38:29.958Z Reads: 52

```
You should be able to put multiple r brakes in parallel :rofl:
```

---
## \#49 Posted by: pjotr47 Posted at: 2019-02-03T01:10:26.364Z Reads: 49

```
20awg will work fine for 5A. It is a little bit warm at 4A continues. That is the reason why I use 18awg for charging wires on each battery pack. But because breaking is no continuous ampere, the wire can take more then 5amps with braking :slight_smile:
```

---
