# Installed and tested a Coulometer (&ldquo;fuel&rdquo; gauge)

### Replies: 22 Views: 5041

## \#1 Posted by: RogerD Posted at: 2016-03-10T15:27:20.216Z Reads: 444

```
I've installed a volt meter before but whilst that gives you a real time time pack voltage, it doesn't tell the whole story of remaining range unless the lipo pack has rested and you do some maths.

The Chinese are now selling high current coulometers:

<img src='/uploads/db1493/original/2X/0/017851843671f561d386b92007a88be35b87e845.jpg'>

http://www.ebay.co.uk/itm/Battery-Capacity-Tester-coulometer-Current-Voltage-8-50V-350A-Lithium-Lead-acid-/181954706863?hash=item2a5d587daf:g:9Z0AAOSwwE5WZfCN

I bought the 350 Amp version as my board pulls a peak 100A current, which is way over the next one dwon (50Amps, 100 burst).. Cost me £30 delivered.

This records Mah used (or AH in my case). You set the battery capacity and it decreases as you use the board, and increases as you charge it. Actual Ah used, not guessed - as it's measuring it. I've tested it today and it's bang on accurate. It also calculates charging time, and discharging (riding time).

Firstly, it shows 2Amps going in when on charge. My charger is rates at 2Amps. So that's a good start.

Went for a ride today. I know my board does 12-13 miles on one charge (24Ah) - use 20Ah for safety.

I went 8.66 Miles The screen showed I had 8.17Ah remaining. 34%, 22.9volts (3.83 per cell) with 22 mins esitmated ride time remaining (it works this out as you ride (or when you are charging it to give you a full charge esitmated time). I would aim to ride it down to 15-20% remaining to leave a nice amount still in the packs for safetly/longevity. So if the coulometer is accurate enough, I'd expect to use another  4.Ah to leave it at 4 Ah remaining, which is 17% of my 24Ah pack. I'd probably quit at 4.5Ah/5Ah to add a little safety margin.

If you do the maths that's 0.94Ah per mile. I know I can go 13 miles so If you add the remaining 4.4 miles, multiply by 0.94Ah = 4.14Ah to get me to 13 miles . Take that off the 8.17Ah that shows as remianing capacity. That leaves you...4.03Ah = 17%  = spot on!.

So I can reliably ride knowing that I have from 100% to 20% rideable power. Anything under 20 and I'll get close to hitting my low voltage cut off.

Below: Fully charged

[URL=http://s97.photobucket.com/user/dodgey99/media/General%20pics/2016-03-10%2012.55.29_zpsguo99net.jpg.html][img]/uploads/db1493/original/2X/7/7394beacde5db9d7278b1b0bc02022b1a3a20bdc.jpg[/img][/URL]

<img src='/uploads/db1493/original/2X/5/575e6da8d3c1d1d63f4dfe54e44604df00906336.jpg'>

<img src='/uploads/db1493/original/2X/8/84d9688e3e63cce2e2266ade991c721c930f62e2.jpg'>

And after 8.6 Miles: (and a bit dusty)

<img src='/uploads/db1493/original/2X/3/3c88a4848a500203ef1f533b2bff59c9b7bc4f89.jpg'>
```

---
## \#2 Posted by: mattdig Posted at: 2016-03-10T15:47:06.222Z Reads: 372

```
What batteries are you using for 24Ah? Also what enclosure are you using?

That Cuolometer looks really awesome, way better than the little voltage/balance meter I have on my board.
```

---
## \#3 Posted by: RogerD Posted at: 2016-03-10T16:04:40.090Z Reads: 379

```
2 x 12Ah Multistar 6S packs (hobbyking).

The enclosure is the one that came with the board (it was a Boom Borda - standard Chinese electric skateboard - slow and heavy)

<img src='/uploads/db1493/original/2X/4/46b759a1d62503787b65ceac92e3a4e4b7fa2654.gif'>
```

---
## \#4 Posted by: treenutter Posted at: 2016-03-10T18:26:11.604Z Reads: 369

```
Very cool @RogerD ! I found the same device on eBay for th US. Does the device have a low-voltage alarm? I can't see that it does in the description. Also, any chance you'd share a picture of how you wired the sensor to your battery? I'd love to replace my simple alams w one of these!

Also, I'd really like to see real-time voltage while I'm riding, something I've never been able to measure.

http://www.ebay.com/itm/Capacity-Tester-coulometer-F-8-50V-350A-Lithium-Lead-acid-Battery-Voltmeter-AMP-/111845558246?hash=item1a0a83c7e6
```

