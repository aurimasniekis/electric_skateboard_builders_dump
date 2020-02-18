# Focbox or Maytech VESC?

### Replies: 7 Views: 1970

## \#1 Posted by: ciscotory Posted at: 2017-10-08T16:27:51.554Z Reads: 305

```
serching to buy 2 VESC's online got confused between Focbox and Maytech, i understand both are VESC's
I'v read lots of posts regarding the difference between them,
still confued as which is better and why? 

why some skaters have problem with switching between FOS and BLDC as fear of frying their VESC?
this's confusing cus i thinkg BLDC is a tool in it self and FOS is a setteing option in it!! if not mistaken.
or BLDC  and FOS are actully a setting option in VESC-tool?

how can i avoid frying VESC, as i'm still trying to learn what is Install/check Bootloader and what is a Firmware, if i didn't request installing these configuration when buy online?

Thanks guys :v:
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-10-08T16:48:07.959Z Reads: 296

```
BLDC and FOC are two different methods of controlling a BLDC (BrushLess DC) motor. FOC stands for Field Oriented Control, and allows the motor to run more quietly and have smoother torque at low speed. BLDC is the standard control method used my all RC car and airplane speed controller. It's simple, louder, less smooth, but it is easy to get right.

Maytech vescs are built down to the absolute minimum price, which means they use the cheapest parts and they usually leave some out. They sometimes work with BLDC but if you try to use them with FOC, they fry themselves because the missing parts were designed there for a reason.

FOCBOX is an upgraded, improved version of the vesc hardware, specifically designed to handle FOC well without frying itself. It's more robust, has all the parts, and many of the parts are upgraded.

TL;DR get a FOCBOX, maytech vescs are garbage. FOC and BLDC are different, and you should read about them.
```

---
## \#3 Posted by: psychotiller Posted at: 2017-10-08T17:24:01.046Z Reads: 266

```
While I agree that Focbox's work better with FOC, There are still numerous posts about them getting fried...

I also agree that Maytech vescs run better with BLDC and not FOC. FACT. 
But they work fine with BLDC. Seriously. I've had 2 returns total on maytech vescs. And one of them was because of user error (which is 98% of the time why all drv's die)

Stop saying that one thing is shit while not acknowledging that the others have issues as well.

When someone asks for advice, and you wan't to help, why not give solid. informed information?
```

---
## \#4 Posted by: Bataleon Posted at: 2017-10-08T17:36:47.579Z Reads: 253

```
[quote="psychotiller, post:3, topic:35109"]
But they work fine with BLDC. Seriously. I've had 2 returns total on maytech vescs. And one of them was because of user error (which is 98% of the time why all drv's die)
[/quote]

Ditto. I wouldn't try FOC mode but have over 300km in BLDC on a Maytech VESC. Never had a single issue. Also FOCBOX is literally twice the price.
```

---
## \#5 Posted by: psychotiller Posted at: 2017-10-08T17:39:57.986Z Reads: 239

```
Yeah, foc is a gamble with the maytechs but they certainly don't suck with sensored BLDC and they are 2.54 now out of the box.
```

---
## \#6 Posted by: chewydinosaurs Posted at: 2017-10-08T22:49:42.324Z Reads: 206

```
Tried a DIY electric skateboard vesc, foc worked but seemed to progressively get noisier. My vesc eventually fried the other day. I had a friend discharge it by running the motor half throttle for 8 minutes as I left it at his house. He tried turning it on 2 days later and DRV is fried (erpm limit was set). How I see it is FOC is always a gamble.
```

---
## \#7 Posted by: racidon Posted at: 2017-10-08T23:09:42.625Z Reads: 190

```
Get a Chakka VESC mate, best I've had and the settings he has should be sufficient for basic bldc setup.
```

---
