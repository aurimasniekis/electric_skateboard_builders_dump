# Limiting BMS current draw from power brick

### Replies: 21 Views: 1391

## \#1 Posted by: Bataleon Posted at: 2018-03-18T20:44:16.340Z Reads: 135

```
After more than a year using a hobby charger, I finally connected a BMS (BesTech HCX-223V1) to my 10S LiFePO4 pack.

I managed to get it wired without anything catching-fire/burning (shout out to @Namasaki for his [helpful diagram](http://www.electric-skateboard.builders/t/connecting-a-bms-quick-guide-how-to/6122/59)) but noticed that when charging, the BMS draws 5A even though the power brick has a max rated output of 2A. Needless to say, the brick gets super hot after a few minutes.

According to the specs the BMS is capable of charging at a max of 20A, but I assumed that cos the power brick has a max output of 2A, then this would determine the upper charge rate?

Have I got something wrong? Were BesTech meant to set the BMS charge rate limit to 2A?

Any suggestions appreciated.

![IMG_1382_cropped|634x500](upload://ryVg5Glx8qyY1PAfTgeeduHzBkb.jpg)
```

---
## \#2 Posted by: Acido Posted at: 2018-03-18T20:52:09.948Z Reads: 126

```
The bms wont amp up the current, it charges with what it gets, if a power brick is capable of 2a it will charge with 2a

These bricks get pretty warm its nothing to be worried off, unless it super hot and bursts into flames, try charging your board outside and see if the charger catches fire lol
```

---
## \#3 Posted by: Namasaki Posted at: 2018-03-18T20:53:49.493Z Reads: 125

```
This is the problem with cheap 2a chargers. They have no means of internal cooling so they get hot.
As @Acido stated, the charger determines the charge rate.
```

---
## \#4 Posted by: Bataleon Posted at: 2018-03-18T21:33:39.270Z Reads: 109

```
Thanks for the replies. I'll see how long the charge brick is able to deliver 5A, hopefully nothing catches fire. It's so strange the brick doesn't limit the output to 2A (as listed on the enclosure), but it was cheap so there's probably almost no logic circuitry inside.

I guess a resistor could be used to limit the current (Ohm's law) but it would have to be massive. Not sure they even exist that big.
```

---
## \#5 Posted by: deucesdown Posted at: 2018-03-18T23:24:13.648Z Reads: 100

```
If you're getting 36v 5a out of the charger, throw it out! 2a chargers of that size get very hot. It's running so far out of spec I'd consider it very dangerous. At least don't charge unatteded.
```

---
## \#6 Posted by: Namasaki Posted at: 2018-03-19T02:04:27.781Z Reads: 83

```
Im curious, how did you measure the charge current?
```

---
## \#7 Posted by: Bataleon Posted at: 2018-03-19T08:48:59.611Z Reads: 78

```
@deucesdown I was thinking the same. Pulling 180w from a small power brick seems dangerous. Million dollar question though: how do you prevent your BMS from pulling more amps than what the source is able to _safely_ provide? The BesTech BMS can recharge at 20A, so this must be a problem for many builders using standard power bricks.

@Namasaki I measured by putting a multimeter in series between the battery and charger positive lead, while the e-switch and power brick were on. Pretty surprising to see a 2A power supply deliver 5A.
```

---
## \#8 Posted by: DeathCookies Posted at: 2018-03-19T10:32:15.735Z Reads: 75

```
[quote="Bataleon, post:7, topic:49455"]
@deucesdown I was thinking the same. Pulling 180w from a small power brick seems dangerous. Million dollar question though: how do you prevent your BMS from pulling more amps than what the source is able to safely provide? The BesTech BMS can recharge at 20A, so this must be a problem for many builders using standard power bricks.
[/quote]

[quote="Acido, post:2, topic:49455"]
The bms wont amp up the current, it charges with what it gets, if a power brick is capable of 2a it will charge with 2a
[/quote]

Even if the bms demands 20amps, it wont pull it. It is just capable of charging at 20A if someone/sth Feeds it with that much power.


Maybe you get confused by batteries because everyone says: 
dont set the max amp from the vesc above the max continous amp of the battery.
--> thats a bit different because the battery could provide more than the continous but would burn after some time
a power supply cannot get more amp out of it or it will burn too (the components are not reated for so much amp). But you dont see burning brick chargers because they get mostly certified and have some protection that they dont supply the whole current of the wall outlet
```

---
## \#9 Posted by: Bataleon Posted at: 2018-03-19T10:37:55.056Z Reads: 68

```
[quote="DeathCookies, post:8, topic:49455"]
Even if the bms demands 20amps, it wont pull it. It is just capable of charging at 20A if someone/sth Feeds it with that much power.
[/quote]

I'm pretty sure that the current is determined by the load on the power source, not what the power source feeds it. In this case, the BMS wants 20A (its max charge rate) but the power supply is only able to deliver 5A, while at the same time getting super hot and almost burning up.

[This](https://www.banggood.com/AC-100V-240V-Converter-Adapter-DC-36V-2A-72W-Power-Supply-Charger-5_5mm-p-1158789.html?rmmds=search&cur_warehouse=CN) is the power brick I'm using. I doubt it has any safety certifications etc.
```

