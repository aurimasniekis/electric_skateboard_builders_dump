# Bms soldering help

### Replies: 29 Views: 1714

## \#1 Posted by: 2-alex-2 Posted at: 2016-11-03T20:50:52.956Z Reads: 149

```
Ok so my bms has arrived and wanted to know a few things. Is anyone running the same bms as me and help with wiring it up. If not hopefully shed some light. 

<img src="/uploads/db1493/original/3X/6/d/6d331ad78b702d036e51ae0cc7b9e3468b0c4f5a.jpg" width="375" height="500">

This is the bms 6s 5a I won't be running the esc through this it's only for charging but would like an led to activate and deactivate with this along with my esc low voltage cut off. 

So far I think I have this right. B+/ B- is where I solder the battery wires to ? 
P+/P- is where I solder my charging wires?
And lastly where would I solder a led indicator so if the bms picks up a low cell and the bms shuts down the led. Would I wire Led+ to P+ and them led- to D-  would this work ?
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-03T21:25:12.536Z Reads: 136

```
There's a separate circuit for LVC and HVC, you would need to identify is and plug to that. If i were you, i wouldn't mess with the bms. Any change in resistance, etc, will probably change the way it works.
```

---
## \#3 Posted by: chinzw Posted at: 2016-11-03T21:43:08.937Z Reads: 129

```
Actually, now that i think about it, this should be pretty simple. 12v led and a 10k/20k voltage divider between d- and battery positive.
```

---
## \#4 Posted by: 2-alex-2 Posted at: 2016-11-03T21:46:55.485Z Reads: 125

```
That's if D- is the hvc output from looking at the boards routing I think it is.
```

---
## \#5 Posted by: Stef Posted at: 2016-11-03T21:47:49.449Z Reads: 123

```
What you suggest probably works fine, though if the ESC low voltage cutoff is earlier than the BMS's, then the LED wont really be of much use as your ESC will cut the power to the motor when your BMS is still lighting up your LED.
```

---
## \#6 Posted by: 2-alex-2 Posted at: 2016-11-03T21:50:21.866Z Reads: 113

```
That's correct but if in say a years time when cells are getting old and say once set of cells drop voltage faster than the others the bms will pick that up I hope. As esc only picks up the total combined voltage.
```

---
## \#7 Posted by: chinzw Posted at: 2016-11-03T22:18:15.869Z Reads: 99

```
Yep, for the ESC LVC he will need to wire to the esc, not the bms.
```

---
## \#8 Posted by: 2-alex-2 Posted at: 2016-11-03T22:20:03.968Z Reads: 97

```
But it's only a 5a bms so I won't do that will let the esc handle the low voltage cutoff and the bms handle the low cell voltage but led indicator but hopefully bms will actually not be needed as esc will do its job.
```

---
## \#9 Posted by: chinzw Posted at: 2016-11-03T22:23:38.353Z Reads: 99

```
So... lets see, if you want an LED to turn off when the BMS LVC kicks in, just wire as i said. If you want an LED to turn on when the ESC LVC kicks in then you will need to wire it to the ESC.
```

---
## \#10 Posted by: 2-alex-2 Posted at: 2016-11-03T22:33:42.903Z Reads: 95

```
No just for the bms lvc as I have a battery % guage on top on the deck as well so should all be fine anyway but just making sure it's safe and not ran to low and seeing as I'm rebuilding the board may as well do it now.
```

---
## \#11 Posted by: chinzw Posted at: 2016-11-03T22:40:01.978Z Reads: 83

```
then just do a voltage divider with 10k/20k resistors between the d- and battery +, easy stuff. If you want the led to turn on when the LVC kicks in you can use a PNP transistor.
```

---
## \#12 Posted by: 2-alex-2 Posted at: 2016-11-03T22:44:06.424Z Reads: 82

```
Was just gonna ng to get it to turn off when it kick in easier to wire up.
```

---
## \#13 Posted by: chinzw Posted at: 2016-11-03T22:46:12.567Z Reads: 79

```
It will be ON all the time tough, as long as the battery is plugged to the BMS
```

---
## \#14 Posted by: 2-alex-2 Posted at: 2016-11-03T22:51:26.938Z Reads: 76

```
Well my switch has a separate led on it when switch the vedder soft switch on the led will come on but powered by the bms I hope lol
```

---
## \#15 Posted by: chinzw Posted at: 2016-11-03T22:55:47.333Z Reads: 78

```
Oh, then you can just use the + from the antispark switch and the D- from the bms, that way you wont need resistors or anything else.
```

---
## \#16 Posted by: 2-alex-2 Posted at: 2016-11-03T22:59:51.051Z Reads: 78

```
Yea it's also a 24v switch so the led should already have one in it I would emagine.
```

---
## \#17 Posted by: 2-alex-2 Posted at: 2016-11-04T15:08:12.288Z Reads: 71

```
Does anyone recon that I could upgrade this to handle more amps. As if you compare my pictur about and this 12a version. 
<img src="/uploads/db1493/original/3X/0/e/0ec5f09227037719be996c86902cbf22a32b7121.PNG" width="281" height="499">

