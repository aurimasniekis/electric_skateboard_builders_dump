# BMS with e-switch - pros and cons, and how to charge/discharge elegantly?

### Replies: 14 Views: 2285

## \#1 Posted by: eitan Posted at: 2017-03-25T09:39:21.252Z Reads: 366

```
I'm struggling to understand whether I should get an E-switch on my BMS*. 

The pros:

1. The e-switch eliminates the need for constructing an antispark switch.
2. One can solder a physical switch to the two ends of the e-switch, and when the switch is ON, the board is ON.

The con:
**My understanding is that the switch needs to be on for both charging and discharging.**

For those with experience, do you not find this cumbersome? 

* Charging should an issue of plugging the charger in, and not be coupled with turning on the rest of the components.
* Discharging (turning on the board) should be an issue of flipping a switch.

Why is this so complicated?

Two important posts for context and learning: [E-switch on BMS](http://www.electric-skateboard.builders/t/e-switch-on-bms) and [Namaski's topic](http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/)

*I plan on ordering from Batterysupports, because their 60A 10S BMS is compact (10cm x 5cm). They offer e-switches by special request.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-03-25T17:38:17.350Z Reads: 329

```
I have no experience with the battery supports BMS. 
I can say that the Bestech BMS with E-switch has been very dependable for me. 
And that having the whole system on during charge cycles has not been an issue for me.
```

---
## \#3 Posted by: Eboostin Posted at: 2017-03-26T04:30:05.097Z Reads: 309

```
Yuneec Ego has a e-switch BMS that can be off during charging. It has been very reliable. 

If someone could offer a BMS like theirs, that would be the best of both worlds.
```

---
## \#4 Posted by: Jebe Posted at: 2017-05-09T07:10:41.322Z Reads: 281

```
Have you got a link to that BMS ?
```

---
## \#5 Posted by: Namasaki Posted at: 2017-05-09T16:04:26.319Z Reads: 267

```
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
Bestech sales are done through email.
Send an email to lucy@bestechpower.com requesting to purchase the bms module.
The minimum purchase is for 2 modules.
The cost is $49 ea. plus shipping and PayPal fee.
If you don't want to keep the extra module, they are easily sold on this forum.
Some of the parameters are adjustable at the factory and you will need to specify your preferences during the order process.
I recommend these settings for Lipo batteries, for Li-ion you could lower the over discharge voltage detection to 2.8v

<img src="/uploads/db1493/original/3X/8/3/8322617f0d408056e732d78fdf6dc209da0cf6f8.png" width="355" height="499">
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-05-09T16:17:36.096Z Reads: 242

```
i use a vedder switch with my battery supports BMSs. I just personally would rather not have the board on while charging unless i just want to check the voltage real quick. It not bad for it or anything, i just feel better with it off for some reason. 

Also, when you have reverse enabled and the board is on but the remote is off, some VESCs will sit there and twich the motors as the PWM signal receives noise from the ambient radio cloud that consumes us all. Some find it really annoying. So i decided to use separate switches.
```

---
## \#7 Posted by: Brando Posted at: 2018-07-27T04:52:42.436Z Reads: 136

```
Does your BMS eSwitch have a big delay when you flip the switch on? It takes mine like 8 seconds for the BMS to send or stop the current.
```

---
## \#8 Posted by: Acido Posted at: 2018-07-27T06:05:43.428Z Reads: 130

```
The bms turns on instantly, at least mine does
That delay is probably your remote connecting
```

---
## \#9 Posted by: Namasaki Posted at: 2018-07-27T11:56:26.263Z Reads: 127

```
It takes about 6 seconds for the Vesc to boot up when you turn it on. 
It takes a little longer for the voltage to drain down when you turn it off.
```

---
## \#10 Posted by: Brando Posted at: 2018-07-27T12:24:31.451Z Reads: 121

```
@acido @Namasaki I don't even have a VESC Attached. Just a multimeter monitoring the bms output. When off, the voltage is reading 8V, and when on after about 8 seconds the voltage goes up to 37V. I'm talking with BesTech about it rn.
```

---
## \#11 Posted by: DJ8055 Posted at: 2019-07-19T08:51:06.820Z Reads: 47

```
What bms do you use? Can you drop a link? Also what switch? (For 10s 4p Samsung 30q)
```

---
## \#12 Posted by: longhairedboy Posted at: 2019-07-24T14:53:57.425Z Reads: 43

```
i build 12S boards. If you want a decent 10S BMS, check out http://www.batterysupports.com/lion-lipo-nbsp-36v-nbsp-10s-c-32_41.html

I don't use eswitches anymore, and I generally do a discharge protection bypass. The unity fixed all of those problems.
```

---
## \#13 Posted by: L3chef Posted at: 2019-07-24T19:09:22.552Z Reads: 34

```
[quote="longhairedboy, post:12, topic:19652"]
I don’t use eswitches anymore
[/quote]

Care to elaborate why you don't use them anymore?
```

---
## \#14 Posted by: longhairedboy Posted at: 2019-07-24T19:27:10.949Z Reads: 34

```
They come built into the unity, so no need to find, test, and abuse discreet eswitches that have consistently failed on me. The unity just works 100% of the time for me. 

The only eswitch i haven't had a problem with is the 300 amp Flier one and you have to order five at a time to get them, and they're 5 fets long so they're huge.
```

---