---
## \#5 Posted by: RogerD Posted at: 2016-03-10T19:03:05.571Z Reads: 352

```
No alarm I'm afraid, but I use the low voltage cut off on my ESC to do that.

A rough diagram below:

<img src='/uploads/db1493/original/2X/6/63d3eb24257c6702832239b8485065fe0624e8ef.jpg'>

In summary.

Your live(+) goes to the ESC as normal.
Your negative (-) goes through the supplied sensor that comes with the display - then on to your ESC as normal.

The sensor has two small wires that plug into the display. (sensor wires).
You also send positive and negative from the lipo to the display to power it. I toggle the positive with a switch or the screen would be on all the time and kill your battery when not in use. (It remembers Mah usage etc between power cycles.)

The lipo hasn't got 4 connections. It's just the way I drew it.

The only difference with charging is you sent the negative from your charger through the sensor so the display can tell how much you are charging.
```

---
## \#6 Posted by: onloop Posted at: 2016-03-10T23:44:45.965Z Reads: 316

```
NICE, Lots of great info on this screen.
```

---
## \#7 Posted by: Kaly Posted at: 2016-03-11T01:59:43.118Z Reads: 308

```
hello
this is really a nice find :smile:
do you have the instruction for this ?
```

---
## \#8 Posted by: RogerD Posted at: 2016-03-11T07:58:18.034Z Reads: 304

```
My diagram is pretty much  the instructions in picture form. The eBay seller will email them to you.

Three buttons on the back. Used to set the Mah of your battery, and also you can reset the count to either zero or full, if you need to. This would be for if you part used or charged your pack without the screen switched on, so it would have lost track of usage. Then you'd fully charge your pack and reset the display to full.

Update: I charged it with my slow charger (basic charging brick @ 2amps) - through a Hobbyking Amp meter that records total Mah throughput etc. The HK amp meter shows 16.9Ah gone through. Add that to the 8.17Ah that was shown as remaining on the coulometer display and that gives you 25Ah. My battery is 24Ah - so not bad at all for accuracy - bearing in mind my charger probably put an extra 1Ah in overnight trickle charging, as if often the way.
```

---
## \#9 Posted by: RogerD Posted at: 2016-03-11T08:00:46.433Z Reads: 286

```
Incidentally,  they do a 50amp version for around £12. If you are running high voltage,  low current,  then you could get away with that.
```

---
## \#10 Posted by: Kaly Posted at: 2016-03-11T11:25:30.643Z Reads: 289

```
@RogerD thank you very much :smile:
```

---
## \#11 Posted by: Chigzy Posted at: 2016-09-28T18:52:05.908Z Reads: 218

```
Sorry for hijacking this thread, just thought it was more appropriate rather than creating a new one. I've received the 50amp coulometer but I'm confused on how to wire it from reading your diagram. I tried putting negative from battery through it but nothing seems to come through. Like an idiot I tried putting positive and negative through and when I touched the wire on the positive side on jx90 plug it just sparked up. I'm hoping I haven't ruined my battery :(.

Can anyone shed some light for me please


<img src="/uploads/db1493/original/3X/4/7/479aaf1d9906d9cc52ca0987ca3a6f6dbf692d1e.jpg" width="689" height="390">

<img src="/uploads/db1493/original/3X/b/7/b704b3a98ed457fec52bdfb3e2385e754ecf70cd.jpg" width="282" height="500">
```

---
## \#12 Posted by: RogerD Posted at: 2016-10-01T08:45:09.758Z Reads: 191

```
Don't worry,  your battery will be fine. You just shorted it briefly. Whether your coulometer is ok is a different matter. Probably ok as you just put power into the current sensor.

On your current sensor there is p- and b-.   (the screw terminals).  Ignore the p- and B- on the larger circuit board,  these are for lower current.

P- is power - negative.     For your esc.
B - Is battery - negative.   For your battery

So battery positive goes to your esc as normal. 
Battery negative goes to B-. Then out of P- to your esc.

You then need to provide power to the actual coulometer circuit board. I don't have your wiring diagram but at a glance, the Green screw terminal on the current sensor board has B+ written near it which suggests battery positive. Just a small wire will do there. Your coulometer will then be able to take + and - from the sensor board to power itself.
```

