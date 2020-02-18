# Maytech Vesc blue light only

### Replies: 13 Views: 931

## \#1 Posted by: MontPierre Posted at: 2017-08-03T13:02:02.891Z Reads: 97

```
I have just finished my board with 10s lipos ( 30amps 40 max 8000mah Zippy).

I'm using moded firmware from @Ackmaniac. I have adjusted the watt mode to 300. Went for a ride. All good but not a lot of power. Then changed it to 700 and my board after 2 seconds stopped responding. 

Fuse is fine( vedder anti spark) but when I connect it to bldc tool there is no connection. Tried also re flashing boot loader but also no connection. I only get blue ligh let and the led next to it is red but very dim... nothing is flashing on startup as before. Have I burned my vesc ?

No signs of any burning on vesc.

<img src="/uploads/db1493/original/3X/e/0/e0735beaf416cc8cfe8359d80fc543db498d4524.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/f/9/f9860a60baf765b3e930393258bcbe3cef039e87.JPG" width="666" height="500">
```

---
## \#2 Posted by: MontPierre Posted at: 2017-08-07T22:51:37.281Z Reads: 74

```
10char bump
```

---
## \#3 Posted by: rpn314 Posted at: 2017-08-07T23:46:21.215Z Reads: 70

```
How exactly did you flash the bootloader? And what messages did it give you during the flashing?
```

---
## \#4 Posted by: MontPierre Posted at: 2017-08-07T23:51:02.685Z Reads: 70

```
Flashing went fine, no errors and was using for a day moded bldc tool. I just had a chat with @Martinsp and after probing vesc with multimeter it looks like CAN chip is fried as my 3.3V line is shortened. Anyone in UK who fixes Vescs? Or at least can change a chip? My soldering is bad AF ;)
```

---
## \#5 Posted by: rpn314 Posted at: 2017-08-07T23:53:30.712Z Reads: 69

```
Oh, well glad you figured it out! I am curious, how do you know it's the CAN module that's shorting the 3.3 line (versus something else)?
```

---
## \#6 Posted by: MontPierre Posted at: 2017-08-07T23:55:36.672Z Reads: 67

```
That's his diagnosis- he had few of those on his repair table before ;) well it isint 100% but at least I'm getting somewhere;)
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-08-08T00:08:37.553Z Reads: 64

```
The CAN transceiver only has 6 pins, its much easier than swapping a DRV. And its only a few bucks. If you get desparate give it a wack yourself. I can usually get away without adding any additional solder or flux when changing those.
```

---
## \#8 Posted by: cliofreak Posted at: 2018-02-26T14:10:37.354Z Reads: 47

```
Hi, any more info on this senario? 
Mine is now intermittent. Blue light on VESC when I opened up enclosure then no connection with Vesc Tool.
Then randomly light changed to normal and remote worked.

So, now I have to turn the vesc on and off about 15 times for it to work correctly. What would cause this!!?![IMG_0195|666x500](upload://gMPCJSZp1OBfF23amHw3YItdixi.jpg)![IMG_0196|375x500](upload://mmblGkPkraMxtpRAuNFmXMvyWmk.jpg)
```

---
## \#9 Posted by: RedEagle Posted at: 2018-02-26T14:22:35.896Z Reads: 39

```
No bootloader or wrong firmware? Something could also be shorted.
```

---
## \#10 Posted by: cliofreak Posted at: 2018-02-26T14:23:10.727Z Reads: 40

```
It was working fine then randomly its started doing this.
```

---
## \#11 Posted by: RedEagle Posted at: 2018-02-26T14:28:27.389Z Reads: 37

```
Did you flash the bootloader or update the firmware? Where did you get the vesc from? I suspect this is a hardware related issue not a software related one.
```

---
## \#12 Posted by: cliofreak Posted at: 2018-02-26T14:33:53.764Z Reads: 39

```
Nah, I changed some parameters within the Vesc Tool (I was playing it safe before so was advised on here to change some parameters). I then too a ride for a few miles and it was pulling great and totally fine. Then next day, turned it on an nothing. Then I opened it up and took pics. The turned of and on a few times to try to connect to vesc tool and failed. Then randomly started working. Rode it for a further 8 miles totally fine. Now it takes 10-15 goes at powering on.

I got Vesc from eskate.eu in Italy.

Im in uk
```

---
## \#13 Posted by: RedEagle Posted at: 2018-02-26T14:36:42.407Z Reads: 35

```
I think it would be wise to start your own thread about this. This looks like a hardware issue. Start by measuring with the multimeter and go from there.
```

---
