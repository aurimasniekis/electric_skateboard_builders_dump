# Tachometers &amp; Measuring RPM

### Replies: 10 Views: 1489

## \#1 Posted by: Mobutusan Posted at: 2016-07-14T23:03:53.532Z Reads: 124

```
Anybody have experience using these little handheld tachometers to measure motor or wheel rpm? While setting up my dual hubs, I noticed that each hub seemed to be running at different speeds, and one hub was getting hotter than the other. I think I fixed the settings, and got them in sync, but got to thinking that it would be nice to be able to measure and confirm that both motors/hubs are running at the same rpm. 

Here is one unit I'm considering buying. Any thoughts?

https://www.amazon.com/AGPtek%C2%AE-Professional-Digital-Tachometer-Contact/dp/B004Q8L894/ref=sr_1_2?s=automotive&ie=UTF8&qid=1468536997&sr=1-2&keywords=tachometer
```

---
## \#2 Posted by: sl33py Posted at: 2016-07-15T06:00:19.050Z Reads: 104

```
i got the sensors to do this for my eagletree v4 logger.  screen shows all sorts of cool detail and logs it for later.  I got the temp sensors for motors and batteries, plus the rpm sensors that 2 wires go to 2 of 3 phase wires from ESC.

http://www.eagletreesystems.com/index.php?route=product/product&path=62&product_id=64

gets a bit $$ to get all the components, but looks like a nice modular kit to monitor/log what you want!

HTH!
```

---
## \#3 Posted by: Mobutusan Posted at: 2016-07-15T08:00:17.026Z Reads: 91

```
@sl33py That looks really cool. Thanks for the link. Looks like it's around the $150 range for the v4 logger and all those sensors, right? That system looks like just what I was wanting when I got one of those cheap watt meters. Something that can log temps, speeds, voltage, current and capacity. Was is difficult to set up?

Is there an easy way to convert the motor rpm sensor data to mph/kph? It looks like they have an optical rpm sensor too that could be good for monitoring wheel speed, but would be even cooler if it could output mph/kph based on wheel diameter. If you've got more info to share about your setup, I'm all eyeballs.:nerd:
```

---
## \#4 Posted by: sl33py Posted at: 2016-07-15T08:05:24.578Z Reads: 76

```
I think i found it online for quite a bit less.  I'd do some hunting as i think i got it as a "kit" with the small LCD, then added the rpm and temp sensors.

I also went w/ the watt meter and loved it.  Except for the lack of logging, so as soon as powered off - all gone!  This will fix that.

As for speed - i usually use Strava app on my phone, but i think you can do this with *another* add-on GPS sensor for the v4!  Would keep it all in one place and include elevation gain...  slippery slope!  

Unfortunately i got waylaid w/ work and am just getting back to some of these project boards.  This was my "ultimate" setup for my replacement e-GBomb that i'm still not started on.  A couple practice boards first before i F up my new custom subsonic deck for e-GBomb v2!  (i'm going to CF wrap the whole board... just need to figure everything out first before ruining Scott's custom deck!)
```

---
## \#5 Posted by: Mobutusan Posted at: 2016-07-15T08:54:26.878Z Reads: 70

```
Good to know. I'll look around for a package deal on that system. I'd really like to log all this data and have it in one place. I've got a ghetto gopro type video datalogging setup with my watt meter for now. I'll probably still pick up one of the tachometers I linked to anyway, to take spot readings of my wheels & motors.
```

---
## \#6 Posted by: PB1 Posted at: 2016-07-15T13:16:16.126Z Reads: 66

```
This eLogger thing  looks very interesting! 

Two remarks: 
Is the eagletree logger going to cope with regen? @sl33py , how did your watt meter take it? I had also been running a WattsUp (this is not a typo!) and loved it. However I removed it because I live on the top of a hill and was afraid of frying my watt meter going down. Btw, would be interesting to see how many watts go back into the battery while braking. Can the eagletree do that? 

VESC has all of the information already (except external temperatures). various voltages, Amps, Temps of all of the six mosfets, rpm, ... 

Wouldn't it be easy to get the info out of the VESC and log it somewhere? Using an Arduino via UART 

I know that Jaccob is working on his VESC Connect, but his focus is more on the settings. 

Where are the smart electronic gurus? We need a "VESC black box"
```

---
## \#7 Posted by: devin Posted at: 2016-07-15T22:51:47.937Z Reads: 51

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#8 Posted by: Qwiksand Posted at: 2016-07-16T01:41:58.532Z Reads: 47

```
[quote="Mobutusan, post:1, topic:6120"]
Here is one unit I'm considering buying. Any thoughts?

https://www.amazon.com/AGPtek%C2%AE-Professional-Digital-Tachometer-Contact/dp/B004Q8L894/ref=sr_1_2?s=automotive&ie=UTF8&qid=1468536997&sr=1-2&keywords=tachometer
[/quote]

I've got one of those and it seems to work well enough. I've got no other way to measure RPMs to verify accuracy, but the values appear to be correct. It comes with a bunch of reflective tape to add to whatever spinny object you're aiming at.
```

---
## \#9 Posted by: onloop Posted at: 2016-07-16T02:09:43.518Z Reads: 45

```
[quote="Mobutusan, post:1, topic:6120"]
handheld tachometers to measure motor or wheel rpm?
[/quote]

you might want to check data from vesc BLDC tool.
```

---
## \#10 Posted by: Mobutusan Posted at: 2016-07-16T02:49:31.890Z Reads: 39

```
@devin nice find! Think I'm gonna get one. 
@Qwiksand thanks for the first-hand feedback. 
@onloop I don't have a VESC yet, but when I take the plunge, I'll be sure to check that out.
```

---
