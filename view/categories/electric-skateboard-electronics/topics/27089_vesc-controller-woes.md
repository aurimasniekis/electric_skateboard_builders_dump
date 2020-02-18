# Vesc controller woes

### Replies: 22 Views: 1622

## \#1 Posted by: ugothakd Posted at: 2017-07-08T20:41:49.743Z Reads: 130

```
Fried my first drv on the vesc, so I got a new one and everything was fine for a few weeks but after hitting a pretty solid bump my board died. I checked it out and the vesc doesn't turn on at all, the LEDs don't shine. I get voltage at the terminals on the vesc and it sparks when connecting. I tried to test for 5v at the connector next to the copper coil thing (don't know what it's called) and it doesn't seem to have voltage there, the multimeter reads something like .21v. Whenever I plug the battery in the copper coil gets extremely hot after a period of time. What could have happened? Really don't want to buy a third vesc<img src="/uploads/db1493/original/3X/6/b/6ba415339f077a8c36f528757c634fba8759b52d.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/5/e/5e118b24967ba21bf11dd1e7583a4e1b9d32d957.jpg" width="374" height="500">
```

---
## \#2 Posted by: goldenHusky Posted at: 2017-07-08T20:53:29.912Z Reads: 118

```
@JohnnyMeduse
```

---
## \#3 Posted by: rpn314 Posted at: 2017-07-08T20:55:42.894Z Reads: 119

```
While I can't do much about the issues with your DRV chip (other than offer to fix it or tell you who can), but I have seen a few issues with the the L1 inductor (the only thing I'd call a big coil thing) Where did you get your VESC(s)?
```

---
## \#4 Posted by: ugothakd Posted at: 2017-07-08T20:58:14.958Z Reads: 118

```
I bought it from a member on here, it worked for a bit but then stopped.. this vesc pictured the drv is fine, the other old one is dead in a box. Do you think I should just replace the l1 inductor or something else is wrong?
```

---
## \#5 Posted by: rpn314 Posted at: 2017-07-08T21:09:59.829Z Reads: 110

```
It may be possible to just replace L1, but its pretty difficult to say if that's the only problem. Do you know the original source?
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2017-07-08T21:11:06.259Z Reads: 106

```
Hi, 

First... 

<img src="/uploads/db1493/original/3X/6/5/65fde83fd9226e38ec9c59492b2a20c11f099e75.jpg" width="375" height="500">

From what I can see those PWM wire aren't insulate... witch mean that if you hit a big bump, they might move and short together, resulting in a dead VESC... Might be the drv since this is the part the give the 5v to the hole pcb... But It might also be the Can transceiver, since it's really the weakest link in the vesc,  you can test it with the following procedure. 

https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse
```

---
## \#7 Posted by: rpn314 Posted at: 2017-07-08T21:18:00.201Z Reads: 95

```
Wow good eye! I did not see that.
```

---
## \#8 Posted by: ugothakd Posted at: 2017-07-08T21:27:04.271Z Reads: 95

```
I checked the c25 capacitor and I get something different then the leads connected (was a value like 5-600 instead of 000 when connected). Does that mean it's the drv chip? When my last drv chip fried the vesc LEDs still flashed and turned on. Yes the ppm wires are not insulated.. I was excited to get it working I got sloppy and soldered the wires into the male connector instead of buying a female to female cable. Thanks for the help
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-07-08T21:38:01.616Z Reads: 94

```
[quote="ugothakd, post:8, topic:27089"]
Does that mean it's the drv chip?
[/quote]

Sadly... It look like the DRV burn... 

[quote="ugothakd, post:8, topic:27089"]
When my last drv chip fried the vesc LEDs still flashed and turned on
[/quote]

Different failure, will give you different result... Like if you short motor lead, there some part of the drv that could still work, like the internal regulator, but if you short the regulator (like in this case) drv won't even power up, resulting in a dead VESC.
```

---
## \#10 Posted by: ugothakd Posted at: 2017-07-08T22:14:50.189Z Reads: 90

```
Well.. I messed up my first drv repair, perhaps this one will go better. I had barely soldered before that but now I have much more experience.
```

