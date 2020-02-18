# What Do You Think About Using DC Breaker Switch?

### Replies: 32 Views: 4740

## \#1 Posted by: laurnts Posted at: 2016-02-12T04:16:45.393Z Reads: 227

```
I've been wondering time to time of using a DC breaker switch. Anyone ever use it / them on your board? It looks like this.

<img src="/uploads/db1493/original/2X/7/78e49bb6a3284dddc51ad347f00a32cf69cdce3a.jpg" width="268" height="500">
https://www.conrad.nl/nl/zekeringautomaat-1-polig-32-a-siemens-5sl6132-6-612724.html

It can do 32V DC voltage with around 30A of current limit. Since it's a breaker switch, it will cut off shorts or immense current draw that exceed 30A without the need of replacing a fuse. As it's a breaker switch, there is no need for anti-spark as it could handle just direct hit of the current draw.

The only big bad disadvantage is the bulkyness, but compared to what does this could offer, seems to be not a big deal. Just wondering would it be possible?
```

---
## \#2 Posted by: claudiofiore88 Posted at: 2016-02-12T04:26:36.090Z Reads: 216

```
I know @lowguido has used a circuit breaker in one of his builds. I believe it was a 100 amp breaker.
```

---
## \#3 Posted by: barajabali Posted at: 2016-02-12T04:57:42.459Z Reads: 212

```
i would love to use a breaker I hope someone can chime in and let us know what to buy
```

---
## \#4 Posted by: Blasto Posted at: 2016-02-12T06:08:59.440Z Reads: 213

```
Those things are fhuge, and completely overkill. They are actually magnetic (current flows through a coil that activates the switch) and mechanical, i really dought they will handle all the vibration from a eboard. Then again i could be wrong.

But they're still fhuge
```

---
## \#5 Posted by: laurnts Posted at: 2016-02-12T06:11:00.626Z Reads: 207

```
I'm going to get this and try it, but I will need to wait for my VESC to come.
I will still use my big rocker switch for "handyness", this is only for electronic precaution.

There are 2 more that are relatively smaller in size, not quite sure the differences between magnetic and thermal.
<img src="/uploads/db1493/original/2X/c/cc283c6df0be67781a4702230579f1ff87aea28f.png" width="150" height="85">
http://nl.mouser.com/ProductDetail/TE-Connectivity-PB/W91-X152-30/?qs=sGAEpiMZZMsVdjGoHXLeS5ZjmtJW3deATyBaC0UfwB4%3d

<img src="/uploads/db1493/original/2X/8/8b7944d2474ac8cd21dff809ccfc51d4b04c50dc.png" width="150" height="85">
http://nl.mouser.com/ProductDetail/TE-Connectivity-PB/W33-T2N1Q-20/?qs=sGAEpiMZZMuGSqhhLqSWxYHQfBEJ0L131Cl498K4Hfc%3d

They are both only about 4cm deep, 50VDC - 65VDC about 30A.

This one is 50VDC 20A about 3cm deep and only 4 euro!
<img src="/uploads/db1493/original/2X/1/1e7a1168ac722db90e8655289f0644a9c51f9c0a.png" width="200" height="114">
http://nl.mouser.com/ProductDetail/TE-Connectivity-PB/W51-A121B1-20/?qs=sGAEpiMZZMsVdjGoHXLeS1yNdWxRO%252bLyltMZmElFvCk%3d
```

---
## \#6 Posted by: lowGuido Posted at: 2016-02-12T08:56:50.921Z Reads: 197

```
Yeah I use a breaker on this board:

http://www.electric-skateboard.builders/uploads/db1493/original/1X/40ad061aec95e8af69e2458191855b3357ee820e.jpg

its not one of the ones you have pictured there but a smaller DC breaker.
if you open the picture and zoom in you can see the red switch.
```

---
## \#7 Posted by: laurnts Posted at: 2016-02-12T09:28:56.297Z Reads: 196

```
Ohh thats nice, seems promising for me to buy one now! To be honest I like the feeling of the electronic switch, but it's not as practical as this rugged breaker switch. Very interesting!
```

---
## \#8 Posted by: sk8ace Posted at: 2016-02-12T15:51:37.939Z Reads: 191

```
I'm also using a breaker. Mine is a 100 amp AC one though. Using it as a switch only. I don't want it triggering and cutting power when I'm going uphill or something. Has never failed me yet :-)
```

---
## \#9 Posted by: lowGuido Posted at: 2016-02-12T16:02:16.918Z Reads: 189

