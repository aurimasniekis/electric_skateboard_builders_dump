# Recurring power cutouts after shorting battery during charge

### Replies: 22 Views: 400

## \#1 Posted by: Teo Posted at: 2018-06-09T12:06:13.438Z Reads: 89

```
Hello everyone!
It's my first post here. I have been reading a lot of threads and the time has come for the first question :)

While unplugging the battery that I was charging I shorted it against the aluminum case where I keep all the electronics under my board. You can see it here in the photo:

![DSC_0013%20(1)|690x388](upload://czaPiBdGS0nb63ODNp4lSPuFRYZ.JPG)

The Vesc was unplugged but still in the case and it could have touched the bottom of the case through the usb port or any other part. It does look completely fine and it doesn't heat up when using it (with or without load).

At the same time I'm not managing to ride anymore because as soon as I get in the street and speed up the power cuts off after the first meter (this is the behavior I was getting with a discharged battery or on too steep uphill). I did try to change the battery but it behaves exactly the same way.

I tested it indoor in a sleek corridor and it was working just fine but in the street it just cuts off when I accelerate. At times I manage to do a few proper starts and then it starts cutting off again. 

It seems like it's not managing to handle medium high currents anymore... but from the outside it looks all fine.

Before replacing the Vesc, does anyone have an idea of what could have happened or what I should be looking into?

Thanks!
```

---
## \#2 Posted by: FabianOdermatt Posted at: 2018-06-09T15:51:55.030Z Reads: 73

```
Can you send us your VESC settings? That will help alot I think.

After that, try it again and when the power cuts off again, don't shut down the VESC. Plug it in your computer and write "faults" in the terminal. It will show you all the faults since the last startup.

I think your VESC isn't broken. There was no load through the VESC when you shorted the batterie. Maybe there is a loose connection in the batterie caused from the short.
```

---
## \#3 Posted by: L3chef Posted at: 2018-06-09T18:11:21.051Z Reads: 63

```
I'm colorblind so I can't read the text in the middle. What does it say?
```

---
## \#4 Posted by: DougM Posted at: 2018-06-09T19:13:26.904Z Reads: 58

```
Wait, so it works on a smooth surface but does not work on rough pavement?   Sounds like a bad connection to me.  Check all your connections.
```

---
## \#5 Posted by: Teo Posted at: 2018-06-09T19:25:50.178Z Reads: 56

```
Hi Fabian, 
here are all the screenshots of the settings I was using:
![general|690x243](upload://8jV7eEqQCFMD1NO9SO8vXo7jR5o.PNG)
![advanced|690x206](upload://2yRV60IS3ZIE65dbkG9EoINAHnG.PNG)
![temperature|690x174](upload://75g7eSLm8r2ReB8lb3Dp6hf7bJp.PNG)
![Current|690x222](upload://qwWHbOUUfyT4EyBTFjkSh2crnbb.PNG)
![rpm|690x166](upload://l8u121v5xebWGOEfHPnSEcuvXe7.PNG)
![voltage|690x276](upload://q94BEEZczRngu3jG5MwLzr5R0ji.PNG)
![PPM|690x257](upload://sUy0xzNMEN1gNTvJHEODKWtbzQf.PNG)
![wattage|690x205](upload://ja8uZ0en2qhhh1YuEPWNFws2X5i.PNG)

And I just went out in the street to test it and this time it did two smooth starts even on rough pavement and then it completely stopped (It's actually the first time that it doesn't even make the wheel spin if I lift the board).  I got these FAULT_CODE_ABS_OVER_CURRENT errors:

![faults|467x500](upload://sKojQ68gmbIIjpvfU4qWDrUYWDC.PNG)
![faults%202|434x500](upload://jcnJ3cFFuDWGFTsUhy1qfYSI4MR.PNG)

It does go over the 130 amps limit but it's something new since I didn't change the setting from before. Not sure why is that happening now. 

I don't think the loose connection could be an issue because I'm using a new battery pack. And both the old (shorted one) and the new behave the same way.
```

---
## \#6 Posted by: Teo Posted at: 2018-06-09T19:27:50.009Z Reads: 44

```
it was to show the setup of the batteries. It says that the batteries were plugged in and I was removing the connectors at the end of a charge when the short circuit happened.
```

---
## \#7 Posted by: Teo Posted at: 2018-06-09T19:32:14.661Z Reads: 44

```
I thought of that as well but the weird thing is that nothing changed from before the short circuit and it all worked fine for a full month of use. Also now this time it worked fine outside as well for the first two starts. It looks like it starts ok in the beginning and then very soon stops being able to manage the current and does the cut-off in acceleration.
```

---
## \#8 Posted by: DougM Posted at: 2018-06-09T20:04:34.037Z Reads: 43

```
So it was the balance connector that shorted out?
```

---
## \#9 Posted by: wafflejock Posted at: 2018-06-09T20:05:09.156Z Reads: 43

```
My guess would have to be something got fried on the shunt resistor used to measure the current flow if you have access to an ammeter then could see if it's reporting the same or roughly similar amperage to the VESC.  Would also double check for anything mechanical creating extra resistance and increasing the actual load.
```

---
## \#10 Posted by: Teo Posted at: 2018-06-09T20:36:49.306Z Reads: 44

