# First time build 6374 single drive

### Replies: 12 Views: 1339

## \#1 Posted by: Strykerpm Posted at: 2018-02-28T03:20:30.131Z Reads: 181

```
Hey I have had a pre built board for a bit. I am about to build my own. I have done a far amount of research so far.  I would love some real world experiance and input any and all is welcome. I will outline what I think I have narrowed it down to.  I want a decently fast and powerful board nothing record breaking but sold. Motor wise single motor 6374, been looking at torque board and maytech as possible options?  battery 10s2p or 12s2p possibly 3p 4 p seems like alot of batteries and although range is important 15 miles plus would be great. VESC for the speed controller. is there a difference between all the different people selling VESCS? these are the most important areas I would like input in the deck wheels and such seem to come down to preference.  So if you have any suggestions or input i.e. best place to buy batteries oh 25r or 30 Samsung batteries?  I hope to narrow things down and get to building a board soon. Thank you in advance for any and all help, I will be continuing on in my search on this forum and across the web. Btw in Phx Az if that helps in recommending suppliers.
```

---
## \#2 Posted by: mmaner Posted at: 2018-02-28T03:23:36.692Z Reads: 177

```
I'd you are using a battery pack made with 30qs get at least a 3p, if 25rs 5p or better. You will avoid massive sag and get better range. For I fo in wheels and pulleys and trucks, etc. go take a look at the builds category, you'll find a metric frap ton of info.
```

---
## \#3 Posted by: Strykerpm Posted at: 2018-02-28T03:28:03.963Z Reads: 168

```
Yeah not to worried about the small stuff mainly the battery, motor and speed controller. I can make and assemble the battery I just dont have a ton of knowledge on the different types. I know they need to be high output.
```

---
## \#4 Posted by: mmaner Posted at: 2018-02-28T03:31:15.803Z Reads: 166

```
You want at least 30la constant & 60a burst, better is 40/80. The Samsung 30qs support 20a per cell, so at 3p you have 60 burst. At 4p you have 80 burst.
```

---
## \#5 Posted by: mmaner Posted at: 2018-02-28T03:33:44.310Z Reads: 157

```
Motors are easy, talk to @torqueboards or @JLabs about 6374s, the TB 6374s are 20 bucks off right now.   I made a thread this afternoon with the discount code. 

If you can find a FocBox that's the way to go, but they are backorder led for another month or so.  @torqueboards makes a solid VESC.
```

---
## \#6 Posted by: Battosaii Posted at: 2018-02-28T03:50:34.965Z Reads: 144

```
I heard @JLabs has 6384s I'd go with one of those if I was going with a single drive.
```

---
## \#7 Posted by: Strykerpm Posted at: 2018-02-28T04:26:37.725Z Reads: 140

```
what are the benifits of an FocBox over a VESC? The wait could be tough lol but if it worth it might able to. My main goals are cruising distance with the option of going high 20s low 30s mph wise mostly city but Phoenix is pretty flat with straight roads for i conditions are good you can move.
```

---
## \#8 Posted by: mmaner Posted at: 2018-02-28T04:38:33.968Z Reads: 132

```
The TB VESC's are fine for that. The FocBox is better without doubt, but regular builds are not really any issue.
```

---
## \#9 Posted by: b264 Posted at: 2018-02-28T04:55:24.569Z Reads: 129

```
[quote="Strykerpm, post:7, topic:47728"]
what are the benifits of an FocBox over a VESC?
[/quote]

A FOCBOX is a [VESC](https://github.com/vedderb/bldc-hardware) 4.12, but all the implementations of VESC4.12 have slightly different [BOM](https://en.wikipedia.org/wiki/Bill_of_materials)s and the FOCBOX has a better one.

A FOCBOX is a VESC.
```

---
## \#10 Posted by: Strykerpm Posted at: 2018-02-28T07:21:40.737Z Reads: 118

```
Torque board motors seem to be a common consensus. I saw info about the maytech motor being sealed.  I did not see any literature that would say this but it leads me to think more splash resistant.  what is the water sensitivity of most of these motors?
```

---
## \#11 Posted by: Strykerpm Posted at: 2018-02-28T07:22:24.848Z Reads: 114

```
ty did some good reading on this.
```

---
## \#12 Posted by: hornet90 Posted at: 2018-02-28T11:36:05.514Z Reads: 100

```
You could think about lipo here's a link 
This is 10s you could do 12s with a focbox 
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014?u=hornet90
I have the 10s 11 to 13 miles I've hit 32 mph with setting maxed out but 25 mph all day long 190 kv motor
```

---
