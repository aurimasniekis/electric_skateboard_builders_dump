# Can I convert my board to a DUAL motor setup?

### Replies: 10 Views: 1170

## \#1 Posted by: kevin.pritchard Posted at: 2016-10-04T10:20:56.822Z Reads: 164

```
Hi.

I have an I-Wonder SK-A2. I also have a spare stock motor and spare stock ESC.

Could I, in theory, connect this spare motor and ESC to achieve a dual (diagonal) motor setup by wiring a Y-splitter to the radio receiver and battery?

I'm not that great with voltages and loads etc, but can do the soldering and wiring. Battery is rated 8.8Ah 24V.

Any help would be much appreciated.
```

---
## \#2 Posted by: rpn314 Posted at: 2016-10-05T20:39:38.063Z Reads: 108

```
Theoretically, most likely.
I've never seen one of those boards, so I'm not sure what kind of extra space there is inside, nor am i familiar enough with the setup of the speed controller to know how it's connected to the radio, but I would imagine so. In general the second motor only makes it use a little bit more power, but each motor does less work to move the same amount and so I don't think you'd have any issues, as long as the battery is protected enough from over current (which it should be already...)

TLDR: You'll probably be okay in terms of how much the battery can handle, as long as it's protected. I think space in the enclosure will be a bigger issue
```

---
## \#3 Posted by: kevin.pritchard Posted at: 2016-10-06T08:44:53.459Z Reads: 85

```
Ooh, that sounds promising! :slight_smile:

I'll try and get some internal photos uploaded soon. When I briefly looked last time, it appeared that the radio PCB was separate to the ESC.

So, in practice, the extra motor should give better, say - hill climbing?

What would be the signs of a 'protected' battery?
```

---
## \#4 Posted by: rpn314 Posted at: 2016-10-06T16:18:31.231Z Reads: 71

```
Yeah, an extra motor will give you better hill climbing and torque (feels "jumpier")

Generally a BMS will take care of the protection part. That will look like a circuit board with a bunch of wires running to inside of the battery, known as balance wires, and then you charge with a single plug in jack (without the whole balance thing to the outside).
```

---
## \#5 Posted by: kevin.pritchard Posted at: 2016-10-07T07:12:41.132Z Reads: 62

```
Here are some photos of the ESC. I'm not 100% sure, but is the board that's 'upside down' the RF transmitter? If so, instead of trying to connect it to both ESCs, could I just leave the RF transmitter on both ESCs and have them both pair with the remote?

Anyway, I hope these photos help in determining whether my plan would work.

Thanks again. Getting a bit excited :slight_smile: 

<img src="/uploads/db1493/original/3X/e/0/e031d913f4e1f8b065ce6076687932616cb205b4.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/9/099bce8c55c7b70932204bca61d8a1caecbbdd07.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/7/3/7305299c2d31bd886bfd52bbd62b714247dbfc28.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/d/a/da3b8bf5816ef6c2af59de4fa71c9c1dfb5241aa.JPG" width="666" height="500">
```

---
## \#6 Posted by: kevin.pritchard Posted at: 2016-10-09T14:02:23.417Z Reads: 54

```
I've wired it all up and but ive only just realised i cant reverse the motor on a sensored motor by switching the wires!

What's my next best option? Scrap the ESCs for two VESCs?
```

---
## \#7 Posted by: kevin.pritchard Posted at: 2016-10-09T14:45:01.159Z Reads: 50

```
Just figured out a solution!! Reversed the red and black on both the 3-phase and thr hall sensor! So happy!
```

---
## \#8 Posted by: kevin.pritchard Posted at: 2016-10-09T16:23:29.940Z Reads: 45

```
Wow. Not only is everything working perfectly, this thing now absolutely destroys hills! So chuffed!!!
```

---
## \#9 Posted by: Sean555 Posted at: 2016-10-09T16:27:57.118Z Reads: 40

```
Kevin, can you post more pics of your modifications inside?  Interested in seeing how you connected everything
```

---
## \#10 Posted by: kevin.pritchard Posted at: 2016-10-10T06:40:55.535Z Reads: 33

```
<img src="/uploads/db1493/original/3X/6/4/648f97d2a41c0bb026f5322177140a402c28b095.JPG" width="375" height="500">

I've had to move the trucks and battery/ESC housing. For now, I've taped the 2nd ESC to the underside.

To power the 2nd ESC, I've taken the live and neutral from the other ESC (straightforward).

To get the motor to reverse direction, firstly i switched the red and black on the 3-phase cable. Next, i did the same on the 6-wire hall sensor cable (switched the red and black).

They now both spin in the correct direction with equal RPM (pitch is audibly the same).

Both ESCs have the stock RF receiver attached and respond at the same time.

This board now has some serious torque! Acceleration from stand still can easily throw you off!

Uphill feels so much less of a strain. The braking however, is TOO strong. Have to be really careful not to pull all the way back on the remote. The board stops DEAD. Perhaps this is something that could be overcome with VESCs in the future.

For now, ive put the board back in 'Fun Mode' because due to the extra torque and braking, theres a new learning curve!

Neverthless, with 2x1200W motors on a 60cm board, it feels like more than enough power than i could ever need. Very happy!
```

---
