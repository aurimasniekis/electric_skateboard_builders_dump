# Bumps in road causing electronics to freak out?

### Replies: 10 Views: 761

## \#1 Posted by: Pafrican Posted at: 2017-08-22T03:18:20.701Z Reads: 110

```
Hey guys,

I inevitably rode over a thick metal plate that spans across the center of a bridge. The impact caused my board to randomly die out; it was not responding to my transmitter. I restarted the system and was riding a-okay again.
I approached a second bridge with a similar metal plate spanning across the center. I decided to ride over it much slower to minimize the impact. The opposite effect happened, my board went full speed and threw me off. It wouldn't stop until it hit something else.

The electronics were held onto the board with velcro and electrical tape at the time as I was still prototyping. Anyone know why the board freaks out when it goes through a sudden jolt or impact? Do I need to mount the electronics to the board using rubber bushings?

I was using FS GT2B trans/receiver and VESC. 

Thanks!
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-22T03:26:31.459Z Reads: 105

```
Sounds like the servo cable became loose, could you post your specs.
```

---
## \#3 Posted by: krloz Posted at: 2017-08-22T07:45:49.031Z Reads: 79

```
Intermittent/weak wire connection or solder I would say. 
So a bench test and move around all the wires to see if something happens
```

---
## \#4 Posted by: darkkevind Posted at: 2017-08-22T08:08:45.853Z Reads: 71

```
I second the servo wire being loose, this happened to me. To remedy it, take the connector off of the receiver, get a small flat screwdriver and bend 1 or 2 of the pins either end slightly outward from the middle pin. Replace the connector for the ESC and it will be a lot more secure...

You could then tape it down with electrical tape to be bullet proof.
```

---
## \#5 Posted by: TehAtheist Posted at: 2017-08-22T08:12:12.662Z Reads: 68

```
Hmm, I don't think that a motor wire came loose like others are suggesting. Because that would make your VESC throw a Over_Current error, along with a full brake of the motor. And that didn't quite happen, right?

I have experienced drop outs of my old remote (winning), when riding close to big metal objects such as bridges or fences. It's possible that you were experiencing loss of signal. In the case that you were NOT accelerating your motor will either brake or go in neutral (depending how you set it up, correctly or wrong :p ) and if you'd be accelerating, it would continue to do so until it reconnects or until the timeout is reached (configured in VESC settings, default is 1s).

So if the second time, your bord kept accelerating, was it less than or equal to 1s (or whatever value your timeout is set to)? If so, this will be your issue.

Edit: Or as **darkkevind**(edited for bad spelling, sorry :dizzy_face: ) said above, that's also possible! But it'll have the same symptoms as I described.
```

---
## \#6 Posted by: lox897 Posted at: 2017-08-22T08:13:31.370Z Reads: 60

```
Exactly what I thought @Jinra . Same thing happened to me and caused random dropouts on impact.
```

---
## \#7 Posted by: lox897 Posted at: 2017-08-22T08:14:42.292Z Reads: 58

```
Hold on... who suggested that motor wires came loose? We said servo cables... receiver to vesc connection...
```

---
## \#8 Posted by: darkkevind Posted at: 2017-08-22T08:15:07.672Z Reads: 58

```
darkdavid? Lol
```

---
## \#9 Posted by: TehAtheist Posted at: 2017-08-22T08:17:32.696Z Reads: 56

```
Haha, my bad. I'm checking this forum while learning for my exams and I'm trying to do it to fast!
Won't happen again ;)
```

---
## \#10 Posted by: rich Posted at: 2017-08-22T09:09:28.185Z Reads: 51

```
On my longboard build I had dropouts on bigger bumps, too. After adding foam to the vesc and receiver it never happened again. But after a while my board started to act like a evil ghost, randomly there was full throttle for no reason, this was so scary and also embarrasing when people watching :joy: fortunately I never had an accident. After a couple of rides full of adrenaline I realized that the servo cable was bend too much after the plug because the enclosure was too tight. There was a loose contact in the cable that's why it happened sometimes depending on vibrations.
```

---