```
Yeah i think you are safe with 100A, most skateboards will never pull more than 60A max
```

---
## \#10 Posted by: laurnts Posted at: 2016-02-13T08:33:39.863Z Reads: 181

```
@lowGuido  What breaker switch do you recommend? Your's seems to come from car parts, am I correct?
```

---
## \#11 Posted by: lowGuido Posted at: 2016-02-13T08:49:37.324Z Reads: 182

```
[quote="laurnts, post:10, topic:1325"]
Your's seems to come from car parts, am I correct
[/quote]

yeah thats right.


----------
```

---
## \#12 Posted by: barajabali Posted at: 2016-02-17T20:37:35.218Z Reads: 179

```
I just got the same breaker  @lowGuido  uses lol works like a charm 👌🏽
```

---
## \#14 Posted by: Mathieu Posted at: 2016-03-04T18:26:26.805Z Reads: 190

```
What amperage is recommended?
```

---
## \#15 Posted by: treenutter Posted at: 2016-03-04T18:35:07.637Z Reads: 184

```
@Mathieu I think it would be determined based on the settings of your ESC\VESC and the rest of your setup. I've never drawn more than 30A riding, and my motor's max is 60A. I'm not sure if there is a benefit to using the lowest possible amperage. Perhaps the size? Cost?
```

---
## \#16 Posted by: trbt555 Posted at: 2016-03-04T19:02:30.268Z Reads: 177

```
*Size: 98mm (L) x 43mm (W) x 35mm (H)*

Those things are huge.
```

---
## \#13 Posted by: Mathieu Posted at: 2016-03-04T21:56:10.294Z Reads: 176

```
hey

Since a few people are looking for something else than a key loop and using fuse blocks i found this one:
http://www.ebay.com/itm/20-30-50-60-80-100A-AMP-Car-Audio-Inline-Circuit-Breaker-Fuse-Holder-DC12v-24v-/371514509555?var=&hash=item567ffd88f3:m:m4mKYPuxh73FvvC0B_pmDdA

Thoughts on this?
```

---
## \#17 Posted by: lowGuido Posted at: 2016-03-04T22:00:00.459Z Reads: 154

```
yeah they are huge.. but you can integrate them alright.. and you can trim them down a fair bit too. its not an ideal solution but it is better piece of mind then a solid state switch and no parts to lose like a loop key.
I use 100A. on mine it seems to work well.
```

---
## \#18 Posted by: torqueboards Posted at: 2016-03-04T22:08:19.003Z Reads: 155

```
I have a new switch soon which I utilized Ben's SparkSwitch but added a few features to make it more friendly.
```

---
## \#19 Posted by: laurnts Posted at: 2016-03-04T22:13:20.507Z Reads: 166

```
The problem with circuit breaker that always confuses me is that they have rated current and breaking capacity. These smaller ones are normally only thermal breaker and not magnetic / thermomagnetic breaker. Magnetic breaker can shut off quickly but that also bad for esk8 build as surges might occur if we hit an obstacle and you don't want your board to be randomly shut off. On the other hand, the thermal breaker are more common, cheaper and can handle surges just fine as their breaking capacity is depending on current versus time. However the problem of thermal breaker is that they normally breaking at 3 - 4x their rated current. So for instance 20A rated breaker switch will break at 100A within 1 - 2 seconds.

Also within thermal breaker switch, rated current of 20A means that if it given 21A it will not break instantly. They will break after 10000 seconds (for instance).

At this moment I am testing the 20A rocker breaker switch. This one will break 100A within 1 - 2 seconds.
Ideally I think some people here want about 30A - 50A so they will break at 200A within 1 - 2 seconds exactly perfect timing for VESC before blowing up above 240A (according to Vedder site).
http://www.distrelec.ch/en/circuit-breaker-thermal-20-schurter-4435-0210/p/13322934
```

---
## \#20 Posted by: lowGuido Posted at: 2016-03-04T22:15:54.827Z Reads: 159

```
I think you are missing the point @laurnts we are looking at using the breaker as a switch, we don't particularly want it to trip at all. however the added safety of having it trip if there is a short is nice.

for what its worth, mine has never tripped. ever.
```

---
## \#21 Posted by: Hummie Posted at: 2016-03-04T22:48:06.134Z Reads: 154

```
Seems unnecessary and bulky.  Surely a small fuse is possible (as someone linked) and an antispark xt90s plug does the rest.  I don't bother with a fuse. What type of situation would it help?  If the motor shorted it's already ruined and in my experience without a fuse it it didn't take the escs out as well and I kept adding amps
```

