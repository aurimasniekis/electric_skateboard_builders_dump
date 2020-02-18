# 12v off road light bar

### Replies: 47 Views: 1514

## \#1 Posted by: MyCampGround Posted at: 2018-04-08T07:06:02.973Z Reads: 146

```
I bought this 12v off road light bar, and i was wondering how i should wire it as im brand new to electric skateboard building and batteries in general. I was wondering if a 3s lipo battery would work being its just under 12v. 

[Light Specifications](https://www.superbrightleds.com/moreinfo/straight-led-light-bars/7-slim-off-road-led-light-bars-12w-1650-lumens/3770/#tab/Specifications)
![orbm7-18ws-sp|500x500](upload://wmkTXL7NDVXPQKfFdCtc29umOS2.jpg)
```

---
## \#2 Posted by: Ishayc Posted at: 2018-04-08T07:06:43.241Z Reads: 139

```
3s Lipo will work great.
If you wire it straight to the battery you can put a voltage step down.
```

---
## \#3 Posted by: telnoi Posted at: 2018-04-08T07:07:11.868Z Reads: 133

```
Get a step down with enough amperage and you can run it directly from your main power supply.
```

---
## \#4 Posted by: MyCampGround Posted at: 2018-04-08T07:07:47.613Z Reads: 133

```
I dont want to run it off main batter supply as i heard that can cause different cell drain
```

---
## \#5 Posted by: telnoi Posted at: 2018-04-08T07:08:12.200Z Reads: 130

```
Don't see how if it is powered from the main lead.
```

---
## \#6 Posted by: Steve-81 Posted at: 2018-04-08T07:10:36.452Z Reads: 124

```
If you wire it with a step down you don't have this problem, because you're linking the step down to main + and -, not only to 3 cels of the main battery :)
```

---
## \#7 Posted by: Ishayc Posted at: 2018-04-08T07:11:35.243Z Reads: 126

```
Doesn’t make sense. You wire it to the main leads not to a specific cell.
```

---
## \#8 Posted by: MyCampGround Posted at: 2018-04-08T07:18:09.724Z Reads: 120

```
if i get a step down how would i wire it directly from 12s4p pre built battery pack?
```

---
## \#9 Posted by: Ishayc Posted at: 2018-04-08T07:22:16.482Z Reads: 117

```
Take the plus and minus from the battery - the same one that goes to the controller and wire it to the step down on the input end and wire the Led bar to the output end
```

---
## \#10 Posted by: MyCampGround Posted at: 2018-04-08T07:31:13.521Z Reads: 117

```
if i wired a 3s battery to here would i need a volt meter alarm so i dont run the batter to nothing?
```

---
## \#11 Posted by: Ishayc Posted at: 2018-04-08T07:38:34.370Z Reads: 104

```
You will need to find a way to check you’re not overdischarging them. A volt meter alarm is one way.
```

---
## \#12 Posted by: MyCampGround Posted at: 2018-04-08T07:41:43.063Z Reads: 96

```
would it be better to go with a li-ion 3s pack?
```

---
## \#13 Posted by: Ishayc Posted at: 2018-04-08T07:44:01.058Z Reads: 98

```
You don’t want to over discharge lion as well, even though the discharge voltage is much lower.
```

---
## \#14 Posted by: MyCampGround Posted at: 2018-04-08T07:59:12.221Z Reads: 95

```
I already have a [imax B6](https://www.walmart.com/ip/iMAX-B6-AC-Digital-LCD-Balance-Charger-Power-Adapter-for-RC-Li-ion-Lipo-LiFe-NiMh-NiCD-Battery-Cables/614423893?wmlspartner=wlpa&selectedSellerId=7215&adid=22222222227139423071&wl0=&wl1=g&wl2=c&wl3=250236537509&wl4=pla-410425544533&wl5=1015225&wl6=&wl7=&wl8=&wl9=pla&wl10=115056135&wl11=online&wl12=614423893&wl13=&veh=sem) so all i would need is a 3s battery. what would be the best way to check that you are not overdischarging the batteries?
```

---
## \#15 Posted by: Ishayc Posted at: 2018-04-08T08:01:26.237Z Reads: 95

```
Voltage meter, alarm, BMS whatever suits you better.
```

