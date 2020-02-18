# Changing the Cruise control button from &ldquo;C&rdquo; to &ldquo;Z&rdquo; on my Kama nunchuck?

### Replies: 17 Views: 1640

## \#1 Posted by: UniqueSnowflakeN27 Posted at: 2016-12-12T19:51:00.779Z Reads: 89

```
**I did it!**

It was unbelievably easy. I just removed the 2 screws held the shell together, then the 2 screws that held to main PCB-board to the shell. Then I just had to flip small PCB-board behind the "C" and "Z" switches upside down. 

The whole process took about 3 minutes. I recommend it to everyone who's using a Kama nunchuck, it feels more much more comfortable.

___________________________________________

I could of course desolder the buttons and switch them around inside, but I'm hoping there's an option in BLDC Tool instead. I'm using a VESC.

So is it possible to change the cruise control from the "C" button to the "Z" button using BLDC Tool? Sorry if this has been asked before, but I searched and couldn't find any other threads about it.

Cheers
```

---
## \#2 Posted by: rpn314 Posted at: 2016-12-13T18:23:50.733Z Reads: 65

```
Nothing in BLDC tool at the moment, but changing it in the firmware is quite easy.
```

---
## \#3 Posted by: UniqueSnowflakeN27 Posted at: 2016-12-14T23:11:09.837Z Reads: 57

```
The hardware modification was easy enough. I didn't know you could program the firmware for the nunchuck!
```

---
## \#4 Posted by: lowGuido Posted at: 2016-12-14T23:23:26.200Z Reads: 53

```
I was going to say.. 
Wouldn't you just re program the firmware?
Anyways what works works.
```

---
## \#5 Posted by: rpn314 Posted at: 2016-12-14T23:23:43.955Z Reads: 53

```
Well, sort of. You can do it in the firmware of the VESC itself or in the firmware of the nunchuck itself if you have one of the custom nunchucks (usually referred to as nunchuckRF or nrf around here). I'm not aware of how to modify the firmware of pre-made nunchucks (like the Kama)
```

---
## \#6 Posted by: Ackmaniac Posted at: 2016-12-15T01:57:11.472Z Reads: 48

```
In the firmware of the vesc the behavior of the buttons simply could be switched for the buttons. But is it that much better when those buttons are switched around? Never had a nunchuk.
```

---
## \#7 Posted by: rpn314 Posted at: 2016-12-15T19:37:03.585Z Reads: 45

```
I'm not sure it's better or worse, more of just a personal preference thing. But just looking at the nunchuck, the Z button is MUCH larger than the C button, so making the bigger button the one that you'd want to press (and hold) more often makes sense to me. To be honest, I'm not sure why Vedder set it up the way it is, but it's not usually a huge deal (and again, just a personal preference)
```

---
## \#8 Posted by: kyo Posted at: 2016-12-18T03:58:58.665Z Reads: 37

```
Hi @UniqueSnowflakeN27
How did you flip that button pcb upside down? I could not do it because the wires are in the way and the pcb is held by 4 plastic teeth. The only way to get it out is slide it out but the wires are in the way.
Did you break these teeth?
```

---
## \#9 Posted by: UniqueSnowflakeN27 Posted at: 2016-12-18T13:10:24.389Z Reads: 37

```
I opened it up again and took some photos. The grey "contact pads" are easy to just pull off, then the pcb-board can come off. You have to bend the white plastic plate holding it in place a bit since the pcb-board won't slide out because of the flat cable coming out of the back.

Once the pcb-board is loose you have to play around with the flat cable and twist it so that you can put the pcb-board back.

Hope this helps!


<img src="/uploads/db1493/original/3X/f/5/f50d8f4a698f369838b7c139ad35156b60dc88a4.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/b/f/bfe838b79afe43319984f042cb0d269195c64e1a.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/8/7/872aabcbe256453f85e26751742552cab9a494b4.jpg" width="690" height="460">
```

---
## \#10 Posted by: kyo Posted at: 2016-12-18T13:49:30.692Z Reads: 35

```
Gee thanks much bro. I did it. It is more comfy forthe finger. But somehow i felt it a bit weird to press it. I mean the bouncing , anyway it works fine now. Thanks again
```

---
## \#11 Posted by: kyo Posted at: 2016-12-18T13:51:56.775Z Reads: 35

```
And by the way, i also added a switch to it 

<img src="/uploads/db1493/original/3X/6/2/620ee4569a15921cef505736e9bd9353911545fe.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/f/b/fb4980ed5117ee40ef4a4a380bfc01aa036a42be.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/d/1/d19c714e78b2729020ec1780dea8302314a77b7c.JPG" width="375" height="500">
```

---
## \#12 Posted by: UniqueSnowflakeN27 Posted at: 2016-12-18T14:30:31.020Z Reads: 31

```
Nice! Is the switch meant to help preserve battery life?
```

---
## \#13 Posted by: kyo Posted at: 2016-12-18T17:06:40.295Z Reads: 30

```
So i dont accidentially send my board to fly when i stop for a bit
```

---
## \#14 Posted by: Maxid Posted at: 2016-12-18T17:11:15.223Z Reads: 31

```
how will that work? the timer is probably programmed into the controller chip - a switch won't change that. Or do you mean it's to shut it off so you don't accidentally move it when touching the thumb stick?
```

---
## \#15 Posted by: UniqueSnowflakeN27 Posted at: 2016-12-18T17:18:12.065Z Reads: 29

```
Looks like the switch is wired to either the negative or the positive of the battery, so the timer doesn't matter. 

Seems like a pretty good setup to me.
```

---
## \#16 Posted by: kyo Posted at: 2016-12-19T02:20:37.267Z Reads: 31

```
yes, that is the case.
```

---
## \#17 Posted by: Maxid Posted at: 2017-04-12T08:10:30.090Z Reads: 20

```
https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286

With @Ackmaniac's firmware you can now switch the C and Z buttons around in the BLDC tool!
```

---
