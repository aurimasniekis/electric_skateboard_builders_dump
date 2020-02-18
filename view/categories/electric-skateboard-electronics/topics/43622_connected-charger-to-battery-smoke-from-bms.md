# Connected charger to battery smoke from bms

### Replies: 13 Views: 749

## \#1 Posted by: Acido Posted at: 2018-01-13T16:12:53.397Z Reads: 97

```
This is not the first time but this time something went wrong

I plugged in my charger heard some small pops it was hot around the balance plugs but nothing is burned

All the wires as i can see are connected properly but the balance wires are connected bearly the cable is shot waiting for a longer one could that be a problem?

Anyone had this problem?
```

---
## \#2 Posted by: Acido Posted at: 2018-01-13T16:16:05.879Z Reads: 96

```
Again when i connect it smoke comes and its ho
Maybe a short?
```

---
## \#3 Posted by: Acido Posted at: 2018-01-13T16:25:39.525Z Reads: 91

```
My 10th balance wire is somehow not connected could that be a reason?
```

---
## \#4 Posted by: Martinsp Posted at: 2018-01-13T16:26:24.121Z Reads: 90

```
Measure the voltages with one probe on the negative power terminal (not balance connector) and go through each hole on the balance connector. The voltages should increase in the same intervals from one side and decrease from the other. Do the same with the probe on the positive power terminal. This way if it all looks OK you can rule out the battery and proceed with the BMS, send pictures of it.

And just to make sure you dont damage anything dont use the BMS until you fin out what it is.

Yes that could be a problem but I had this problem with my BMS and mine just did not len current through it did not smoke.
```

---
## \#5 Posted by: Acido Posted at: 2018-01-13T16:33:41.103Z Reads: 83

```
Figoured it out my genious ass connected the 10th balance wire as a charger wire...hope i didnt burn out my bms

Bestech please have this type of protection!!!
```

---
## \#6 Posted by: Acido Posted at: 2018-01-13T17:07:12.534Z Reads: 77

```
Now its stuck on on position
Vesc is on altough the wires are disconnected
I will see with bestech what they can do
```

---
## \#7 Posted by: Acido Posted at: 2018-01-13T17:17:13.199Z Reads: 71

```
So i cut the negative wire from bms to vesc and now to check if vesc works i took a thin wire and like bridged the cables like battery negative -thin cable - vesc negative

And it sparked it never did that before battery is li ion so it shouldnt spark as I know
Please someone help fast its not easy to be in this position!!
```

---
## \#8 Posted by: Martinsp Posted at: 2018-01-13T17:30:17.395Z Reads: 63

```
It sparked because the capacitors were charging, that is normal.
```

---
## \#9 Posted by: Acido Posted at: 2018-01-13T17:38:36.958Z Reads: 62

```
I left it connected for a few seconds and there was no light.. What could it be
```

---
## \#10 Posted by: Martinsp Posted at: 2018-01-13T17:59:20.705Z Reads: 59

```
Disconnect it and check with multimeter all the power lines against ground. Most probably one of them will be shorted. 
And make sure the VESC was getting power since the bms is questionable at this point. Ideally try with different power source but only if the main power leads on the vesc are not shorted so that you don't short your battery or powersupply
```

---
## \#11 Posted by: Acido Posted at: 2018-01-13T18:13:40.890Z Reads: 55

```
I was connecting it directly to the battery this time
Without the bms

While i was cutting the battery wire thst went to the bms i heard a pop and if i remember well the vesc just turned off 

Also I dont have any other power supply than my battery thats compatible with vesc only got 2 car battery chargers so thats 24v wich could work if its possible to connect those two together to get 24v

I will look up how to check it aggaints ground and try that on monday
```

---
## \#12 Posted by: Martinsp Posted at: 2018-01-13T18:18:04.631Z Reads: 56

```
Don't try it with the chargers, battery directly is enough since the point was to make sure the bms wasn't preventing the vesc from turning on. You just measure resistance between ground and positive terminal input on the vesc, 5V on for example the hall sensor connector, and 3.3v on for example the programing header.
```

---
## \#13 Posted by: Ethanstone Posted at: 2018-04-30T19:36:29.669Z Reads: 23

```
Hi, 
What happened to @Acido happened to me but instead of having a small pop and being hot it when into flames. This is the configuration that I had when it went into flames:
![IMG_0669|375x500](upload://caGFtgNw6rEVEnNpCnrMjpiUwHq.JPG)

Here is the schematic of the BMS I had: 
![22 PM|690x239](upload://aDhCel1fnUspoHBgA8zF2G710iP.png)

Is the wiring wrong? Did I get the wrong BMS?
Thanks
```

---