---
## \#16 Posted by: MyCampGround Posted at: 2018-04-08T08:23:35.017Z Reads: 95

```
did a little research would something like this work?

[Step down](https://www.amazon.com/gp/product/B01J5M84FG/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1)
```

---
## \#17 Posted by: E1Allen Posted at: 2018-04-08T08:53:34.016Z Reads: 92

```
![IMG_4637|375x500](upload://xzoDYtYLLgtIR9aMTKqNLm2JxFf.JPG)![IMG_4638|375x500](upload://oms3avcvHnEDm7i5HSP7CPiZXAU.JPG)![IMG_4636|375x500](upload://sbWTQtS9jPB9qlqDwUk7D4c1bAC.JPG)

3s3p liion from laptop. Cheap Amazon 3s BMS.  4 hours of light on a light bar twice the size.

Chances are your light can handle 4s.  At least the battery my friend made it worked on 4s
```

---
## \#18 Posted by: E1Allen Posted at: 2018-04-08T08:55:31.177Z Reads: 89

```
Yes. That would work
```

---
## \#19 Posted by: MyCampGround Posted at: 2018-04-08T09:04:55.736Z Reads: 89

```
do you have any links to what you showed in picture? this is how i pictured setting it up.
```

---
## \#20 Posted by: E1Allen Posted at: 2018-04-08T09:09:01.460Z Reads: 86

```
4A-5A PCB BMS Protection Board for 3 Packs 18650 Li-ion lithium Battery Cell 3S https://www.amazon.com/dp/B01MG8XQMQ?ref=yo_pop_ma_swf

Once hooked up you have to charge it to activate the BMS.  It won't read a voltage on the output terminals or work until you do.
```

---
## \#21 Posted by: MyCampGround Posted at: 2018-04-08T09:10:33.974Z Reads: 76

```
[quote="E1Allen, post:17, topic:51555"]
Chances are your light can handle 4s.  At least the battery my friend made it worked on 4s
[/quote]

It could work with 4s, but that would probably shorten the life span of the light also that light is already bright as shit lol.
```

---
## \#22 Posted by: E1Allen Posted at: 2018-04-08T09:11:11.039Z Reads: 73

```
Yeah. It wasn't his intent to do that
```

---
## \#23 Posted by: MyCampGround Posted at: 2018-04-08T09:14:17.707Z Reads: 73

```
[quote="E1Allen, post:17, topic:51555"]
3s3p liion from laptop
[/quote]

where did you get this? Also i have never used a BMS how does it work?
```

---
## \#24 Posted by: E1Allen Posted at: 2018-04-08T09:20:57.573Z Reads: 61

```
I got the laptop batteries free from a friend.  Then to wire I just googled 3s BMS and one of the images shows you how it goes.
```

---
## \#25 Posted by: E1Allen Posted at: 2018-04-08T09:22:25.491Z Reads: 61

```
The BMS prevents over charging and over discharging.  Also balance charges the cells
```

---
## \#26 Posted by: MyCampGround Posted at: 2018-04-08T09:30:51.125Z Reads: 64

```
like this but just in series? ![Screenshot_3|445x286](upload://8bnFEbOLQaoNHmkNUWkWcCbsLPs.jpg)
```

---
## \#27 Posted by: E1Allen Posted at: 2018-04-08T09:33:40.648Z Reads: 60

```
That is series.  That is 3s1p. Mine is 3s3p so same picture but three batteries in parallel instead of one.
```

---
## \#28 Posted by: MyCampGround Posted at: 2018-04-08T09:44:58.849Z Reads: 62

```
I am sorry i meant to say parallel, it is almost 6:00 am here lol. what did you use to connect in between batteries that connects to BMS
```

---
## \#29 Posted by: E1Allen Posted at: 2018-04-08T09:47:57.480Z Reads: 63

```
![IMG_4747|281x500](upload://su9tcgpCKNxWEPJyh8hLjCqQB62.jpg)

I spot welded the pack and soldered wire between the series connections.
```

---
## \#30 Posted by: MyCampGround Posted at: 2018-04-08T09:56:24.918Z Reads: 61

