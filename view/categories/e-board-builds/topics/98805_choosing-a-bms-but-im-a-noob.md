# Choosing a BMS but im a noob

### Replies: 14 Views: 382

## \#1 Posted by: shark78921 Posted at: 2019-07-20T18:55:55.901Z Reads: 115

```
Hey guys, im nearing the end of my second build and one of the final touches is a BMS. i've been in contact with bestech and im not 100% sure the one the sales assistant suggests is the right one i need 

I have 2 12C 6S lipo batteries in series to make a 12S battery powering each motor.  https://tinyurl.com/yy8fwqpe

this is the info they gave me, i know i can bypass when discharging but i was concerned about charging, will this do?

my first time dealing with a bms so i appreciate the help

![Screenshot_20190720-194926_Word%201|57x500](upload://xUNepX5faxQy63U4FACEr6ABHwn.jpeg) ![Screenshot_20190720-194926_Word|85x500](upload://93pp4NPK4uIGdgm643YlrpAWxQu.jpeg)
```

---
## \#2 Posted by: janpom Posted at: 2019-07-20T19:14:18.219Z Reads: 101

```
It looks like it can handle 60A+ charge current, which is a complete overkill. It's pretty bulky. How much is the price? You would likely be better off getting the DieBieMS.
```

---
## \#3 Posted by: shark78921 Posted at: 2019-07-20T20:05:06.119Z Reads: 98

```
they keep dodging the price everytime i ask so i don't know atm, should i ask for a lower amped bms, when i emailed them i said the max amps the batteries can draw was 150, is 60 enough? thats the max my vesc can handle, but if im bypassing when discharging does it even matter?
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-07-20T20:23:16.382Z Reads: 89

```
Your battery is rated for 12s 79.2A
```

---
## \#5 Posted by: shark78921 Posted at: 2019-07-20T21:28:59.208Z Reads: 76

```
oh okay, so a 80A bms should be fine? thanks again btw
```

---
## \#6 Posted by: glyphiks Posted at: 2019-07-20T22:46:03.456Z Reads: 73

```
I think I've read that bestech won't sell a single BMS, they only sell in groups of two? I may be wrong.
```

---
## \#7 Posted by: janpom Posted at: 2019-07-20T23:21:21.924Z Reads: 70

```
What you have linked looks like a pretty advanced and beefy BMS. I suppose the price will be well above $200. It's an overkill.

Are you looking for a smart BMS? If yes, DieBieMS is likely a better options since it fits the esk8 ecosystem. It can communicate with VESCs and if you get the Metr module, you can get the BMS data on your mobile phone. At $120 shipped it's probably also a lot cheaper.

If you don't want/need a smart BMS, you have a number of cheaper and more compact options, especially if you're OK with bypassing discharge. In that case Bestech D140 is pretty popular.

In general, you're looking for something rated 10A+ for charge and 60A+ for discharge. If you bypass discharge, then obviously discharge rating is irrelevant.
```

---
## \#8 Posted by: shark78921 Posted at: 2019-07-20T23:29:45.617Z Reads: 65

```
That's okay, I'm after 2
```

---
## \#9 Posted by: shark78921 Posted at: 2019-07-20T23:32:03.400Z Reads: 67

```
Pretty much bang on, the one thing I haven't really understood is the communication protocol/smart bms, in this case with the vesc Like what would it be for?
```

---
## \#10 Posted by: janpom Posted at: 2019-07-21T07:30:19.599Z Reads: 64

```
Here's an example:

https://giphy.com/gifs/3OC2r75I9xp9M2hdxa

The most important feature of a smart BMS is that it can communicate individual cell voltages to other systems.

This can be done in various ways. You can read more about it here: https://www.electric-skateboard.builders/t/monitoring-individual-cell-voltages/80340

The DieBieMS, in particular, connects to VESC via CAN. The VESC itself is not programmed to make any use of the DieBieMS data but it can forward the info to other devices that connect to the VESC, such as the Metr module.
```

---
## \#11 Posted by: shark78921 Posted at: 2019-07-21T17:51:03.693Z Reads: 53

```
oh alright, i thing i get it better now. where would i get the DieBieMS, bestec or is it off someone in the forum?
appreciate it btw
```

---
## \#12 Posted by: janpom Posted at: 2019-07-21T23:11:12.426Z Reads: 48

```
@Samau18 makes them. He might still have some from the last batch.
```

---
## \#14 Posted by: janpom Posted at: 2019-07-22T08:15:23.152Z Reads: 40

```
140 x 60 mm (it takes 10 secs to find on the forum using search, BTW)
```

---
## \#15 Posted by: ShutterShock Posted at: 2019-07-22T16:03:53.511Z Reads: 33

```
The DieBie is good, very advanced and such but the PCB is quite bulky, if you want a less smart one, I suggest SuPower @ batterysupports.com

BesTech does also have less smart ones like others have mentioned, I think they were trying to upsell you depending on what you said your requirements were

I have used those BMS's in 4 builds now and they work wonderfully for a pretty fair price, much lower than the DieBie
```

---