There just seems to be more fets at the one end. Would it be possible to get it to run say 60/80a if I got some better suitable fets
```

---
## \#18 Posted by: chinzw Posted at: 2016-11-04T18:32:13.017Z Reads: 62

```
Im not sure how the over current protection works on this BMS, so it might not be possible, but looking at the first picture:
You dont even need to change the FETS, just buy 4 more of the exact same FETS that are already on the board. Those FETS are in parallel, so by adding 4 more you would theoretically increase the A rating from 5A to 15A. Or if you need more amps you can replace the FETS with ones that are rated even higher.

But, as i said before, depending on how the over current protection is designed this might not work.
```

---
## \#20 Posted by: 2-alex-2 Posted at: 2016-11-04T20:24:32.619Z Reads: 56

```
Yea I'm guessing they are 5a fets but if I got higher amp ones not sure if would work or not all depends on weather the board can handle 80a
```

---
## \#21 Posted by: chinzw Posted at: 2016-11-04T20:35:35.463Z Reads: 54

```
The traces are fine for higher amps, they tend to use the same pcbs for low and high amps, sometimes even same board between 6s and 7/8/9/10s or higher. But whatever is shutting down the fets in case of an over current, might still shut down at 5A even if you change the fets.
```

---
## \#22 Posted by: 2-alex-2 Posted at: 2016-11-04T20:45:30.680Z Reads: 43

```
O ok so the fets might actually handle higher amp but the smds on other pars of the board might not. Will try it the way I'm doing it now probably won't need it anyway as esc will cut if any issues. 

I had a response from the seller and he seems to think D- doesn't need to be used. But I can't see how it will cut if using only p-/p+ as that's stated as the charging side.
```

---
## \#23 Posted by: chinzw Posted at: 2016-11-04T20:50:24.374Z Reads: 43

```
The seller is right, if you want more than 5A you need to connect the battery directly to the ESC/VESC and also in parallel to B+ and B-. Then on P+ and P- you would connect your charger.
This will only protect the battery while charging, but will not protect overcurrent, overdischarge and overcharge from regen
```

---
## \#24 Posted by: 2-alex-2 Posted at: 2016-11-04T20:54:00.424Z Reads: 43

```
No but for discharging so for me led idea to work they say just connect to p-/p+ but from what I can see that would only cut off on charging not discharging.
```

---
## \#25 Posted by: chinzw Posted at: 2016-11-04T20:55:16.491Z Reads: 41

```
oh, for the led, you need B+ and D-
```

---
## \#26 Posted by: 2-alex-2 Posted at: 2016-11-04T20:56:34.118Z Reads: 47

```
Yea that was my thought from the start but the seller says no. But they are Chinese and probably don't know much about the product.
```

---
## \#27 Posted by: chinzw Posted at: 2016-11-04T21:02:27.622Z Reads: 44

```
You can allways test all of this pretty easily. All you need is a dc-dc buck converter so you can adjust voltages and plug it into the first cell port, then adjust from 4v to 4.3 and check what happens with P+- D-, etc. Then do the opposite, start on 4v and lower the voltage to 2.3
```

---
## \#28 Posted by: 2-alex-2 Posted at: 2016-11-04T21:40:20.583Z Reads: 39

```
Yea don't have one or know anyone with one. Will just put the battery one charge up and make sure it cuts and then run them down and check that it cuts.
```

---
## \#29 Posted by: chinzw Posted at: 2016-11-05T00:52:42.944Z Reads: 41

```
You can get them from ebay/amazon for about 10$ :smile:
```

---
## \#30 Posted by: 2-alex-2 Posted at: 2016-11-05T01:12:44.820Z Reads: 40

```
Found a 3-40v one but need a power supply as was just the regulator but needs to go below 3v for liion
```

---