---
## \#13 Posted by: Chigzy Posted at: 2016-10-03T17:13:41.858Z Reads: 189

```
Hey thanks for the help. Managed to wire it up and it seems to have some life, however the screen is stuck on the below. When I try pressing the buttons on the back it just only gives me these 2 options. Not sure if I have damaged it from earlier.

<img src="/uploads/db1493/original/3X/5/3/53c720b7ff8f5f506ea02904af562782f7adfb62.jpg" width="282" height="500">

<img src="/uploads/db1493/original/3X/5/4/54de8758a87e17d190bfdcb26c6ded0b077778d2.jpg" width="689" height="390">
```

---
## \#14 Posted by: Chigzy Posted at: 2016-10-03T17:48:06.204Z Reads: 187

```
Ok. So figured out how to change the capacity but there's some settings I'm not sure what to set as.
<img src="/uploads/db1493/original/3X/4/8/48c47705cce02a1ea2d5e1096f8ba2e9fcafa0e7.jpg" width="689" height="390">
<img src="/uploads/db1493/original/3X/0/c/0c5ffde56e98853e4086089fa81966a026c2ddbd.jpg" width="689" height="390">

<img src="/uploads/db1493/original/3X/9/a/9a61678cab9dafbe2c79fd5e23e533224aa6c0a1.jpg" width="689" height="390">

<img src="/uploads/db1493/original/3X/9/5/9541e0693357ec87b66a2249c532c058bd89038e.jpg" width="689" height="390">

Sorry if I'm being dumb. Also when it's connected, it seems to just stay on 100% 8ah which is my bat cap, but doesn't go down.

Also I want the led screen to stay lit, it seems to flash on and off whilst power doing through.

Thanks a bunch for all the help
```

---
## \#15 Posted by: RogerD Posted at: 2016-10-03T22:30:09.496Z Reads: 163

```
Leave all the screens alone except cap. That is where you set your batter Mah. The rest you should not touch.

holding one button  resets it to full, one to empty. It flashes when you are charging the battery pack. It stays lit solid when in use ( battery is being drained). 

Did you not get any instructions?
```

---
## \#16 Posted by: Chigzy Posted at: 2016-10-04T06:07:40.874Z Reads: 163

```
Hi, Unfortunately no as I bought it from ebay and they did not send anything but the boards. 
I think I may have changed some of the settings on the others. Is there anyway I can set it back to default then just change the Cap settings and leave the rest. Sorry dude for the dumb questions. 

This is going to look sick once I've made my carbon deck. Going to integrate it into the nose and hopefully have the screen between the truck bolts.
```

---
## \#17 Posted by: RogerD Posted at: 2016-10-04T21:02:11.918Z Reads: 152

```
No idea I'm afraid.
```

---
## \#18 Posted by: DougM Posted at: 2016-10-04T22:11:21.178Z Reads: 153

```
Has anyone cracked this thing open to see what chip it is using?
```

---
## \#19 Posted by: Lambjr088 Posted at: 2017-05-03T02:01:39.351Z Reads: 124

```
Ive tried looking this item up as well from the brand name on it "Baiway"  but only seem to find on a different version as i have the bw-tf02 v.1 i downloaded a file that is similar but not the exact one. Bw-tf01 no luck since i cant figure out the wiring
<img src="/uploads/db1493/original/3X/9/8/98b1454cfb97c7b8b8912a9526f26f6068da75b8.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/a/2/a2de1d8b9f6152cb096e271eddcc76fba361b1c9.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/b/7/b7d6b1ebabe64bcb6e3edaa417b511cba53f9409.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/1/9/19a4c633388a3b01711aebddeb89c594c3fb276d.jpg" width="281" height="500">
```

---
## \#20 Posted by: Lambjr088 Posted at: 2017-05-08T17:09:42.835Z Reads: 101

```
http://115.28.16.44:81/file/3519.pdf
This is a diagram to wire lol forgot to mention it before
```

---
## \#21 Posted by: Okami Posted at: 2017-05-09T18:34:27.368Z Reads: 88

```
@Lambjr088  Good that this crazy link has a pdf extension at the end :D otherwise im not sure I would click on it :D
```

---
## \#22 Posted by: Lambjr088 Posted at: 2017-05-09T19:23:00.006Z Reads: 86

```
Yea i just updated it forgot to mention it hahahaha
```

---
