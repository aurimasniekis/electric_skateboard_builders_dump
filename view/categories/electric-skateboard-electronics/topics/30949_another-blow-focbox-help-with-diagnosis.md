# Another blow Focbox, help with diagnosis

### Replies: 22 Views: 1764

## \#1 Posted by: Eboosted Posted at: 2017-08-18T07:06:57.507Z Reads: 197

```
I thought these things were more robust but it seems they are not. 

I bought 4 Focboxes for my Trampa, 2 for immediate use and the other two for spares.

Right off the box, the first Focbox threw an overcurrent fault when I pulled the trigger at full throttle, the scary part was during the error the Focbox kept the board at full speed, no response from the remote for 3 seconds, pretty scary feeling. That VESC is already back to Enertiin fir warranty. 

The second Focbox died on me while braking 4 days ago, only one wheel was spinning slowly on full throttle. The bad VESC wheel had resistance if I turn it by hand, so I unplugged each of the three phase cables one by one, when unplugging the center phase cable the motor was released and it brake when I plugged back in.

Can anyone help me finding the culprit of the second VESC issue?
```

---
## \#2 Posted by: scepterr Posted at: 2017-08-18T07:12:47.179Z Reads: 193

```
Does it power on? Get any faults in bldc tool?
```

---
## \#3 Posted by: Eboosted Posted at: 2017-08-18T07:15:07.821Z Reads: 185

```
Yes it powers on but there are no signs of blown electronics. 

Tomorrow I'll look for errors on bldc tool
```

---
## \#4 Posted by: scepterr Posted at: 2017-08-18T07:16:06.755Z Reads: 177

```
Opened it up?
```

---
## \#5 Posted by: Eboosted Posted at: 2017-08-18T07:17:53.868Z Reads: 178

```
Yes I'll upload pictures tomorrow as well. 

Thanks for replying!
```

---
## \#6 Posted by: Namasaki Posted at: 2017-08-18T07:26:17.547Z Reads: 176

```
Are these the new Focboxes from China with the 14 awg phase wires and 3.5mm bullets.
Also can you please share the specifics of the setup and bldc settings?
```

---
## \#7 Posted by: Maxid Posted at: 2017-08-18T07:30:35.487Z Reads: 176

```
They come from china now? 
Didn't the US version also come with that wire and connectors? I don't think they ever had a different configuration.

@Eboosted doesn't a short like that mean a Mosfet failed? If so you might be able to fix it yourself as they are easier to replace than a DRV.

Edit: ah well they are directFETs - so probably not easier to do by hand :(
```

---
## \#8 Posted by: scepterr Posted at: 2017-08-18T07:31:22.917Z Reads: 173

```
Mine is, got it a little over a month ago<img src="/uploads/db1493/original/3X/e/9/e9cf70573466f41e23d123b79be117f38922329d.jpg" width="666" height="500">
```

---
## \#9 Posted by: scepterr Posted at: 2017-08-18T07:34:56.904Z Reads: 171

```
@Maxid DRV takes 10 minutes to replace with a cigarette break in the middle :grin:
```

---
## \#10 Posted by: Eboosted Posted at: 2017-08-18T07:37:03.572Z Reads: 173

```
These are the ones, why do you ask? 

http://i.imgur.com/uutj6mi.jpg
```

---
## \#11 Posted by: Maxid Posted at: 2017-08-18T07:37:36.253Z Reads: 171

```
If you have a reflow oven - with just the standard tools it is trickier
```

---
## \#12 Posted by: scepterr Posted at: 2017-08-18T07:38:13.749Z Reads: 168

```
Those are the old vescx, what's the hw version on the PCB?
```

---
## \#13 Posted by: scepterr Posted at: 2017-08-18T07:39:05.257Z Reads: 168

```
I don't use ovens, just hot air station and IR board heater
```

---
## \#14 Posted by: Maxid Posted at: 2017-08-18T07:39:56.983Z Reads: 167

