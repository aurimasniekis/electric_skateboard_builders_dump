# Eskating Dual Beast Not working like it should

### Replies: 7 Views: 415

## \#1 Posted by: Leonardadelmann Posted at: 2018-08-23T16:38:39.625Z Reads: 151

```
HI!

I need some expert help here. A couple of days a go my lost Eskating Dual Beast was found (lost whilst shiping). Once I got it back I replaced the faulty motor myself (which I originally sent the board to italy for).

We started off by just doing motor detection in vesc which worked out fine. Whilst riding the board for 20k yesterday I got my 2nd drv8302 error, the first one I got the day before after. Turned out the motors were to closely mounted which also caused one of my belts to snap. Once back in the workshop we repositioned the motors, installed new belts (both sides) and I rode the board home. I could push it very hard without getting the previous drv errors, but had roughly 10km/h top speed missing.

This morning I went into Vesc->General>Current and changed battery current max from 40 A, battery current max regen -10 to 35, -10. Did this to my master and my slave. After doing this the motors started working incorrectly.

So I started out from scratch. Did motor setup wizard for master, slave, then input setup. Which from the testing within my home seemed to be working fine.

When I went out for the ride on the other hand I got double cut outs within 4-5 min. First pushing the board uphill and the second one just pushing it after going uphill for a bit.

Comming home I felt the motors being pretty hot for just going for a 10 min ride which it was at most.

I don't really dare to ride the board untill I got this figured out. Could it be the drv (on my slave foc failing and causing cut outs, but would this make the motors go warm?

/beginner eskater trying to figure out why my board isnt working.

![39913948_10215773420722812_1592008208984047616_o|690x388](upload://n19kETUMgT9QudJxuGDU1qrZAaV.jpg)![39945332_10215773423042870_8257972635502116864_o|690x388](upload://kfi4vw4KoXo9771kxKU23HPeuo4.jpg)![39951640_10215773416202699_3957837153815232512_o|690x388](upload://jodfUUXgYtivo9ptZMAGHkUkbei.jpg)![39967462_10215773418162748_669894179530211328_o|690x388](upload://i4w6n0IAZZwu3j2dBZUPj2FHPgH.jpg)![39964282_10215773418922767_2032694028469796864_o|690x388](upload://mIIiO22ZtTp8MfHfD2FuYzsRKzL.jpg)![40022352_10215773421722837_8132294775660347392_o|690x388](upload://d9dXJka9B2nxyVvC4nUO8lCXRqz.jpg)![39960772_10215773417162723_7607321988222156800_o|690x388](upload://yB0aNfkCfl2z0auJrELQXXt2nSi.jpg)
```

---
## \#2 Posted by: Leonardadelmann Posted at: 2018-08-23T16:49:37.261Z Reads: 129

```
https://eskating.eu/product/eskating-dual-beast-landy-evo-7020watts-10s4p-30q-fully-assembled/
```

---
## \#3 Posted by: legend27 Posted at: 2018-08-23T17:31:10.162Z Reads: 121

```
Try to send Alberto @fottaz an email. He usually answers within a day. Hopefully it will get fixed.
```

---
## \#4 Posted by: Blasto Posted at: 2018-08-23T17:40:16.706Z Reads: 116

```
Did you do your sensor setup w the new motor?

(6th screenshot)
```

---
## \#5 Posted by: TowerCrisis Posted at: 2018-08-23T19:58:57.361Z Reads: 92

```
Honestly, the surefire way to know exactly what is wrong would be to ride it, make it cut out, and then USB in without power cycling the board. Just keep it on after it faults.

In the terminal just enter "faults" without quotes and it will tell you what error is occurring. This will likely lead you to whatever setting isn't right.
```

---
## \#6 Posted by: Leonardadelmann Posted at: 2018-08-28T11:17:01.999Z Reads: 53

```
Little update. Gonna try running the motors in bdlc instead of foc just for fun and see if it changes the outcome at all. My uneducated guess is that the right drv chip got damaged by the faulty motor that I had previously. Whilst riding last time I got right motor cutoffs, same side as the original motor broke. So obv there is something up with the right foc box. 

Been trying to contact @fottaz but havent gotten any reply yet. I could either have the drv chip replaced locally or (I hope) get a new foc box sent to stockholm and send him the faulty one back. 

Considering the amount of trouble I've had not only with shipping (one faulty motor and now one faulty foc box I would hope that he could possibly send me a replacement foc box). I'd send him the faulty back which he maybe can do a claim with. 


All in all, bought the board off a guy who had ridden it twice. The board was more or less brand new, I took it for one ride where the motor already broke (magnet starting to come off). 

I really love the board, just wish Alberto had a little less on his plate so he could take care of existing customers as well.
```

---
## \#7 Posted by: amanuelamanuel Posted at: 2019-05-15T11:01:55.577Z Reads: 23

```
Any update on this? Heard back from Alberto yet?
```

---
