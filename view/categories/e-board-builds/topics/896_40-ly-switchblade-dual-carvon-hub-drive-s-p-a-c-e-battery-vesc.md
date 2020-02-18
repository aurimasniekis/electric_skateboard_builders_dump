# 40&rdquo; LY Switchblade &#124; Dual Carvon Hub Drive &#124; S.P.A.C.E Battery &#124; VESC

### Replies: 20 Views: 4083

## \#1 Posted by: OGP Posted at: 2016-01-03T22:22:28.290Z Reads: 255

```
After lurking on a few differed forums, I've decided to make this one my home.  So hello!

I'm an old engineer / downhill snowboarder that's fed up with parking prices in the Bay Area.  My main inspiration is to lessen my commute but also to tinker out of curiosity.  So far I've ordered my deck and hub motor from Carvon and planning on going with the SPACE battery, x2 VESC.

I'm still considering which options would be good for remote.  I'll post pics / videos as I begin my build.. and probably way too many stupid questions.
```

---
## \#2 Posted by: psychotiller Posted at: 2016-01-03T22:49:07.552Z Reads: 249

```
Welcome to the forum! Good luck on your build
```

---
## \#14 Posted by: OGP Posted at: 2016-01-05T07:54:09.119Z Reads: 241

```
Also, what is the preference, in general, of people mounting their components?  Screw directly to the board, then drop an enclosure over it or let the enclosure catch it?  Seems like a good idea to mount it because of vibration from the road?

The enclosure is a whole other project in itself if I go CF.  This thread is amazing:
http://www.electric-skateboard.builders/t/how-do-you-lay-carbon-fiber/214/38

All I can think is "OMG carbon fiber is so cool".  ABS looks pretty cool too:
https://www.youtube.com/watch?v=hGBRiYhxRTM
```

---
## \#3 Posted by: onloop Posted at: 2016-01-06T03:57:50.155Z Reads: 190

```
16 posts were split to a new topic: [Good Radio Transmitter Hand Controller for use with DIY Electric Skateboard](/t/good-radio-transmitter-hand-controller-for-use-with-diy-electric-skateboard/928)
```

---
## \#15 Posted by: onloop Posted at: 2016-01-06T03:59:11.827Z Reads: 210

```
Sorry @OGP your build thread got mega hijacked... all the talk about radios is now in its own topic.
```

---
## \#16 Posted by: psychotiller Posted at: 2016-01-06T04:19:15.631Z Reads: 206

```
http://www.electric-skateboard.builders/t/making-your-own-vacuum-forming-set-up-cheap/126
```

---
## \#17 Posted by: OGP Posted at: 2016-01-06T05:09:26.876Z Reads: 202

```
hah it's ok.  I think it's very amusing :sunny:
```

---
## \#18 Posted by: OGP Posted at: 2016-02-15T04:50:56.358Z Reads: 195

```
I was able to get some basics functioning so far:

https://www.youtube.com/watch?v=ZLRcI20WSy0

Next steps I'll be working on flashing my other VESC and wiring the bus.  Still thinking about what I might do for my enclosure..
```

---
## \#19 Posted by: OGP Posted at: 2016-02-24T01:04:33.854Z Reads: 185

```
https://www.youtube.com/watch?v=hGD4jJuWesc

I've wired my CANBUS and configured my forwarding via BLDC for the Kama controller.  Having an issue with dropped signal possibly or power fluctuations.  I haven't tested with keyboard to see if it's consistent but I strongly suspect the Kama remote / receiver combo.  Everything is soldered in as recommended but perhaps it's something else.

Also, once I finalize some of my power settings, I'll share them.
```

---
## \#20 Posted by: SpartanScrub Posted at: 2016-02-24T02:22:23.379Z Reads: 193

```
Had the same problems with my Kama remote testing out my board last week. On the bench test like you are doing it actually worked completely fine though. It wasn't until the board had a load on it and was going >15mph the controller decided to have a mind of its own accelerating and braking. Pretty scary stuff, sent the board flying into the curb after I bailed a couple times haha

Probably totally talking out of my ass right now, but could the drop outs have anything to do with the receiver being so close to the motor? It's a giant magnet so I figured it might mess with the signal somehow. Wasn't till after I was done riding I realized I had the transmitter right next to the motor and noticed yours is pretty close to a motor too. Wasn't able to test it myself with the transmitter on the other side of the enclosure since I blew a battery in the process but that's been my theory.
```

---
## \#21 Posted by: mostwanted Posted at: 2016-02-24T09:56:00.089Z Reads: 185

```
@OGP . 

in video we all can see clearly that the USB is still connected to VESC . and is USB is still connected to computer ?

i'm not sure .  but  some earlier  VESC  videos i've seen , most of them saved , reboot and power off . disconnect USB . and switch on eboard and nun chuck . 

try to disconnect USB after saved programming .
```

---
## \#22 Posted by: lowGuido Posted at: 2016-02-24T10:12:47.618Z Reads: 176

```
That doesn't look like a kama problem to me. That looks like something else. I have never seen a kama drop like that.

Does the light go out on the kama when it drops?

I think there is a lot of misinformation out there about the kama. I have had 6 different nyko kamas and over 800km of skating and only time i get droppouts is when the batteries in the nunchuck are low.
```

---
## \#23 Posted by: mostwanted Posted at: 2016-02-24T10:57:34.813Z Reads: 168

```
true ! low batt on kama . me too .
```

---
## \#24 Posted by: OGP Posted at: 2016-02-24T19:25:13.506Z Reads: 173

```
The USB was disconnected from BLDC.  Same results with and without USB connected, rebooted with USB disconnected, etc.
```

---
## \#25 Posted by: OGP Posted at: 2016-02-24T19:30:23.865Z Reads: 183

```
I'll have a closer look tonight but so far everything is equally possible given my observations so far.  I'm only going on a hunch that the problem is somehow related to controller communication but that's not a fair conclusion without more data.  Thanks for your help so far!
```

---
## \#26 Posted by: OGP Posted at: 2016-02-25T23:53:48.684Z Reads: 179

```
Here's another update with my power problems:

https://www.youtube.com/watch?v=AJebYl7d4GU

The mounting is a reference as I finalize the layout and try to debug some of the settings on the VESCs.  It's super handy to use cheap velcro tape but ultimately, I will go a different route after more thought.

The controller / receiver seem solid.  I could test with a meter to see if it's truly a problem but when the power cuts out, I see the lights flash on the VESCs, with the power remaining constant on the receiver.  I also haven't done a motor detection yet and definitely need to read up on properly provisioning beyond the recommended SPACE battery settings I have set.
```

---
## \#27 Posted by: sgaana Posted at: 2016-02-26T06:15:26.051Z Reads: 170

```
Instead of Velcro, consider 3M Dual Lock Fastener SJ3650.
```

---
## \#28 Posted by: delta_19 Posted at: 2016-03-09T12:49:53.330Z Reads: 164

```
I would suggest against that. It's great for holding stuff to the wall but the moment it vibrates it losses all strength
```

---
## \#29 Posted by: LukeM Posted at: 2016-04-05T20:02:26.314Z Reads: 150

```
Any conclusions/solutions on what was causing the drops?
```

---
## \#30 Posted by: Eboosted Posted at: 2016-12-12T05:38:37.618Z Reads: 80

```
Did you ever fix this problem?
```

---
