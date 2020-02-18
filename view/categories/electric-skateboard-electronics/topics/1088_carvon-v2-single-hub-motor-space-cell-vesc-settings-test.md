# Carvon V2 Single Hub Motor &#124; Space Cell &#124; VESC Settings Test

### Replies: 27 Views: 5406

## \#1 Posted by: RunPlayBack Posted at: 2016-01-24T02:53:40.182Z Reads: 282

```
So I had a chance to get some riding in yesterday and was able to optimize some of my VESC settings for the Carvon Single Hub V2 motor + Enertion Space Cell with the help of @chaka and @onloop. I can't conduct range tests at the moment because the weather is too cold but speed is easy.

First I used recommended VESC settings for the Space Cell:

Motor Max: 80.00
Motor Min: -60.00
Bat Max: 30.00
Batt Min (Regen): -12.00
Absolute Max: 130.00

1st ride had FOC enabled and while it was a super smooth and a quiet ride, my top speed seemed to be capped at around 18mph which felt safe, but slow. The stealth of the Carvon hub is pretty sweet. Along with a 29" deck size and FOC, I attracted very little attention. At the moment FOC feels like incognito mode. There are times, especially traveling through the city, when I won't go past 18mph and I want to attract as little attention as possible.

2nd ride I had BLDC enabled, much noisier, but performance is beefier. I hit a top speed of 27mph before I got the speed wobble and chickened out. Pretty sure I could have gone 30mph+. Also noticed the VESC would back off after hitting the brake at max speed which is a little scary with the coasting ability of the hub motor. I definitely attracted more attention with this setting. However, the Carvon hub noise compared to the E-GO belt drive noise is way less obnoxious and kind of a pleasant whirring.

3rd ride I had BLDC enabled but changed the Space Cell settings to:

Motor Max: 50.00
Motor Min: -30.00
Bat Max: 30.00
Batt Min (Regen): -12.00
Absolute Max: 130.00

Hit a top speed of 21mph, definitely could have gone faster but was being conservative. Brakes seemed to be more responsive and didn't notice any cut outs. I believe this setting is probably the best all purpose setting for the Carvon V2 Single Hub + Space Cell + VESC.

I'd love to compare settings with anyone else using this combo but I'm definitely satisfied that I can hit 27mph+ on a single hub.

<img src="/uploads/db1493/original/2X/4/480a103e0d9dabce791bb100ac2a2f4894167835.jpg" width="500" height="500">
```

---
## \#2 Posted by: chaka Posted at: 2016-01-24T03:09:02.139Z Reads: 257

```
NIce! Thank you for sharing your parameters. 

Remember that asphalt will eat you at 27mph and a little potato chip like that will buck you off pretty quick.
```

---
## \#3 Posted by: RunPlayBack Posted at: 2016-01-24T03:22:54.690Z Reads: 253

```
Trust me I won't go near those speeds anytime soon unless its some kind of defensive escape maneuver. Last time I wiped out was 13mph on the E-GO and while it wasn't serious, it wasn't fun at all. Safety always.
```

---
## \#4 Posted by: Jeff Posted at: 2016-01-24T23:02:58.902Z Reads: 234

```
Not sure what bushings you use but to deal with speed wobbles I put venom double barrels on my boards. You can customize them to your weight and it can really improve your stability at speed.
```

---
## \#5 Posted by: RunPlayBack Posted at: 2016-01-25T02:20:38.215Z Reads: 223

```
I'm using whatever came with the Carvon hubs. I'll definitely look into the Venom double barrels. Looks like 85a is the right size for my weight. Will these fit on the Carvon trucks? http://www.carvonskates.com/store/p4/CarvON_V2_Single_Hub_Motor___Matching_Front_Truck___Wheels_Set.html
```

---
## \#6 Posted by: chaka Posted at: 2016-01-25T02:24:52.571Z Reads: 214

```
Should fit perfectly. I like to use soft bushings up front to keep it twitchy and just run a hard bushing board side on my rear truck leaving the roadside bushing soft. This gives me stability when going straight but still allows for deep carving when needed.

Try to find a balance. Too stiff and you may not be able to avoid something you wish you could have.
```

---
## \#7 Posted by: RunPlayBack Posted at: 2016-01-25T03:44:53.823Z Reads: 213

```
Good call I'll pick some up to smooth out the ride. BTW here's some footage of me doing the speed wobble dance on the rock salted streets of Detroit today :wink:  
https://www.instagram.com/p/BA8SXWFNHku/?taken-by=rikcordero
```

---
## \#8 Posted by: chaka Posted at: 2016-01-25T04:41:13.782Z Reads: 200

```
Can't help but smile when riding an eboard! Really makes my day when I see ride videos from patrons!
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-01-25T18:43:13.736Z Reads: 198

```
@RunPlayBack   venom double barrels are the trick for sure to eliminate speed wobbles. i have a Bustin YOFACE double kick (6S LiPo with dual PropDrive 270s) with a much shorter wheelbase than a Scarlet and I keep double barrels on it. Wobbles are a thing of that past on that board. 

