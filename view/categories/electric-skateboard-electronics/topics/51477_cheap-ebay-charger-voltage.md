# Cheap Ebay Charger Voltage?

### Replies: 34 Views: 954

## \#1 Posted by: TrainRider Posted at: 2018-04-07T12:29:21.584Z Reads: 116

```
I've just completed my first build using a bestech 10s BMS and everything is working well apart from the board won't charge.

I checked all my connections and everything is correct apart from the voltage output from the charger.

I bought the charger from ebay (no longer listed), which was sold as a 42v 2A balance board/segway charger and that's what it says on the charger itself but I measured it as 24v? Is this expected from a charger or did I get ripped off?

Thanks
```

---
## \#2 Posted by: Acido Posted at: 2018-04-07T12:42:03.885Z Reads: 109

```
Do the electronics turn on?
Whats the battery voltage?
```

---
## \#3 Posted by: TrainRider Posted at: 2018-04-07T12:43:55.119Z Reads: 106

```
Electronics turn on, motors spin. Battery voltage is ~32v
```

---
## \#4 Posted by: Acido Posted at: 2018-04-07T12:47:25.044Z Reads: 104

```
Then you got ripped off, just tell eBay not as advertised / you did not receive it
```

---
## \#5 Posted by: TrainRider Posted at: 2018-04-07T12:51:24.166Z Reads: 95

```
Thanks for confirming that, very frustrating! I was hoping to go for my first ride today.
```

---
## \#6 Posted by: Acido Posted at: 2018-04-07T12:52:29.549Z Reads: 94

```
One more thing, try charging with the bms on if it does not work try with it turned off

I did not try this new model so do not know...
```

---
## \#7 Posted by: TrainRider Posted at: 2018-04-07T13:02:35.015Z Reads: 87

```
I have given it a go, there is no connection when it is turned off and I have been trying with on. Will have to see if I can source a charger locally today.
```

---
## \#8 Posted by: Namasaki Posted at: 2018-04-07T13:09:32.660Z Reads: 85

```
[quote="Acido, post:6, topic:51477"]
One more thing, try charging with the bms on if it does not work try with it turned off
[/quote]

It is standard with Bestech bms that have a built in E-switch that the switch must be on when charging. 

@TrainRider
If your charger is not outputting 42v then it is defective or mislabeled.
```

---
## \#9 Posted by: TrainRider Posted at: 2018-04-08T10:25:51.426Z Reads: 66

```
Okay, so I got a new charger, 42v 2A. Plugged everything in it charged for about 5 seconds then popped a capacitor... Tripled checked my wiring everything looks correct. I'm at a loss to know what do to.
```

---
## \#10 Posted by: Tuomalar Posted at: 2018-04-08T10:54:23.140Z Reads: 65

```
Post a picture of your wiring.
```

---
## \#11 Posted by: TrainRider Posted at: 2018-04-08T11:23:47.287Z Reads: 64

```
Sorry for the paint. Let me know if this isn't clear:
![20180408_120032-mod|666x500](upload://hythKIhPhp4zOSDqneu23ZhzFUJ.jpg)

Here is the wiring diagram I'm working from:

![HCX-D596---wiring-diagram|690x478](upload://iepEHEYiFz1eXr4glC6ihROngWN.jpg)
```

---
## \#12 Posted by: Tuomalar Posted at: 2018-04-08T12:28:57.227Z Reads: 57

```
That wiring is so messy that it’s giving hard times to see what goes where. Can u post better pic from batteries? Those look kinda weird to me.
```

---
## \#13 Posted by: TrainRider Posted at: 2018-04-08T12:38:49.002Z Reads: 57

```
I know that the batteries work and are wired correctly as they have the right voltage and I have had the motors spinning. I didn't post the battery pack as the wires are the wrong colors and I didn't want to cause confusion, black is positive and red negative but here it is anyway:

![20180408_133603|666x500](upload://3BGescfjWtg3gnn0MgAZyUHF11x.jpg)
```

---
## \#14 Posted by: TrainRider Posted at: 2018-04-08T12:43:41.281Z Reads: 55

```
Balance leads are reading correctly between BMS negative terminal and the end of the balance lead. I have labelled on the first picture in which order they are wired and where the first and last leads are connected.
```

---
## \#15 Posted by: Namasaki Posted at: 2018-04-08T13:48:07.830Z Reads: 52

```
Where did you buy both chargers?
```

---
## \#16 Posted by: TrainRider Posted at: 2018-04-08T13:52:07.684Z Reads: 52

```
First charger was from ebay, no longer listed. Second one was [this one](https://www.amazon.co.uk/gp/product/B071FQGB1H/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1)
```

