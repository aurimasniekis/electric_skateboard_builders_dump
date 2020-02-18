# GT2B Mod Connection Issues Inside BLDC Tool

### Replies: 6 Views: 352

## \#1 Posted by: clistpdx Posted at: 2018-05-28T18:22:58.479Z Reads: 86

```
I'm having trouble getting a signal from my GT2B mod and I'm wondering if anyone has seen this particular quirk before?
I've previously been using a mini remote without any issues, but wanted to try the GT2B mod. So I bought the large GT2B remote and followed all the steps to install it into a mastercho enclosure. I then inserted a bind key into the receiver, turned on the VESC/board, held down bind key and turned on the remote. The blinking red light on receiver became a solid red light (that's great!). I powered everything off, pulled the bind key out, and attached the PPM cable to the receiver in channel 1 as seen here:
![gt2b2|690x460](upload://lBOujNLmxuaMpVFpgh0WhwhT7s3.jpg)

The controller shows that it's connected:
![gt2b1|690x460](upload://24pYffrl7zsF9UYyQTCoQMrfkJh.jpg)

Then, inside BLDC Tool>App Configuration>PPM I cannot get a signal/pulsewidth to change when I squeeze the remote trigger. **BLDC Tool shows a pulsewidth reading that hovers around 1.9 or 1.8 and if I keep it open for a while it very slowly decreases in ms.** But nothing changes when I squeeze the trigger:
![21 AM|690x363](upload://fj0x7TttqqjZAFVXYMkyrcOUP4X.png)

Does anyone see anything glaringly obvious about my configuration? Do I need to use a different channel on the receiver?
```

---
## \#2 Posted by: gaetjen Posted at: 2018-05-28T18:35:03.494Z Reads: 72

```
should be in channel two not in one, if I am not mistaken
```

---
## \#3 Posted by: DeathCookies Posted at: 2018-05-28T18:46:53.110Z Reads: 70

```
Jup.
channel 1 = steering
channel 2 = acceleration
channel 3 = lights, ...
```

---
## \#4 Posted by: clistpdx Posted at: 2018-05-28T22:10:26.513Z Reads: 60

```
Thank you, both! As I was typing this up I started to think maybe that was where I had gone wrong. I love that this forum allows me to dare to try something without being absolutely sure I know how, knowing that there's lots of smart people on here willing to lend their expertise :)
```

---
## \#5 Posted by: clistpdx Posted at: 2018-06-10T17:33:48.293Z Reads: 36

```
I'm continuing to have trouble getting my GT2B Mod controller to show any signal inside BLDC Tool, or even to register the slightest movement of the motor. I've got the receiver on channel 2 (that was my issues earlier) but I think when I filed down the PCB in order to fit the potentiometer into the case I may have broken a trace on one of the 3 leads. I will need to resolder one of the 3 wires to salvage this thing (I think). **Does anyone know which of the 3 wires (red, green, or brown) corresponds to the pin labled 'C' in my photo?:**
![gt2bPot|466x500](upload://atimbac312h56LRA9gedhriRKTT.jpg)
```

---
## \#6 Posted by: clistpdx Posted at: 2018-06-10T17:42:02.749Z Reads: 34

```
I just did a continuity test on my multimeter (should have thought about this before I posted) and discovered that **RED wire is A, GREEN wire is B, and BROWN wire is C**. In case someone needs this info in the future :)  and I did destroy the trace when I filed down the PCB too much. Should be an easy solder fix
```

---