```
Then you have good soldering skills and a steady hand - where are you from exactly ;)
```

---
## \#15 Posted by: scepterr Posted at: 2017-08-18T07:42:39.290Z Reads: 168

```
NYC, I run a repair shop, after replacing 1000s of iPhone logic board ICs, anything on the vesc I can do half asleep lol
Sadly I got the focbox thinking it had some magic sauce that made it worth the premium and I thought I could rely on the warranty. After mine took a dirt nap and I diagnosed and repaired it myself I realized I shouldve just made one myself :confused:
```

---
## \#16 Posted by: Namasaki Posted at: 2017-08-18T07:52:49.215Z Reads: 176

```
I can relate to that, 
After 40+ years of welding and the last 20 years welding SS pipe, I can almost do it half asleep.
```

---
## \#17 Posted by: toma Posted at: 2017-08-18T08:43:14.231Z Reads: 171

```
If the 3.3v pin is shorted with the GND pin then you've blown the canbus transceiver.  Just use a multimeter to check this.
You can blow that part when you are using two vesc-x/focboxes connected by canbus and power them on/off one by one. 
To avoid this you must power both vesc-x/focboxes on at the same time. I highly suggest that you make a cable to connect the two in parallel.

To repair this you'll need to replace the canbus transceiver. 

<img src="/uploads/db1493/original/3X/0/6/06895c7cfe426a6fde3fdcbe7c8ff85a5e382f6f.jpg" width="320" height="320">

<img src="/uploads/db1493/original/3X/c/9/c9ffbe6adf001e5bc215d80241e97601fd5ce714.png" width="212" height="180">
The P/N is SN65HVD232DR and I ordered my replacements from [mouser](http://ca.mouser.com/ProductDetail/Texas-Instruments/SN65HVD232DR/?qs=%2fha2pyFaduiSwNSNMapJZOp5DAyrO2K%2fCQstQslsB94obQk%2fsWfaHA%3d%3d). 

I used an "smd rework station" to replace the chip.
https://3.imimg.com/data3/AB/JQ/MY-13060832/hot_air_bga_smd_rework_station_quick-500x500.jpg

After replacing the part you should be good to go. It's a pretty tricky repair job to do it correctly, and it's really easy to fuck your boards up and make them completely unrepairable.
```

---
## \#18 Posted by: deucesdown Posted at: 2017-08-18T19:17:31.168Z Reads: 146

```
https://www.absolutesci.com/store/prodimages/S484-207-1AD.JPG

Wouldn't something like this be easier for the CAN chip?
```

---
## \#19 Posted by: scepterr Posted at: 2017-08-18T19:19:46.435Z Reads: 147

```
Hot air station is best, a regular soldering iron will work just fine too. Those tweezers are not for smd work.
If you really want tweezers then these
<img src="/uploads/db1493/original/3X/1/4/14d139b82cff1278b0841fa8f3e54ee4a38375c5.jpg" width="690" height="388">
```

---
## \#20 Posted by: MontPierre Posted at: 2017-08-20T08:35:34.398Z Reads: 117

```
I have a short on 3.3V line on my maytech vesc. And I do have smd rework station but never used it. Do you think by watching few YouTube videos I should be able to preform procedure myself ? Im kind of scared haha.
```

---
## \#21 Posted by: scepterr Posted at: 2017-08-20T08:43:59.521Z Reads: 112

```
I don't see why not. Get a few smd project boards off eBay for practice. Make your own voltmeter/clock/thermometer in the process 😁

Ton of these for a few bucks http://www.ebay.com/itm/232218671232
http://m.ebay.com/itm/SMT-Waveform-Generator-Full-SMD-Multi-Channel-Suite-DIY-Kits-Solder-Test-/391772357333
```

---
## \#22 Posted by: MontPierre Posted at: 2017-08-20T08:54:03.199Z Reads: 110

```
Great idea! I shall practise first! If I get it to work I will be over the moon 💪🏻
```

---
