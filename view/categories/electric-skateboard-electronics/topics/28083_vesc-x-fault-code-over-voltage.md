# Vesc-x fault_code_over_voltage

### Replies: 9 Views: 795

## \#1 Posted by: Eboosted Posted at: 2017-07-20T05:27:10.725Z Reads: 143

```
Guys, I started to have this issue today, the board cutted out several times leaving me with no brakes or throttle.

The cause of the fault was over voltage, however, during the cutoff, the voltage was perfectly normal at 47.5V. I'm runing 12S battery and two FocBoxes.

These are my VESC settings:

motor min	65.0 A
motor min	-65.0 A
battery max	40.0 A
battery min	-8.0 A
cutoff start	36.0 V
cutoff end	33.6 V

Would you please take a look at my log?

The red bars are the time the VESCs went offline.

<img src="/uploads/db1493/original/3X/0/d/0de0f97694e93b8ce8a268e5d9c4ee126f0a4b75.png" width="497" height="499">
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-07-20T06:57:56.526Z Reads: 130

```
Both Vescs cut off? 
Do you have the full fault code?
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-07-20T08:32:09.646Z Reads: 129

```
Whats your Maximum Input voltage in the settings?
```

---
## \#4 Posted by: Eboosted Posted at: 2017-07-21T04:40:14.107Z Reads: 102

```
Guys I disassembled the board today to check for visible problems and I found the culprit. 

<img src="/uploads/db1493/original/3X/f/4/f41eb6b1c19334f0cace115463901fff0b77787d.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/c/8/c8b42401acf6135d8999cd3aa90b21087577bb74.jpg" width="666" height="500">

So, one more thing learned today: whenever you have FAULT CODE OVER Voltage, your VESCs start to reboot and you loose brakes or throttle for 3 seconds, then you have a broken nickel strip or bad connection between packs. 

When I first build the battery pack, I used flat braided cable in order to have a flexible pack, this is really a bad idea, those will break with time or a flexible deck, no matter what, at that time I added a 14awg wire to increase the flow of current between the packs and after today's inspection I realized none of them were broken, so today I decided to remove the flat wire and add a second 14awg wire between packs, this is going to hold much better keeping the flexiness of the battery pack. 

<img src="/uploads/db1493/original/3X/3/f/3f0f1f9621a0a15b0e663900cfb6a5525a65a68e.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/4/2/42d486a6052c918e5323cbe4f87ed7f09a2a04fa.jpg" width="374" height="500">

Board is back on the track, riding like a dream no more cutouts or reboots!
```

---
## \#5 Posted by: Blasto Posted at: 2017-07-21T05:06:59.146Z Reads: 90

```
What was the original flat braided wire did you use for the series connections?
```

---
## \#6 Posted by: Jinra Posted at: 2017-07-21T05:54:19.696Z Reads: 89

```
Maybe use a flat buss bar instead of cable between the groups
```

---
## \#7 Posted by: Eboosted Posted at: 2017-07-21T06:17:32.262Z Reads: 85

```
I got them from Kaly with the enclosure
```

---
## \#8 Posted by: Eboosted Posted at: 2017-07-21T06:19:37.487Z Reads: 85

```
You mean copper stops instead of nickel?
```

---
## \#9 Posted by: Jinra Posted at: 2017-07-21T06:25:44.093Z Reads: 83

```
like this

http://m.ebay.com/itm/K-S-Brass-Strip-016x1-2-8231-/282515605117?hash=item41c73e067d%3Ag%3A5dwAAOSw~rpZOWXO&_trkparms=pageci%253A47e48ca7-6ddd-11e7-be0f-74dbd180f6f6%257Cparentrq%253A63d1d3ad15d0a7e0725cc555fffd9359%257Ciid%253A6
```

---
