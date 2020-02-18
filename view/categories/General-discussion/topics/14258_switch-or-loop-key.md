# Switch or loop key?

### Replies: 18 Views: 2386

## \#1 Posted by: Koto Posted at: 2016-12-06T11:38:07.978Z Reads: 341

```
kind of stuck on which one, what do YOU think is better. 
switch or loop key

btw is this reliable http://www.ebay.com.au/itm/2-Pcs-x-ON-OFF-2-Position-SPST-2-Pin-Snap-in-Rocker-Switch-16A-250V-20A-125V-AC-/221602299803?hash=item339886bf9b:g:zjEAAOSwcF9UYcjG
```

---
## \#2 Posted by: jujet Posted at: 2016-12-06T11:40:16.080Z Reads: 341

```
Use a loop key, it's very convenient and easy to use

That switch is for AC, you need one for DC
```

---
## \#3 Posted by: JLabs Posted at: 2016-12-06T11:40:16.936Z Reads: 336

```
That switch would not work. It would cause a spark every time you turn on the circuit and eventually wear down the switch until it does not work. A loop key is a bit harder to do, but the cheapest most reliable way to turn on and off your skateboard.
```

---
## \#4 Posted by: Koto Posted at: 2016-12-06T11:41:08.076Z Reads: 332

```
cool good to know before i blew my circuit :relaxed: i am a noooooooooob
```

---
## \#5 Posted by: Monte Posted at: 2016-12-06T11:42:34.760Z Reads: 327

```
If you use a switch, it would break after 5-10 uses. It stays on if it breaks
```

---
## \#6 Posted by: Koto Posted at: 2016-12-06T12:00:02.907Z Reads: 320

```
http://www.ebay.com.au/itm/DC-36V-2A-Off-On-NO-16mm-Metal-Flat-Momentary-Push-Button-Switch-SH-/252613191845?hash=item3ad0eb68a5:g:FLsAAOSw4GVYFvwv

how does this one work
```

---
## \#7 Posted by: mmaner Posted at: 2016-12-06T13:54:06.697Z Reads: 304

```
Thats an On/Off/On switch, so no it wont work.  Its also only 2 amp, so it wont work.  You either need...

MEB Power Switch http://miamielectricboards.com/shop-1/120amp-12s-power-switch
or 
Car Audio Circuit Breaker
http://www.ebay.com/itm/162119251810?_trksid=p2060353.m2749.l2649&var=461081390227&ssPageName=STRK%3AMEBIDX%3AIT
```

---
## \#8 Posted by: jmasta Posted at: 2016-12-06T15:36:59.143Z Reads: 276

```
A circuit breaker like that is not specifically designed for spark suppression and is generally not recommended
```

---
## \#9 Posted by: mmaner Posted at: 2016-12-06T15:39:02.147Z Reads: 275

```
I keep hearing those arguments, but here's the facts.  Its got plenty of amp protection and I've been using one for 3 moths with no problems.  If it fails, no big.  They cost less than 10 bucks and takes 2 mins to change out.

Also, you can use an anti-spark key (xt90).
```

---
## \#10 Posted by: Koto Posted at: 2016-12-06T23:34:55.757Z Reads: 252

```
does the 120 amp switch go just before the vesc and if you look at "Great Scott"s youtube build, he uses a three position switch, how does it work?
```

---
## \#11 Posted by: hankhill Posted at: 2016-12-07T00:02:19.281Z Reads: 244

```
So this switch typically goes between the battery and the esc. I looked at "Great Scott's" build and it looks like he's using this switch http://www.ebay.com/itm/171907590479?rmvSB=true which won't work as it's an AC switch rated for 6A. Since the switch is going to open/close the full circuit it needs to be able to withstand the continuous high current electric skateboards demand, which at a minimum is going to be around 35-40A. I'm guessing the switches that he used in his build probably stopped working. As @mmaner said, your only options is really to use a FET based soft switch like the one linked, a circuit breaker, or a anti-spark loop key.
```

---
## \#12 Posted by: mmaner Posted at: 2016-12-07T00:14:35.506Z Reads: 230

```
If you wnat to use a circuit breaker...Get a 100 to 120 amp DC Circuit Breaker, typically called audio circuit breaker.  It will go inline on the POS lead between the battery and the ESC.
```

---
## \#13 Posted by: Koto Posted at: 2016-12-07T00:16:56.910Z Reads: 230

```
ill stay with loop key, later might get switch
```

---
## \#14 Posted by: Namasaki Posted at: 2016-12-07T00:56:29.690Z Reads: 228

```
Any type of mechanical switch like an automotive breaker or toggle switch  is going to suffer from high voltage spark because of the rush of current to fill the Esc's capacitors. A mechanical switch will work but will wear out quickly. 
There are really only 2 good options  here. 
An electronic switch designed for high DC voltage and current. 
Or an anti-spark XT90 loop key connector. 
In my opinion, the loop key will be the least expensive and the most dependable.
```

---
## \#15 Posted by: mattdig Posted at: 2016-12-07T01:32:03.998Z Reads: 221

```
Ive been using a "20A/125V AC" switch for the last 2 years (a beefy metal one, not plastic). They're cheap enough that you can buy a few and replace them when they stop working, but I haven't had to do that yet. However I have ordered a 100A/48V inline breaker switch and I'm going to give that a shot.
```

---
## \#16 Posted by: caustin Posted at: 2016-12-07T05:11:03.145Z Reads: 211

```
For those of us "solder skill challenged" lol, is anyine sellling anti-spark XT90 loop key connectors pre-built?  Have already gone through several softswitch antisparks (they fail in the ON position at least lol), and incorporating XT90 anti spark connectors but would like it all in a loopkey setup. Anyone?  Thanks!
```

---
## \#17 Posted by: PDXroses Posted at: 2018-01-01T03:38:50.927Z Reads: 119

```
Oh this is a big find. Just double checking my understanding - the switch will no longer turn off after it malfunctions. Yes?  Thank you!
```

---
## \#18 Posted by: wafflejock Posted at: 2018-01-01T05:50:58.880Z Reads: 109

```
This is what he was saying I'm pretty sure... the general term is "failed closed" vs "failed open" when some components (capacitors, mosfets etc.) fry they will fail in one of these two ways.  If they "fail closed" then the circuit remains "on" or closed loop if they "fail open" then there is a break in the circuit when the component fails (generally better since the component is acting as a fuse but better if there's a fuse that does it instead).
```

---
