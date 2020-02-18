# How do I program the vesc for buttery smooth acceleration and braking

### Replies: 18 Views: 2811

## \#1 Posted by: GrecoMan Posted at: 2017-07-27T17:59:23.055Z Reads: 304

```
Hello, I just got done riding my neighbors benchwheel and fell in love with how smooth the braking/acceleration was.  It was so smooth that you could slam all the way in the brakes and it would bring you to a very, very smooth stop, I am trying to replicate that and the acceleration on my diy board. I want the acceleration to be smooth as in I can go full throttle from zero mph and not go flying off my board, kind of a foolproof mechanism. Any tips?
```

---
## \#2 Posted by: Hummie Posted at: 2017-07-27T18:22:44.628Z Reads: 301

```
Devin got kicked off the forum but has a simple
Formula for Motor an battery amps based on ur motor winding resistance and what continuous wattage u want.    He's on vedders forum and could ask there. Or there's akamaniacs software.  Or evohyax is going add Devins math to his software I think
```

---
## \#3 Posted by: evoheyax Posted at: 2017-07-27T18:31:02.590Z Reads: 291

```
Calculator is in the works. Should be a few hours tops.
```

---
## \#4 Posted by: Martinsp Posted at: 2017-07-27T18:32:45.618Z Reads: 288

```
I believe you can do that in @Ackmaniac firmware/bldc tool. :) hopefully he will see it and help you.
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-07-27T18:46:20.966Z Reads: 278

```
@evoheyax once you finish please put a link up in this topic, I am looking forward to smooth braking :slight_smile:

@Hummie thanks, does anyone know why Devin got kicked off?  I've seen his deleted reply on a couple other posts but am yet to come across one on the topic of him getting kicked off 

@Martinsp thanks for tagging him, hopefully he will link it on this topic
```

---
## \#6 Posted by: Martinsp Posted at: 2017-07-27T18:51:10.728Z Reads: 273

```
But as far as start from stop goes the smooth feeling can be achieved with sensors the same goes for smooth stop because the sensors operate in low RPM.
```

---
## \#7 Posted by: evoheyax Posted at: 2017-07-27T19:23:46.700Z Reads: 265

```
He was kicked off because he had an argument with Jason from enertion about a post. I he annoyed a lot of people with his "crazy" formulas. The reality is, I believe his formula here holds merit. What's really going to give you smooth acceleration and braking is an even wattage through out your curve. His formula aims to do just that, and I have to say, for me, it worked very well.
```

---
## \#9 Posted by: themegak Posted at: 2017-07-27T19:36:00.667Z Reads: 261

```
Interesting, do you have to use akamaniacs firmware for and tool for this ?  Have you applied this formula on an FOCBox ?
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-07-27T19:40:12.572Z Reads: 256

```
Devins theory is simply wrong. A even wattage doesn't result in a even acceleration. And current control and also Watt control takes automatically care of that. Because a even torgue (motor Amps) results in a even acceleration. 

And that is physics. 2000 watts at 50 km/h gives you a little acceleration and 2000 watts at stand still will mostly throw you off the board.

And Wind and Rolling resistance comes on top of that.
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-07-27T21:05:47.047Z Reads: 242

```
@Ackmaniac could you give me the link to your program and instructions on how to set it up right?
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-27T21:13:17.911Z Reads: 243

```
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#13 Posted by: Hummie Posted at: 2017-07-27T23:53:18.875Z Reads: 229

```
no theory.  you can program the vesc's motor amp and battery amp settings to have a consistent wattage output at all rpms.  that's what the formula does not try to have even acceleration but even power output.  

from the beginning it seemed everyone was taking enertions word for it, or maybe vedder's word, I don't know who but everyone was at 60/60.  that equates to huge power at higher speeds but low speed power was lacking.  People who want to simplify the power output to a given wattage at any rpm can use the formula when plugging in the motor and battery amps.

for me the low speed power with the highest motor amp settings was of course nice with the increased power and this is because of hub motors especially, and it also made cogging at low speeds much less.  can move from standstill.

i think the vess4.12 has a programed limit of 120motor amps regardless of higher input.  I think I remember that was the case.  hardware limit at 160 amps.  But can be increased with better bits and different code if you wanted to.  I think with hub motors this is more of a possible want than with a pulley on the motor
```

---
## \#14 Posted by: evoheyax Posted at: 2017-07-28T00:53:36.891Z Reads: 208

```
I'm starting realizing why the FOCBOX is actually useful. rated to a peak 300A, I wouldn't be limited like I am now with the CARVON v2's. I didn't have this issue with hummies motors because the kv was way lower (and resistance was higher).

I'm putting the final touches on the calculator now.
```

---
## \#15 Posted by: Jinra Posted at: 2017-07-28T00:58:11.577Z Reads: 199

```
I don't think you should be aiming to pull anywhere near 300A, especially with 4 VESCs. If you're pulling that many amps, your range is going to suffer
```

---
## \#16 Posted by: evoheyax Posted at: 2017-07-28T02:03:43.348Z Reads: 192

```
I don't want 300A, but I could see now how in certain cases, like with really high kv motors, there's a benifit in being able to peak higher than 120 motor amps.
```

---
## \#17 Posted by: lrdesigns Posted at: 2017-07-28T02:56:36.817Z Reads: 194

```
[quote="GrecoMan, post:11, topic:28793"]
@Ackmaniac
[/quote]

I highly recommend Ackmainiac's firmware it will give much smoother than the standard. 

Other things you can try is to reduce the battery amps + and -  Use sensored motors helps a lot but you probably need new motors for that if they dont have already. 

I also found if you bump up you gear ratio a bit you will get smoother power delivery but slightly less brake power and a bit more top speed, at the expense of more load on you motors. So I wouldn't do that if they already get hot.
```

---
## \#18 Posted by: landonkun Posted at: 2017-07-28T04:42:36.683Z Reads: 184

```
Interested in your calculator. Keep us posted :slight_smile:
```

---
## \#19 Posted by: evoheyax Posted at: 2017-07-29T04:56:06.416Z Reads: 162

```
Here's the [calculator](http://www.vescstatus.com/setcalc). Enjoy!
```

---