```
i dont have a spot welder, dont they already come spot welded together from laptop battery pack?

![Screenshot_4|690x380](upload://xD4UEBtcNack9Ko7IiOIlQRsuSQ.png)
```

---
## \#31 Posted by: MyCampGround Posted at: 2018-04-08T16:25:07.492Z Reads: 51

```
if i wanted to permanently mount this into my enclosure would i just need xt90 y connector at the battery so one goes to light other mounted into enclosure for charging?
```

---
## \#32 Posted by: E1Allen Posted at: 2018-04-08T16:25:07.679Z Reads: 47

```
Yes they were spot welded.  I just changed the shape of the pack.  The BMS that's attached to the laptop pack has to come off.  Then the basic one can be wired in its place
```

---
## \#33 Posted by: MyCampGround Posted at: 2018-04-08T16:26:11.378Z Reads: 45

```
awesome yah i found a video on youtube showing you how to disassemble it. looks really easy.
```

---
## \#34 Posted by: E1Allen Posted at: 2018-04-08T16:27:43.077Z Reads: 45

```
Yes. Or unplug the light and use that lead.  You can use a smaller connector if you want. The light draws like 2a
```

---
## \#35 Posted by: MyCampGround Posted at: 2018-04-08T16:28:43.548Z Reads: 46

```
ok awesome what connector would you use?
```

---
## \#36 Posted by: E1Allen Posted at: 2018-04-08T16:30:47.517Z Reads: 46

```
I used a xt60 because I have them.  For you I would just use whatever is compatible with your board and charger.
```

---
## \#37 Posted by: MyCampGround Posted at: 2018-04-08T16:46:02.909Z Reads: 52

```
[quote="MyCampGround, post:14, topic:51555"]
I already have a imax B6
[/quote]

so basically i would have to buy connectors the imax B6 came with a xt60 to bullet connector. so i guess i should just buy xt60 for ease of use.
![Screenshot_5|593x443](upload://6YmOvO4Tu7SN1KQMMJk4xHpTnyr.png)
```

---
## \#38 Posted by: E1Allen Posted at: 2018-04-08T16:57:44.503Z Reads: 51

```
I use lots of xt60s because that's what my chargers use.
```

---
## \#39 Posted by: MyCampGround Posted at: 2018-04-09T05:14:33.976Z Reads: 43

```
could i use this switch to power the light on and off?
[12v White LED Switch](https://www.ebay.com/i/301203246981?chn=ps&var=600262374404)
```

---
## \#40 Posted by: E1Allen Posted at: 2018-04-09T05:39:14.858Z Reads: 41

```
I don't see why not.  It should work just fine. I've never used one.
```

---
## \#41 Posted by: ARetardedPillow Posted at: 2018-04-09T06:05:19.817Z Reads: 35

```
I have that exact light connected to a step down from my 10s pack. I have a switch to turn it on and off aswell
```

---
## \#42 Posted by: MyCampGround Posted at: 2018-04-09T06:11:16.979Z Reads: 33

```
@ARetardedPillow yah i went with a quality brand superbrightleds.com other than one from amazon.com that had really bad reviews of water leaking inside lens just from humidity.
```

---
## \#43 Posted by: MyCampGround Posted at: 2018-04-09T06:14:22.330Z Reads: 35

```
do you happen to have a picture of the light on a night?
```

---
## \#44 Posted by: MyCampGround Posted at: 2018-04-09T06:34:13.036Z Reads: 37

```
since i want to make everything permanent inside the enclosure should i use a charging connector that is waterproof for the 12v light? [5.5 x 2.1mm waterproof female jack](https://www.ebay.com/itm/111889160001?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT)
```

---
## \#45 Posted by: E1Allen Posted at: 2018-04-09T06:36:25.391Z Reads: 37

```
That's a good idea
```

---
## \#46 Posted by: ARetardedPillow Posted at: 2018-04-09T07:19:21.310Z Reads: 35

```
Its bright as hell trust me 
![IMG_6334|666x500](upload://boyRYOK7z5Z1PgQnEdIbRhiO2eN.jpg)
```

---
## \#47 Posted by: MyCampGround Posted at: 2018-04-09T08:10:12.598Z Reads: 32

```
awesome i am so stoked! thanks for the picture.
```

---
