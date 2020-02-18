# Dual Vesc question

### Replies: 13 Views: 1784

## \#1 Posted by: Namasaki Posted at: 2016-07-25T03:03:14.241Z Reads: 153

```
With a 9ah battery and dual vesc/motors, the most regen current that I want going to the battery
is 10a. So do I set the battery regen minimum on each vesc to -5 ?
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-25T04:02:40.848Z Reads: 140

```
Yep. Since I have a 4p setup with Samsung 25Rs (4A max charge current) I set my two  VESCs for -8A battery regen each.
```

---
## \#3 Posted by: Namasaki Posted at: 2016-07-25T05:25:11.104Z Reads: 131

```
Setting each Vesc to -8. Wouldn't that give you a total of 16 amps regen charge?
Each Vesc supplying 8amps?
```

---
## \#4 Posted by: Jinra Posted at: 2016-07-25T05:25:48.912Z Reads: 124

```
Yep, that's what I want. 4P x 4A = 16A
```

---
## \#5 Posted by: Namasaki Posted at: 2016-07-25T05:28:23.033Z Reads: 117

```
Ok I see.👍👍👍👍
```

---
## \#6 Posted by: Namasaki Posted at: 2016-07-25T05:31:24.855Z Reads: 107

```
So my pack is 10s2p with 4500mah cells
So I was thinking 1c @ 9ah  and round up to 10a
or -5 per Vesc. 
Is it safe for the battery to go 2c for regen charge?
I don't want to eliminate the brakes too much.
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-25T05:36:23.743Z Reads: 106

```
I did some searching and it looks like your Basen's handle a max charge current of 5.2A. You should be fine for -5A each VESC

source: http://www.electronic-cigarettesco.co.uk/26650-batteries/509-basen-26650-4500mah-60a-high-drain-battery.html
```

---
## \#8 Posted by: Namasaki Posted at: 2016-07-25T05:41:44.052Z Reads: 105

```
Cool, thanks for the help and thanks for the link. 
I searched but could not find Dara on charge current.
```

---
## \#9 Posted by: Skitzor Posted at: 2016-07-26T11:15:50.070Z Reads: 81

```
What's your opinion on the regen for a Space cell 3 ? default was at -80. I've burned a drv at the moment while one wheel was braking. could this be related?
```

---
## \#10 Posted by: Namasaki Posted at: 2016-07-26T15:43:57.393Z Reads: 79

```
I'm no expert with the Vesc but from what I've read, 
There are 2 settings
Motor Regen controls the amount of braking
Battery Regen controls the current going back to the battery. 
Find out the recommended charge rate for SC3
and set the battery Regen to match. 
I think most people are running -60 for motor Regen
```

---
## \#11 Posted by: Namasaki Posted at: 2016-07-26T15:46:47.999Z Reads: 78

```
The burned DRV:
Sounds like a possible short in the motor.
```

---
## \#12 Posted by: Skitzor Posted at: 2016-07-26T19:09:07.959Z Reads: 71

```
True, but had multiple shorts already. Last one burned the DRV. I thought that would be better protected by the vesc.

Edit and let me rephrase my question:
Whats the difference between battery regen and motor regen.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-07-26T20:07:47.822Z Reads: 70

```
I could be wrong, but the way I understand it, 
The motor Regen current regulates the amount of brake force. 
The battery Regen current regulates the charge going back into the battery while braking. 
There is a thread that explains it better:
http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
```

---