But Scarlet seems to give no shits about wobble. I'm running stock barrel and cones (came with the caliber IIs) on that deck and speed wobble just doesn't seem to happen. Of course a 27" wheelbase might have something to do with it, and i do have my cones tightened down to about 4 threads, and that w-cave keeps my feet cozy while carving hard and suddenly, but I also have yet to max it out. So far i've only taken it up to about 26mph.
```

---
## \#10 Posted by: broshi Posted at: 2016-01-26T01:49:31.268Z Reads: 191

```
Sweet finally some specs coming out for the hub motors. 
I was just wondering, how did the single handle hills?
```

---
## \#11 Posted by: RunPlayBack Posted at: 2016-01-26T02:29:17.587Z Reads: 183

```
Didn't really hit many hills yet but I'm assuming I'd need a good amount of top speed to climb anything steep. For where I live and my usage, I'm okay with compromising a little torque for the stealth and coasting ability.
```

---
## \#12 Posted by: RunPlayBack Posted at: 2016-01-26T02:38:08.542Z Reads: 174

```
Cool just got the Venoms :) Yeah not much WB clearance on my 29" deck so that speed wobble might not be something I can completely avoid but we'll see once I test the Venoms. For now I think this build is best served for 10-18mph daily commuting in the city where I can maneuver easier and be super stealthy. Seriously that FOC in a crowd makes it feel like it's totally disguised from being electric.
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-01-26T14:29:29.970Z Reads: 164

```
So FOC has clearly affected your top speed, which in your use case isn't an issue, and it seems like some other benefits make it worth it. Has it affected your range?
```

---
## \#14 Posted by: RunPlayBack Posted at: 2016-01-26T14:44:24.301Z Reads: 165

```
Haven't truly done any range tests just yet but I found the perfect spot to try it soon. I'm assuming that the FOC is more efficient in my startup and it feels like the hub motor coasts better than BLDC if that makes sense. I think because there isn't any noise, I'm also more mentally aware of my coasting capabilities and balancing out smooth, controlled bursts of speed with some kick push. I dig both though, FOC in the city and BLDC in the country.
```

---
## \#15 Posted by: psychotiller Posted at: 2016-01-26T14:49:25.187Z Reads: 167

```
We need to get on an app for android and Apple.
```

---
## \#16 Posted by: RunPlayBack Posted at: 2016-01-26T15:12:05.699Z Reads: 173

```
Yeah that would be sweet. Even just having input parameters for parts would be helpful so your summary ride would have everything neatly listed along with speed / elevation / distance stats. I actually work with an engineer / skater buddy who might be able to help us.
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-01-26T15:52:44.798Z Reads: 171

```
we need an app that can let the device display info from and write configurations to the VESC. 

And there needs to be an rpm/mph/kph trip meter display right on the front screen.  

I don't even care if its wireless. If i have to tether with a weird usb/lightning cable so i can log info on my iphone than so be it.
```

---
## \#18 Posted by: RunPlayBack Posted at: 2016-01-26T16:09:24.531Z Reads: 170

```
When I had my Miniquad FPV, there was an android app called [EZ-GUI Ground Station][1] which was able to connect to the flight controller for real time data and to change up settings on the field instead of whipping out a laptop but you still had to connect via USB. For my camera gimbals there's a [SimpleBGC app][2] that allows you to connect to the gimbal through bluetooth to change settings, control the camera through a virtual joystick and view realtime data. Pretty sure one or both of those options would be possible with the VESC.


  [1]: https://play.google.com/store/apps/details?id=com.ezio.multiwii&hl=en
  [2]: https://www.basecamelectronics.com/downloads/android/
```

---
## \#19 Posted by: chaka Posted at: 2016-01-26T16:12:49.509Z Reads: 167

```
Let me know if you get any under voltage errors on FOC. If you do, there is a hardware mod to rectify the issue.
```

---
## \#20 Posted by: psychotiller Posted at: 2016-01-26T18:17:12.860Z Reads: 169

```
I would be happy with just being able to make field adjustments and record trip data.
```

---
## \#21 Posted by: lox897 Posted at: 2016-01-26T20:52:34.185Z Reads: 157

```
Didn't vedder or someone else start up a thread for an android app on ES?
```

---
## \#22 Posted by: longhairedboy Posted at: 2016-01-27T01:28:02.763Z Reads: 156

```
ok this is going to sound really weird but i just got off the phone with some people affiliated with a local university and they want to build thier own vesc and write apps to talk to it. they want to build a 12v solar powered electric skateboard (i know, i know) and collect data from it. 

anyway i'll report back about the app portion of it when i gather more intel.
```

---
## \#23 Posted by: psychotiller Posted at: 2016-01-27T02:03:43.044Z Reads: 151

```
They must be listening in to our conversations! :confused:
```

---
## \#24 Posted by: cmatson Posted at: 2016-01-27T02:41:54.434Z Reads: 159

```
[quote="longhairedboy, post:22, topic:1088"]
they want to build a 12v solar powered electric skateboard
[/quote]

never seen that before, I hope they make it look cool :laughing:
```

---
## \#25 Posted by: longhairedboy Posted at: 2016-01-27T02:59:19.474Z Reads: 160

```
i know! i mentioned that i knew somebody that did this already and also 12V... its going to crawl. But i don't think their objective has anything to do with a finished rideable ... tolerable... product. I think its a data mission.
```

---
## \#26 Posted by: RunPlayBack Posted at: 2016-01-27T03:53:08.453Z Reads: 159

```
Awareness is always a good thing, for science! Hopefully they share their data
```

---
## \#27 Posted by: Esrapp21 Posted at: 2016-12-12T02:04:18.711Z Reads: 79

```
I'm about to make a build pretty much exactly like this one. Did you ever happen to find out the range on FOC @RunPlayBack?
```

---