---
## \#11 Posted by: rpn314 Posted at: 2017-07-08T23:56:58.837Z Reads: 81

```
Do you have a hot air gun? That's what made the difference for me on that particular chip.
```

---
## \#12 Posted by: ugothakd Posted at: 2017-07-09T00:21:14.981Z Reads: 76

```
I do indeed have a hot air rework station, my problem is I put the chip backwards. Then when trying again, I couldn't get it exactly on the pads
```

---
## \#13 Posted by: ugothakd Posted at: 2017-07-10T04:18:31.495Z Reads: 62

```
Well, I have successfully swapped the drv chip, and the problem is still here.... Any idea where to start next? Possibly swap the inductor?<img src="/uploads/db1493/original/3X/b/8/b8f56b885a1af38c5ddee43fe02f7309f58cbd73.jpg" width="374" height="500">

No LEDs inductor still gets hot
```

---
## \#14 Posted by: Blasto Posted at: 2017-07-10T04:24:28.226Z Reads: 61

```
Clean up the drv pins with flux, there is what seems to be a ton of whiskers

<img src="/uploads/db1493/original/3X/f/9/f9081666bf48685d9c98c06791156c6bfaeac6ad.jpg" width="281" height="500">

Check if your 3.3V rail is shorted...
```

---
## \#15 Posted by: ugothakd Posted at: 2017-07-10T04:33:12.547Z Reads: 58

```
Like hit it with the gun and some light flux? I just don't want to apply too much heat and it fall off. Where would I check the 3.3v rail?
```

---
## \#16 Posted by: Blasto Posted at: 2017-07-10T04:38:47.687Z Reads: 58

```
No clean it up with an iron, put flux and touch pin by pin.

For the 3.3V... check the connectors, its marked on the silkscreen
```

---
## \#17 Posted by: ugothakd Posted at: 2017-07-10T04:48:28.301Z Reads: 58

```
So when checking the 3.3v and using the gnd it's not shorted... However I made an interesting discover. When checking the c25 capacitor the capacitor was not shorted, so I assumed 5v was fine. But when checking the 5v and gnd pins I get a short...
```

---
## \#18 Posted by: Blasto Posted at: 2017-07-10T04:55:21.298Z Reads: 56

```
[quote="ugothakd, post:17, topic:27089"]
But when checking the 5v and gnd pins I get a short...
[/quote]

Ok, we're getting somewhere, clean up that drv before replacing anything else
```

---
## \#19 Posted by: ugothakd Posted at: 2017-07-10T05:07:39.238Z Reads: 57

```
I think that might be glare from my light off of the flux, I hadn't cleaned the flux off yet. I tried to clean it up but doesn't seem like much is different<img src="/uploads/db1493/original/3X/8/0/80dfd8c73c02ff2e086be7600a9634b61489a2c0.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/4/9/494b72f094e9a4354ed414c79c1060424cec0240.jpg" width="374" height="500">
```

---
## \#20 Posted by: ugothakd Posted at: 2017-07-10T05:51:10.194Z Reads: 58

```
Using a parts vesc, I swapped over a spare can transceiver (u401) AND swapped in a new drv and still shorting on 5v. Getting the exact some problem from the start, and inductor is still heating up when battery is connected
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2017-07-10T12:49:01.911Z Reads: 50

```
OK... Just remove the the tvs diode D5 and check if it still short... also before replace it make sure that the voltage on the 5v leg is 5V not 8V... (if it is 8V it mean that your pads under the drv isn't properly solder)
```

---
## \#22 Posted by: ugothakd Posted at: 2017-07-10T18:12:57.322Z Reads: 44

```
Replaced the diode, all is well!!! I'm going to be ordering a male to male cable so it doesn't short again. It's interesting that the old diode is considerably larger than my parts vesc diode, but I guess that means the parts vesc was not very high quality in the first place. Thank you so much.. I would have never known where to start<img src="/uploads/db1493/original/3X/7/2/728243509cf44a10c4859fe6a8e2444dc7a34658.jpg" width="374" height="500">
```

---
