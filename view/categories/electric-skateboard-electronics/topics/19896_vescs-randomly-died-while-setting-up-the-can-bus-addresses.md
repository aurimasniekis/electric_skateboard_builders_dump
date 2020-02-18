# VESCs Randomly died while setting up the CAN bus addresses

### Replies: 23 Views: 1655

## \#1 Posted by: Sourcecode Posted at: 2017-03-29T07:36:23.020Z Reads: 155

```
Hello team,

I have an issue during the setup of my Vescs (while adressing the vescs for canbus) the master vesc kept disconnecting from BLDC then the slave vescs lights turned off so i unplugged the power to them both now neither one will power up or connect to BLDC, motor detection for  both vescs worked fine and all settings saved previously. I have posted some images below i cannot see any faults with the pcb, any help or ideas would be appreciated! 

http://imgur.com/Ql8gT4T
http://imgur.com/gvU1YkV
http://imgur.com/4jCPcsG
http://imgur.com/rsVBH6Z
http://imgur.com/cRErsn3
http://imgur.com/hrqe0ul

-12s ( 2 x 5000mah 6s packs in series) 
-192kv SK3 motors  
-VESC X
```

---
## \#2 Posted by: laurnts Posted at: 2017-03-29T08:05:42.902Z Reads: 138

```
Maybe wrong can bus polarity?
```

---
## \#3 Posted by: Sourcecode Posted at: 2017-03-29T08:25:44.385Z Reads: 140

```
I had a look and it and its all good, it did work briefly before it all died
```

---
## \#4 Posted by: Jebe Posted at: 2017-03-29T09:23:34.311Z Reads: 137

```
I've had 2 sets of enertion vescs fail with canbus. I attributed mine to bad solder connections on a r spec motor. Were you doing motor detection at the time?
```

---
## \#5 Posted by: Jebe Posted at: 2017-03-29T09:30:59.062Z Reads: 131

```
http://www.electric-skateboard.builders/t/need-help-dead-vescx-and-3-dead-vesc/18666
```

---
## \#6 Posted by: Sourcecode Posted at: 2017-03-29T09:35:34.056Z Reads: 127

```
interesting thanks ill have a look through that thread. I had already done the motor detection on both vescs.I was just setting up the addresses when things went a bit nuts. its a tad frustrating lol
```

---
## \#7 Posted by: Blasto Posted at: 2017-03-29T12:44:10.698Z Reads: 123

```
Where is you CAN bus wire? How does it look like?
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-03-29T12:51:58.082Z Reads: 122

```
Do the vesc still light up when you open them, if not can you check if the can tranceiver is broken. This kind of damage occur when you short the can connection. 

C25 on vesc-X is this one: 
<img src="/uploads/db1493/original/3X/1/7/17c1848535a8b915cbb9dbf013809fbbcf5e1551.jpg" width="375" height="500">

Also, make sure you don't damage the dissipative tape on the mosfet. 

http://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-03-29T12:54:05.515Z Reads: 118

```
Sorry @Jebe I've read your thread and the damage seem more to be the motor, not the can connection.
```

---
## \#10 Posted by: Jebe Posted at: 2017-03-29T20:06:22.816Z Reads: 109

```
I've bought 2 new motors, my concern was that the slave motor was taken out as well.
I will be going with a Y connector splitting the ppm signal next, just waiting for my vesc 6's.
Appreciate your advice bud, thanks for replying.
```

---
## \#11 Posted by: Sourcecode Posted at: 2017-03-30T01:03:08.889Z Reads: 101

```
Thanks for the reply. No lights but my receiver still has power, I also have dead short across the c25 cap.
```

---
## \#12 Posted by: Sourcecode Posted at: 2017-03-30T01:04:06.511Z Reads: 99

```
I'm not at home atm but it was just standard 2 wire canbus connection
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-03-30T01:05:39.039Z Reads: 97

```
so you to change U401 witch the can tranceiver chip.
```

---
## \#14 Posted by: Sourcecode Posted at: 2017-03-30T05:36:33.953Z Reads: 93

```
So just to confirm I'm testing from the c25 cap to the 5v and I should get open circuit? 

Between C25 and 5v -  open circuit 
Between C25 and can H  - short circuit 
Between C25 and can L - short circuit 
Between C25 and gnd - short circuit 
Between 5v and gnd, canH, canL, gnd - open circuit 

Thanks for your input it's much appreciated!
```

---
## \#15 Posted by: Sourcecode Posted at: 2017-04-12T05:53:26.883Z Reads: 84

```
Just to close the thread if anyone reads this it was the transceiver chip in the end 

http://imgur.com/yAVhx2n

http://imgur.com/fGqfD7t
```

---
## \#16 Posted by: Jebe Posted at: 2017-04-15T06:24:38.588Z Reads: 70

```
when you removed it could you connect with the bldc tool and run as a single?
```

---
## \#17 Posted by: Sourcecode Posted at: 2017-04-15T08:24:22.257Z Reads: 68

```
Yep you can connect to it after the chip is removed
```

---
## \#18 Posted by: thisguyhere Posted at: 2017-04-15T08:33:30.979Z Reads: 68

```
might be kind of late in the game to even mention this but [skip the CAN altogether](https://www.electric-skateboard.builders/t/how-should-i-go-about-programming-double-vesc/19731/20).
```

---
## \#19 Posted by: Sourcecode Posted at: 2017-04-15T08:38:56.843Z Reads: 69

```
Yep I'm just running it with a y splitter and no canbus atm
```

---
## \#20 Posted by: Jebe Posted at: 2017-04-15T09:11:02.245Z Reads: 65

```
I wish I had have....was waiting for a response from enertion which never came and blew two more vescs :(
```

---
## \#21 Posted by: miodice3 Posted at: 2019-04-05T20:20:03.864Z Reads: 21

```
I know this is an old thread but are there any tips to not kill these, i got 2 brand new form diyelectricskateboards, and followed all their instruction and they died completely. They are being resent but i am afraid to configure them and kill them again.  I suspect they may not have tested them completely as they claim to do because i used all 100% their stuff, 36v li ion battery, and have a lot of experience with this stuff, didn’t reverse any polarity at all and just totally frustrated.  Any tips on this, i see some talking about the Y adapter, but have read that the voltage differences under load can cause ground loop issues and kill the VESCs.
```

---
## \#22 Posted by: Andy87 Posted at: 2019-04-05T20:36:31.812Z Reads: 19

```
Don’t switch on or off only one esc while CAN Bus connected. Don’t disconnect the can bus while your esc are on. If you use y-split for your ppm instead of can thsn cut the middle wire on one of the ends. I think that’s pretty much all.
```

---
## \#23 Posted by: miodice3 Posted at: 2019-04-05T20:43:31.586Z Reads: 16

```
So plug everything in together, xt90 parallel connector, CanBus connector, motors, then plug in correct?  Seems really easy but want to be really clear, nothing like seeing $200 evaporate in front of your eyes.

Can you confirm the VESCs should indpenently be setup 100%, then plug it all in together, or are you supposed to hook all the wiring together, then configure via usb together after they’re all connected?
```

---