---
## \#17 Posted by: moon Posted at: 2018-04-08T13:54:52.391Z Reads: 53

```
Does the second one not work either?
```

---
## \#18 Posted by: TrainRider Posted at: 2018-04-08T13:56:12.293Z Reads: 49

```
Plugged it in, 5 seconds later it popped a capacitor.
```

---
## \#19 Posted by: moon Posted at: 2018-04-08T13:56:30.386Z Reads: 49

```
Return it, thats not your fault
```

---
## \#20 Posted by: TrainRider Posted at: 2018-04-08T13:58:50.986Z Reads: 49

```
I'm 3 chargers in at this point, I have to be doing something wrong.
```

---
## \#21 Posted by: moon Posted at: 2018-04-08T14:00:07.952Z Reads: 49

```
Oh I have not realised this. I hope theres someone that can help
```

---
## \#22 Posted by: TrainRider Posted at: 2018-04-08T14:00:15.651Z Reads: 50

```
![20180408_145755|375x500](upload://c9Ia6goFJryNGj4qDrxCEnE0F2J.jpg)
```

---
## \#23 Posted by: TrainRider Posted at: 2018-04-08T14:33:00.010Z Reads: 49

```
Do you think I should try another charger?
```

---
## \#24 Posted by: Namasaki Posted at: 2018-04-08T15:43:02.503Z Reads: 47

```
If your wiring was incorrect, it would smoke the bms as soon as you connected it and turned it on.
And btw, are you turning the bms on to charge?
If not, then that’s your problem. 
I new of another member who burned up his charger by trying to charge with a Bestech bms while it was off. 
Any Bestech bms with a built in E-switch MUST be turned on while charging. 

If this scenario does not apply to you, then I would guess that you are just having bad luck with chargers
```

---
## \#25 Posted by: TrainRider Posted at: 2018-04-08T16:27:00.946Z Reads: 41

```
I've done as thorough a visual inspection I can without desoldering the two boards from each other on the BMS, as far as I can see everything looks good.

BMS has been on while I've been charging, I've been plugging everything in, turning on the BMS and then turning on the charger.

I will try one more charger.

Thank you for advice on this, much appreciated.
```

---
## \#26 Posted by: TrainRider Posted at: 2018-04-10T18:50:55.274Z Reads: 34

```
so uhh, turns out I had the polarity on the charge port reversed... quite embarrassing.
```

---
## \#27 Posted by: onepunchboard Posted at: 2018-04-10T19:08:03.976Z Reads: 36

```
lucky u didnt pop bms like i did.
```

---
## \#28 Posted by: TrainRider Posted at: 2018-04-10T19:12:48.610Z Reads: 38

```
Man that must really suck. I've already wasted so much money on chargers i'm really hoping my BMS is alright, if not this would be a very expensive mistake.
```

---
## \#29 Posted by: GAsplund Posted at: 2018-04-10T19:20:18.424Z Reads: 35

```
If you keep getting faulty chargers, I don't blame you since the seller probably did something wrong. Anyway - I purchased my 10S charger som SuPower Battery/Batterysupports and they tolerated even charging when my friend charged his with his BMS wired in reverse. (It's fixed now)

Anyway, they have a 2A and a 5A charger for about double the price of the ones you bought.

2A:
http://www.batterysupports.com/liion-lipo-42v-for-36v-37v-10s-2a-wall-socket-battery-charger-p-364.html

5A:
http://www.batterysupports.com/36v-42v-5a-lithium-ion-battery-charger-10s-10x-36v-lion-lipo-p-166.html
```

---
## \#30 Posted by: TrainRider Posted at: 2018-04-10T19:26:43.854Z Reads: 33

```
Thanks for the recommendation, I will definitely get one of those next time!
```

---
## \#31 Posted by: moon Posted at: 2018-04-10T19:27:27.631Z Reads: 30

```
Are you looking for a charger? I am in the UK and I will sell one to you if needed
```

---
## \#32 Posted by: TrainRider Posted at: 2018-04-10T19:28:52.501Z Reads: 30

```
I've already primed a new one to me. Should arrive tomorrow, thanks for the offer though :).
```

---
## \#33 Posted by: moon Posted at: 2018-04-10T19:29:17.432Z Reads: 29

```
Ok no problem. I wish you luck!
```

---
## \#34 Posted by: Bataleon Posted at: 2018-05-11T12:58:04.176Z Reads: 19

```
Just a heads-up: even though the Amazon link above is described as a "42V 2A PowerFast Charger", it's actually just a normal 2A 42V power brick. It has no CC/CV functionality which is needed when charging li-ion cells. I made this exact mistake a few months ago.
```

---