---
## \#10 Posted by: pat.speed Posted at: 2018-03-19T10:42:36.413Z Reads: 67

```
It could be because it is at the start of the charge cycle. As it continues to charge and gets closer to the eoc voltage the current decreases. 

Although it is weird that the power supply can give that much current, I know that my little 15v one shuts off if I pull more than 2.5 while using an imax b6
```

---
## \#11 Posted by: DeathCookies Posted at: 2018-03-19T10:42:39.089Z Reads: 67

```
[quote="Bataleon, post:9, topic:49455"]
I’m pretty sure that the current is determined by the load on the power source, not what the power source feeds it. In this case, the BMS wants 20A (its max charge rate) but the power supply is only able to deliver 5A, while at the same time getting super hot and almost burning up.
[/quote]

I agree partly.
The BMS cant just take 20A from the power brick. e.g. if you have a 1kw power supply which could deliver These 20A but was Setup to only deliver 10A it wont just magically Output 20A just because the BMS wants to.

(i like to compare it to a funnel with water. The power supply is before the funnel and the bms is after the funnel. the bms accepts the funnel to be 20amp wide but the power supply is only 5amp wide. you just cant squeeze that water into that 5amp wide funnel to magically increase it at the other end :D)


But maybe i am just wrong. If so i would like to get corrected!
```

---
## \#12 Posted by: deucesdown Posted at: 2018-03-19T11:50:57.639Z Reads: 61

```
Ah I missed a few details. In a lithium ion charging system, it is the charger job to limit/control current and voltage in a cc/cv profile. The charger is a power supply with a buitl in charge controller.

The BMS cannot "control" the charge. Its job is to cut off power if something is wrong, and usually, to balance the cells in the pack when the pack gets full.

What you have is just a plain old power supply? There is no charge controller in your system. The battery will demand basically infinite amps, and your PSU will try to supply it, going into overload. No bueno.
```

---
## \#13 Posted by: SimosMCmuffin Posted at: 2018-03-19T13:12:10.881Z Reads: 55

```
Your charger is just CV (constant voltage) capable, meaning it will try to always output it's specific voltage.

What you need is a CV/CC charger, which limits the current to a certain amount by lowering it's output voltage, if the load is "asking" for more then what it can supply.
```

---
## \#14 Posted by: Bataleon Posted at: 2018-03-19T14:30:57.066Z Reads: 55

```
@deucesdown @SimosMCmuffin So a regular constant-voltage power brick must _not_ be used with a BMS, it actually needs a special charger? I thought the BMS did the CC/CV switching (as the battery approaches 100% fully charged), just like a hobby charger does.

I'm surprised there isn't more talk of this on the forums. Here I was thinking everybody just uses a regular power supply at the correct voltage.
```

---
## \#15 Posted by: deucesdown Posted at: 2018-03-19T16:59:19.047Z Reads: 50

```
You got it now. The typical bms is not a cc/cv charge controller
```

---
## \#16 Posted by: Bataleon Posted at: 2018-03-19T17:51:48.286Z Reads: 49

```
Good to know, thanks for the info. Do you have a link to the charger which you use with your BMS? It'd be useful to get an idea what chargers are popular.
```

---
## \#17 Posted by: Deckoz Posted at: 2018-03-19T18:03:12.227Z Reads: 46

```
Power bricks put out the amps at full voltage. 

So on a 5a 42v brick..

42v 5a = 210w
210w/36v = 5.8a
210w/30 = 7a...

Etc power bricks are dumb and typically put out a set wattage. Unless they are constant current variable voltage. Which most are constant voltage variable amps.
```

---
## \#18 Posted by: deucesdown Posted at: 2018-03-19T22:33:01.822Z Reads: 39

```
Okay, there are lots of small details that are wrong. 36v PSU, and 10s? 10s is 4.2v * 10 = 42v.

If you use a 36v charger with a 10s BMS, you'll never trigger the balancing function of the bms.

You should be able to find a 10s (42v) 2a lithium ion charger on ebay/amazon/aliexpress, if you want cheap. or search the forum. sellers change all the time.
```

---
## \#19 Posted by: Bataleon Posted at: 2018-03-20T07:50:27.298Z Reads: 35

```
The pack is 10S LiFePO4 (mentioned in the first post) so fully charged it sits at ~36v.

My mistake was using a regular laptop-style power brick (instead of a special LiFePO4 charger), thinking that the BMS handled all the CC/CV switching etc, just like a regular hobby charger.

I'll see what chargers I can find online, thanks.
```

---
## \#20 Posted by: pat.speed Posted at: 2018-03-20T11:43:35.454Z Reads: 34

```
I think @Deckoz means when the pack isn’t fully charged. It will rest at 36v at storage charge and 30v when nearly fully drained
```

---
## \#21 Posted by: deucesdown Posted at: 2018-03-20T11:55:17.466Z Reads: 30

```
[quote="Bataleon, post:19, topic:49455"]
mentioned in the first post
[/quote]

Sorry bad reading skills :grin:
```

---