---
## \#22 Posted by: lowGuido Posted at: 2016-03-04T23:43:27.529Z Reads: 163

```
purely cosmetic for me.

that, and I wanted to make it idiot proof.
```

---
## \#23 Posted by: kyo Posted at: 2016-09-22T16:57:20.487Z Reads: 116

```
Hi @lowGuido , what is the voltage of ur dc breaker on ur board? all the breaker i found on ebay is rated from 12v to 24v? ur system is 12s right? thats 42v . Is your breaker 42v ?
```

---
## \#24 Posted by: lowGuido Posted at: 2016-09-23T05:18:29.856Z Reads: 111

```
I have only ever used the breaker on 6S boards. My 12 S build has a loop key.
```

---
## \#25 Posted by: JdogAwesome Posted at: 2016-09-24T00:33:35.025Z Reads: 108

```
I originally used a breaker switch for my EBoard just like the one in @lowGuido picture, and I HATED it so much! First off the biggest problem was how physically big it is, so much so that I had to mount it on my board outside of the enclosure. After a lot of riding the thing started to fall apart, not only from the vibrations but from water damage. Eventually i was riding down the street on a brick road which is a horrible idea FYI, and the vibrations were bad enough that the pins holding it together fell out and the thing literally fell apart while I was riding it lol. Anyways point is I hated it so much and I wish I had originally just gone with a better quality switch like my MOSFET Switch im using now. One thing ive learned is dont be a cheap ass with EBoards, or electronics in general, because it never pays off and you just end up spending more money in the long run.
```

---
## \#26 Posted by: lowGuido Posted at: 2016-09-24T03:47:52.551Z Reads: 98

```
Personally I hate MOSFET switches I consider them dangerous because you can never really physically turn them off, only logicaly. I only will use a physical switch like a loop key or a breaker.
Which has been working on my board for over 2 years of hard riding now without falling apart. 
Having said that I dont like how big they are, and they arent rated for more than 6S. So.. not the best solution.
```

---
## \#27 Posted by: lowGuido Posted at: 2017-02-12T08:36:22.625Z Reads: 81

```
just a follow up... been using DC breakers for years now and My mate finally broke one..

https://www.youtube.com/watch?v=tjJ9_wc4ugI
```

---
## \#28 Posted by: benwong Posted at: 2017-02-12T11:46:06.163Z Reads: 74

```
How they break? I am using breaker also 
<img src="/uploads/db1493/original/3X/2/6/2613dae9067830ce69b534b093d79fa5b98d2dcd.JPG" width="666" height="500">

I think the replacement will not cost too much. 
Recently i wish to try another type of switch. 
<img src="/uploads/db1493/original/3X/3/1/31ef7596ebc51d67fb91b89a26e78e63a5b7d4b3.jpg" width="375" height="500">

6 pins of switch. 
25a per pin. 
So i connect two off and two pin on. 
Not sure work or not.
```

---
## \#29 Posted by: smurf Posted at: 2017-02-12T14:45:41.598Z Reads: 71

```
This one looks tough. I have no idea how long it would last.

https://www.amazon.com/gp/product/B01HW4YSNG/ref=ox_sc_sfl_title_11?ie=UTF8&psc=1&smid=A2LBFUKITQIB7
```

---
## \#30 Posted by: lowGuido Posted at: 2017-02-12T19:26:43.014Z Reads: 69

```
nothing test components better than direct contact with concrete at speed.
```

---
## \#31 Posted by: lowGuido Posted at: 2017-02-12T21:22:14.891Z Reads: 65

```
I think your breaker will be fine, tucked up under the truck like that.. its not going to hit the ground.
```

---
## \#32 Posted by: mmaner Posted at: 2017-02-12T21:58:04.949Z Reads: 63

```
The automotive 80-100 amp breakers are fine at 6s, anything over and they don later long.  If you want to go the XT-90s route you can get and XT-90 panel mount and XT-90 cap and keyring cover...Looks good.

XT90s
https://www.google.com/url?sa=t&source=web&rct=j&url=https://www.amazon.com/AMASS-XT90S-XT90-S-Connector-Female/dp/B01DK98USQ&ved=0ahUKEwiDve3FxovSAhVl8IMKHbY0CZkQFghiMBA&usg=AFQjCNHb1LnOm3A5VCFFK8n1X9V_Agws-g&sig2=5GdG1m3htyrqbJuKDvJWtg

XT-90 panel mount
http://www.thingiverse.com/thing:623324

XT-90 cap and key ring cover
http://www.thingiverse.com/thing:1796963
```

---
