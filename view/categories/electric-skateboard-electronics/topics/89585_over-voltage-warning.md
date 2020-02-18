# Over voltage warning

### Replies: 18 Views: 252

## \#1 Posted by: Sascha_stevenson Posted at: 2019-04-06T14:49:36.654Z Reads: 78

```
Hello everyone,
I've recently been receiving over warnings from my vest and didn't used to have them. I'm no battery expert and would like to get this fixed for riding in summer and don't want to kill a focbox. anyone got any ideas? if you need anymore info just let me know

Thanks
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-06T16:17:19.019Z Reads: 72

```
Hey! Yap some more infos would be nice.

Let us know which battery you use. Do you use a bms, an anti spark and how long are your wires from battery to vesc and from vesc to the motors (just round about, doesn’t need to be exactly on the cm)
```

---
## \#3 Posted by: Sascha_stevenson Posted at: 2019-04-06T21:37:49.668Z Reads: 52

```
hey @Andy87 I have a 7s2p mboards battery, I do use a BMS, I use an XT90 Antispark loop key, Battery to Vesc about 20-30cm and the same for vesc to vesc to motor.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-04-07T08:10:18.267Z Reads: 34

```
Hm all that seems good and shouldn’t be a reason for the over voltage fault. Did you change something in your battery settings while set up your motors? I mean did you change the operating voltage range (8-60V I think) to any other value?
```

---
## \#5 Posted by: Sascha_stevenson Posted at: 2019-04-07T08:11:29.078Z Reads: 30

```
No its still all the same, I will post a picture of the vesc settings in a minute
```

---
## \#6 Posted by: Andy87 Posted at: 2019-04-07T08:15:07.081Z Reads: 28

```
Hm. Honestly I never had this issue so i‘m not aware what it can be, but if you have issues with focbox it’s always worth a try to tag our official wizard @JohnnyMeduse maybe he can guess from where the voltage warnings coming.
```

---
## \#7 Posted by: taz Posted at: 2019-04-07T08:16:31.564Z Reads: 30

```
Over voltage warnings can also come from a bad connection.
When I had a broken series connection in a pre-made pack I got over-voltage warnings.
At least it forced me to start making my own packs. :smirk:
```

---
## \#8 Posted by: Sascha_stevenson Posted at: 2019-04-07T08:18:06.322Z Reads: 29

```
I will have a good look over all the connections now,
also here are the settings i use![12|690x417](upload://m0izZphYHZyL5frarIO3ACrOQK4.png)
```

---
## \#9 Posted by: Andy87 Posted at: 2019-04-07T08:22:08.033Z Reads: 26

```
Just a side note. You will not reach your max erpm with 7s as long as your motor kV is not over the top, but non the less take away the tick at „Limit max erpm with negativ torque“

It basics hit you off the board as soon as you reach your max erpm. Something you don’t want.
```

---
## \#10 Posted by: Sascha_stevenson Posted at: 2019-04-07T08:33:29.182Z Reads: 21

```
just did that now, thanks!
```

---
## \#11 Posted by: taz Posted at: 2019-04-07T08:35:54.523Z Reads: 21

```
Also, I would suggest you upgrade your firmware and switch to VESC Tool.
One of the big differences was the introduction of a feature called "temperature acceleration decrease".

This basically allows you to set different temperature limits between accelerating and braking when the vescs or motors overheat. So when you reach the top of that hill the board starts to slow down but you still have brakes going down.

Before that feature I was left without brakes quite a few times and let me tell you it was not fun at all.
```

---
## \#12 Posted by: Sascha_stevenson Posted at: 2019-04-07T08:40:09.319Z Reads: 20

```
I'm afraid of updating the firmware, because last time I did I killed my focbox. but it sounds like i have a similar issue. sometimes i would start to brake and then it won't anymore for like 4sec
```

---
## \#13 Posted by: Andy87 Posted at: 2019-04-07T08:42:44.337Z Reads: 19

```
[quote="Sascha_stevenson, post:12, topic:89585"]
it won’t anymore for like 4sec
[/quote]
If you use your bms for charge and discharge that could also be caused by your bms.
```

---
## \#14 Posted by: Sascha_stevenson Posted at: 2019-04-07T08:43:35.600Z Reads: 16

```
@Andy87 what could I do to solve this?
```

---
## \#15 Posted by: Andy87 Posted at: 2019-04-07T08:50:26.875Z Reads: 16

```
Which bms you have?
If the bms has a too low discharge protection (like 15A or so) it will cut out. In this case get a better bms.

What every bms wired for discharge will make is to cut out if you start breaking with fully charged batteries. It’s to prevent your pack from overcharging. What you can do here, just charge your pack till 4.1-4.15V per cell only or wire up the bms as charge only. Be aware that as charge only the bms will not take care about over current, over discharge etc. and if you have an integrated e-switch to switch on/off your board that function will not work anymore as well.
```

---
## \#16 Posted by: Sascha_stevenson Posted at: 2019-04-07T08:57:14.976Z Reads: 15

```
if im going to be upgrading the battery soon anyway with https://eskating.eu/product/10s4p-eskating-electric-skateboard-battery-samsung-30q/?v=7516fd43adaa do you think i will still have the problem?
```

---
## \#17 Posted by: Andy87 Posted at: 2019-04-07T09:15:15.092Z Reads: 16

```
The bms they use in there packs are good ones from bestech. You shouldn’t get cut offs with it besides the situation when you start driving with fully charged pack. Just try to avoid to drive down a hill the first kilometers after you charged up your pack and all should be good.
```

---
## \#18 Posted by: Sascha_stevenson Posted at: 2019-04-07T09:28:59.450Z Reads: 15

```
cool thanks Andy, I guess we got a bit off topic but I still need to find a solution to the over voltage problem.
```

---