```
@DougM no, it's actually another connector coming out of the charger that in this case has no use. 
The two cables I'm holding were the ones connected to the battery and the other one on  the right was just dangling  unprotected too close to the metal case (I did learn a lesson here!).

![DSC_0022|690x388](upload://aff1ouhYztjdc0AAb2ZFSkNSKOy.JPG)

@wafflejock that could be indeed. Do you think it could have happened even if the vesc was unplugged and just close to all the aluminum case?  Not sure how to check with the ammeter while riding though :confused:
Quite sure that all the mechanics are fine and there was also no change from before the spark.

After the last test it actually doesn't even start moving anymore. The vescs turns on with the standard blue light. When I accelerate the motor hardly moves (it does like a tenth of a spin) and if I check the faults in the terminal I get the same error of FAULT_CODE_ABS_OVER_CURRENT.
```

---
## \#11 Posted by: wafflejock Posted at: 2018-06-09T20:54:58.758Z Reads: 36

```
In the real-time monitor does it show as really high amperage?  You could temporarily increase the max amps settings assuming nothing is actually getting hot or really pushing that many amps through.  Regarding testing was more thinking just bench test and see if a separate ammeter is reading roughly the same amps.
```

---
## \#12 Posted by: Teo Posted at: 2018-06-09T22:06:28.690Z Reads: 39

```
So I set the max current to 150A (max allowed on the tool) and it started twice. Then same issue again as it doesn't move anymore but this time the faults from the terminal show currents over 160A.  
I don't have an ammeter at home but i'll try tomorrow and see what's the reading.

I tried to switch it off and on and re-write the configuration but nothing changes. Still blue steady light and then red blinking light only when I accelerate and it doesn't start. I was holding the vesc while trying and nothing gets even warm. It feels just like the same temperature of when it is off.
```

---
## \#13 Posted by: DougM Posted at: 2018-06-09T22:53:12.484Z Reads: 34

```
Any chance you have someone nearby who can loan you a known good VESC for testing?  Where are you?
```

---
## \#14 Posted by: Teo Posted at: 2018-06-10T09:31:03.003Z Reads: 28

```
@DougM Yes I'm Dublin and working on it with a friend. We'll try to do that even if at this point there is a clear issue with the vesc.

@wafflejock I read in another  of your posts  that you gave tips on how to re-flash the firmware for 
this kind of problem. I did it this morning but even that didn't go through.
_Serial port error: Operation I/O stopped due to exit from thread or request of an application_ 
![error%20update%20firmware|690x402](upload://jUyMz3yyQ2PgaO6lxf8r9BtaR7q.PNG)

Now the lights stil switch on but it gives no signs of life when I accelerate, not even blinking. :frowning: 
Does anyone have any ideas on how to bring it back to life?
```

---
## \#15 Posted by: wafflejock Posted at: 2018-06-10T13:22:48.346Z Reads: 24

```
Sorry sounds pretty fried to me but not sure what else you can try or check at this point, maybe can get @JohnnyMeduse to chime in if he's familiar with any of these behaviors since he does a good amount of VESC repair.
```

---
## \#16 Posted by: DougM Posted at: 2018-06-10T19:10:19.243Z Reads: 24

```
Agreed.  I think your 5v rail took a full power hit and that caused either your processor or your DRV chip to crumple.
```

---
## \#17 Posted by: L3chef Posted at: 2018-06-10T19:19:16.086Z Reads: 22

```
What brand of lipo are you using?  Your regen is high..
```

---
## \#18 Posted by: Teo Posted at: 2018-06-10T19:33:41.233Z Reads: 21

```
I did  I few more tests this afternoon and the third time I uploaded the new firmware and went through the setup process the vesc started again giving signs of life :slight_smile:

I still haven't figured out what happened but I'm super happy it works again! I just came back now from a 4km ride and it was perfect. No cutoffs even with high acceleration getting quickly up to 30km/h. This is actually the first time I ride with the new firmware and it's much better than the older one (also way more energy efficient!).

Thank you everyone for the tips and trying help me figure out what was wrong with the vesc!!! :slight_smile: 

@L3chef  It's a zippy compact 4500 mAh, 35C, 5S (it was 6s but I had to remove one shell after a crash). Do you think I should lower the regen?
Also i have just ordered 21 Samsung 30Q 18650 3000mAh 15A to build a 7s 3p pack. On that I think I'd probably have to lower it even more?
```

---
## \#19 Posted by: L3chef Posted at: 2018-06-10T19:44:18.658Z Reads: 20

```
This one? https://hobbyking.com/en_us/zippy-compact-4500mah-6s-35c-lipo-pack.html
It's rated at 5c max charge. And you removed one cell. So basically you have 3750mah left. So I would set it to -15 amp.
However. This will make your brakes weaker.
```

---
## \#20 Posted by: Teo Posted at: 2018-06-10T20:28:34.274Z Reads: 20

```
@L3chef Yes that's the one.

I'm not an expert but I believe that if I remove one of the cells I'd just get a lower voltage with the same capacity, so 4500mah at 5C it should be ok with a constant recharging current of 22.5 A. I set it to -30A because I though that, given the 22.5 A constant recharging current, a burst at 30 A for a few seconds while breaking wouldn't hurt the battery pack, but this can be indeed a very wrong assumption... probably much better to lower it to -15 A as you said.

Regarding the breaking wouldn't that be given by the other value in the tab which is marked as "Motor current max brake"? I thought i could still generate a higher breaking current for strong breaking without necessarily making it all flow through the battery.
```

---
## \#21 Posted by: pat.speed Posted at: 2018-06-10T20:46:11.236Z Reads: 17

```
Yes that is correct you would have a 5s 4500mah battery, I would just leave the settings how they are now as the vesc has started working correctly, although lowering the erpm to 60k would be safer
```

---
## \#22 Posted by: L3chef Posted at: 2018-06-11T03:33:00.788Z Reads: 15

```
Yes sry mixed that up. You have an 5ss 4500 battery :)
```

---
