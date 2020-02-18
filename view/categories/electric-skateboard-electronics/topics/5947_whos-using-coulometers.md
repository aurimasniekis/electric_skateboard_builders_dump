# Whos using coulometers

### Replies: 45 Views: 3687

## \#1 Posted by: Pablo_702 Posted at: 2016-07-12T01:36:52.980Z Reads: 249

```
whos using one? and how is it wired? and what information can you get real time while riding?
```

---
## \#2 Posted by: KMeyerson Posted at: 2016-07-12T02:17:56.323Z Reads: 244

```
Me!

I have GT Power Wattmeters on my builds between the battery and ESCs.  Haters gonna hate, but I use it for voltage/battery check and to do basic math (how many watts did I consume going x distance in y amount of time?).

Its handy, but gives you a lot more information than you need. It can really help if you're building your own motors and need to check your stator/pole ratio and or your sensor setup. When you're drawing too many amps, then you know you didn't really make anything better.
```

---
## \#3 Posted by: Pablo_702 Posted at: 2016-07-12T02:22:24.510Z Reads: 236

```
After the power switch right? Do ubhve a link for your meter? Pics of wiring perhaps
```

---
## \#4 Posted by: rpn314 Posted at: 2016-07-12T02:40:01.065Z Reads: 225

```
I bought [this guy on ebay](http://www.ebay.com/itm/141413493299?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT). Can't comment on quality as I haven't received it yet, but I'm not too worried about it.
```

---
## \#5 Posted by: KMeyerson Posted at: 2016-07-12T02:51:07.051Z Reads: 214

```
I own one of those too.  PCB/schematic is nearly identical, you'll have no problems.  The potentiometers are not present, but it's factory calibrated.

I just plug mine in and use this as the antispark.

If I were to do it again, I'd use XT-90 antispark plugs between the battery and switch (or battery and Wattmeter) and make a loop key from a standard XT-90 or 60
```

---
## \#6 Posted by: bill_f Posted at: 2016-07-12T13:47:50.764Z Reads: 192

```
I bought this deal [here](http://www.ebay.com/itm/Capacity-Tester-coulometer-F-8-50V-350A-Lithium-Lead-acid-Battery-Voltmeter-AMP-/221962147414?hash=item33adf99656:g:iPsAAOSwxN5WZWUv) but have not had time to look into the installation. The shunt is huge. Maybe too big for what I need. Worth getting a smaller shunt? ([my build specifics](http://www.electric-skateboard.builders/t/diy-cherry-stick-trampa-infinity-trucks-8-slickline-wheels-ollin-vescs-dual-sk3-6374-149-kv-scramboard-motor-mounts-and-pulleys/4805))
One of the emtb guys here has it on his rig. Need to dig around and find out who it is and see how he installed it.

The Shunt
<img src="/uploads/db1493/original/2X/5/50d516e40ca504c806e946665f2a97cce90577d7.PNG" width="451" height="320">
```

---
## \#7 Posted by: JdogAwesome Posted at: 2016-07-12T16:15:33.327Z Reads: 171

```
I bought one of these, http://m.ebay.com/itm/DC-100A-Two-way-Detect-wireless-power-meter-voltage-current-charge-capacity-time-/181866030474?nav=WATCHING_ACTIVE

For my EBoard and its not bad. I don't really use it much because I don't like carrying the wireless receiver with me though I have used it for testing the board and seeing my amperage draw. The functions on it don't seem to work, though I may he do I may be doing something wrong, like the auto shutoff function and stuff. Might be worth checking out and seeing if it may be useful. Only problem is its rather larger and takes up quite a lot of space in my enclosure, I do plan on taking it out now because I don't need it anymore and I already know my amperage draw.
```

---
## \#8 Posted by: Pablo_702 Posted at: 2016-07-12T17:27:39.083Z Reads: 164

```
My plan is having ll the electronics in the enclosure and the screen mounted on the top of the board so i can see it is ride
```

---
## \#9 Posted by: devin Posted at: 2016-07-12T18:40:36.974Z Reads: 162

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#10 Posted by: rpn314 Posted at: 2016-07-12T18:41:41.924Z Reads: 157

```
I was just planning on using it for diagnostics during my build and if any issues come up, but I'm not planning on making a permanent space for it on my board
```

---
## \#11 Posted by: KMeyerson Posted at: 2016-07-13T01:02:17.216Z Reads: 147

```
Yeah, thats generally how it ends up. Do you have a volt meter though?
```

---
## \#12 Posted by: rpn314 Posted at: 2016-07-13T01:19:17.585Z Reads: 146

```
Yeah. [This meter](https://www.ebay.com/itm/262501050575 ) will be a permanent part of my build.
```

---
## \#13 Posted by: Mobutusan Posted at: 2016-07-13T08:32:04.175Z Reads: 142

```
Here's a little setup I've got running using a Tenergy Watt meter (same as GT Power), and a Xiaomi Yi camera, both from Amazon. The ghetto Gorilla tape hood is so the camera can view the backlit screen in the dark, so outside light variations don't interfere with viewing. The camera can also be removed, to view the screen while riding, although it can be a bit hard to see in bright light, and looking down while you're going fast can get a little sketchy. I haven't had a chance to use it much since I got it set up, but it allows me to take video logs of the real-time data. If only I could figure out how to also monitor speed at the same time and data log each run. 

<img src="/uploads/db1493/original/2X/8/889a431c45f1375683533fa0dc4dc047b263ae2d.jpg" width="281" height="500">

<img src="/uploads/db1493/original/2X/f/f16579449475ced51bd7172bbacc431ff2307ffc.jpg" width="690" height="388">

<img src="/uploads/db1493/original/2X/6/6c5c4028a52d4189c0148355f7de266c346ff6eb.jpg" width="690" height="388">
```

---
## \#14 Posted by: Okami Posted at: 2016-07-16T08:50:45.160Z Reads: 123

```
Hello everyone! A topic about what is the real amp draw / current needs for a system surfaced on another topic. So everyone with a watt meter / configured vesc are welcome!

So, gladly @DeathCookies made a simple template for everyone to enter their data into.

Any feedback / improvements would be great, as I think it is still possible to be changed and should be improved. You should contact him personally, as I think there is not a seperate thread about the poll yet.

Poll for entering Amp draw data:
---
http://gct-hp.de/esk8/index.php 
---
 *delete any numbers after index.php, if there is a number it won't work
---
<img src="/uploads/db1493/original/2X/d/d4b686faff0f39f57f6d1d1ed16d14ac0f64e8cc.png" width="300" height="300">
```

---
## \#15 Posted by: Cptanpanic Posted at: 2016-08-18T11:38:26.512Z Reads: 113

```
This is an older thread, but was wondering for something like the GP Power watt meter, does it have any type of memory, like for max amps, etc.  Or do you have to be looking at it the whole time, which would explain the gopro above?
```

---
## \#16 Posted by: Pablo_702 Posted at: 2016-08-18T13:08:12.657Z Reads: 101

```
That's a really good question
```

---
## \#17 Posted by: Hummie Posted at: 2016-08-18T15:59:41.232Z Reads: 102

```
Agreed it's a shame to have a watt meter but have to be looking at it.   This one I've had and it graphs the amps on its little lcd screen through time. Pretty awesome in a thin colorful package 

http://www.hobbyking.com/hobbyking/store/__69085__Turnigy_2_in_1_Power_Meter_Servo_Meter_1_5_TFT_RU_Warehouse_.html


 I really liked the idea of it but wish it showed voltage sag too and not just amps and it burnt out on 12s quickly and im not getting another and it seems to still be out of stock.  

The vesc has everything u could want being calibibrated and if youre computer literate you can record what it registers.  Wish it was easier.
```

---
## \#18 Posted by: devin Posted at: 2016-08-18T16:09:06.447Z Reads: 97

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#19 Posted by: Hummie Posted at: 2016-08-18T16:13:59.840Z Reads: 96

```
Yea cool math solution to do it if needed but requires zeroing(unplug and replug) to find values hit on specific hills or at different points in time.
```

---
## \#20 Posted by: devin Posted at: 2016-08-18T16:15:03.095Z Reads: 100

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#21 Posted by: sl33py Posted at: 2016-08-18T16:17:06.615Z Reads: 102

```
I used it on an older setup to determine my peak amp draw, power in watts, etc.  Cool info to know.  Also helps me determine actual battery amp supply for future builds (using same motors/gears/etc.).

Mine (i think the GT 150a one) shows peak as well as some live data, but saves the peak values and rotates them to view when you stop.  It however does not have memory and once powered off is reset and data is lost.  Here are some old pics of mine showing amps/watts/etc.
[img]https://goo.gl/28RZao[/img]
at a stop - no amps.  30.6v left in the pack (8s).  1921 Watts peak.  1.x Watts at the stop (maybe wheel was still spinning a bit?)
[img]https://goo.gl/zqKbSz[/img]
Again no amps - 30.6v left (8s) - 65 Amps peak (dual 5065 200kv VESC) - 2.1 Watts at rest (not sure why).

It cycles through mAh/Ah consumed, and a few other things - the ones i wanted to see was Watts and Amps peak.  Just as good info to know.
```

---
## \#22 Posted by: devin Posted at: 2016-08-18T16:22:03.829Z Reads: 97

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#23 Posted by: sl33py Posted at: 2016-08-18T16:29:59.281Z Reads: 99

```
There are two i know of, that have the best logging (and stored for review later w/ graphs) that i've seen.  The first is the eagletree v4 logger:
[img]http://www.eagletreesystems.com/image/data/powerful%20charting%20software.gif[/img]
You can add sensors (temp, GPS, etc.), and a LCD display - pretty modular but a bit $$ - especially compared to a $20 watt meter like above.  Select what you want to see as well on the graphs depending on sensors you have.  Pretty cool really.

Another option is the Speedict Mars/Mercury which does similar (actually some really cool views - this is just a quick pic i could find of the graphing.  Some great map overlays w/ info at each point - using the gps in your phone for location vs a gps module):
[img]http://i451.photobucket.com/albums/qq236/d8veh/rides/speedict%20climb_zpswmvpj536.jpg[/img]

They also have a "BMS" (not it's not a real BMS) - but it does show pack voltage and cell detail to your phone via BT!:
[img]http://www.speedict.com/neptune-lite/images/2-phones-neptune-lite.png[/img]

They are also $$$.  But do logging for review later - and unique to the speedict = have BT and apps on your phone.
```

---
## \#24 Posted by: sl33py Posted at: 2016-08-18T16:30:47.962Z Reads: 86

```
that makes sense.  plus the screen and any power drawn by the watt meter.
```

---
## \#25 Posted by: devin Posted at: 2016-08-18T16:32:12.089Z Reads: 87

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#26 Posted by: sl33py Posted at: 2016-08-18T16:35:11.458Z Reads: 86

```
hehehe - and then a third watt meter to measure the second watt meter... :smiley:

Makes sense though.  I'm pretty sure it's minimal draw either way.  thanks for pointing it out though!
```

---
## \#27 Posted by: Hummie Posted at: 2016-08-18T16:43:34.745Z Reads: 81

```
Sleepy I've never seen that speedict thing! Awesome how every cell voltage is shown in realtime on the phone!  I want it badly and as long as it's not too big in the board.  Just started checking it out and it looks small and at 90$ worth it.  I ruin cells so quickly this is a money saver. U like it? Or it seems u haven't used it
```

---
## \#28 Posted by: Cptanpanic Posted at: 2016-08-18T16:48:03.105Z Reads: 80

```
Anybody see any builds that they permanently mounted a GT watt meter?  Would like some ideas on how it could fit.
```

---
## \#29 Posted by: devin Posted at: 2016-08-18T16:49:21.145Z Reads: 79

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#30 Posted by: sl33py Posted at: 2016-08-18T16:55:23.543Z Reads: 84

```
[quote="Hummie, post:27, topic:5947"]
U like it? Or it seems u haven't used it
[/quote]


Just got it the other day! - plus the Mars inline as well.  I now have both the Eagletree eLogger v4 and Speedict - one planned for each of my next two boards!

I can easily use the Speedict Neptune Lite (their "BMS") on one of the boards to try it out - what do you want to see?
```

---
## \#31 Posted by: sl33py Posted at: 2016-08-18T16:56:29.712Z Reads: 85

```
I remember seeing a couple folks who incorporated it into their enclosure - screen removed and set into the case/enclosure.  Let me look at see if i can find a pic.  My original plan before i went off the deepend with the Eagletree and Speedict.

@okp - he used one in his original vaguard build:
[img]http://www.e-sk8.fr/wordpress/wp-content/uploads/2015/08/IMG_3590.jpg[/img]
And the one before also i think.
```

---
## \#32 Posted by: longhairedboy Posted at: 2016-08-18T17:06:57.120Z Reads: 78

```
i go by smell. If things start to smell funny, i'm drawing too many amps.
```

---
## \#33 Posted by: Hummie Posted at: 2016-08-18T17:41:43.024Z Reads: 77

```
Haha. 


I'm looking up the speedcific stuff and it's really nice

I'd rather do the visual part on the phone than try to jam anymore stuff in a board. 

Man if only they integrated a simple balancing feature I'd be sold.  I have all these little balancers for ten bucks and I'd still have to use them with this.  A simple discharge balancer and this thing would be fantastic.  Don't know why they don't.  Anything u know that does that? Not necessarily a bms but just a simple balance feature
```

---
## \#34 Posted by: Hillso Posted at: 2016-08-18T22:17:08.538Z Reads: 80

```
Why not just use some board like arduino that can read voltage and send with bluetooth module?
it will cost ~10$
```

---
## \#35 Posted by: Hummie Posted at: 2016-08-18T23:22:26.341Z Reads: 78

```
really I'm looking for a balancer for 12s.  Something like the battery medic but that can do 12s.  the other features are helpful but if they can't discharge also it's back to the same thing.  How hard would it be to make a 12 cell balancer?
```

---
## \#36 Posted by: RogerD Posted at: 2016-08-20T18:05:53.974Z Reads: 81

```
Search my posts on here (title includes coulometer or fuel gauge), I installed a coulometer on my board. Works perfectly. Full schematic on my post .

http://i97.photobucket.com/albums/l235/dodgey99/General%20pics/IMG_3251_zpstpj6dcp4.jpg

http://i97.photobucket.com/albums/l235/dodgey99/General%20pics/IMG_3246_zpseazyfvpq.jpg
```

---
## \#37 Posted by: elkick Posted at: 2016-08-20T20:21:02.849Z Reads: 82

```
<img src="/uploads/db1493/original/2X/5/574938ac9bdb1310b715e61784e9b7d27ce1a8e1.jpeg" width="375" height="500">
Agree, works well. (Picture taken before calibration)
```

---
## \#38 Posted by: Okami Posted at: 2016-10-05T23:47:07.282Z Reads: 61

```
[quote="devin, post:18, topic:5947"]
@Hummie You can calculate average voltage under load (average voltage sag value) by dividing total watt hours used during ride by total amp hours used during ride. This gives average battery voltage during throttle use.
[/quote]



Hi there! Know I that this is not the newest post - although - I was not entirely clear on the calculation. Can you do an example?

I tried to input the numbers, like 240wh (for 10Amps X 24v), then dividing this number by 2Ah, gives me 120. What exactly is this number and is there any use for it? I think there's a point im missing here :rolling_eyes:

Been looking into understading batteries better so this would help with that.
```

---
## \#39 Posted by: devin Posted at: 2016-10-06T03:56:32.632Z Reads: 58

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#40 Posted by: Okami Posted at: 2016-10-06T08:57:26.870Z Reads: 58

```
Oh okay, will try to do this once I hit the streets with my board ;)
```

---
## \#41 Posted by: GrahamZhu Posted at: 2016-10-06T09:15:29.727Z Reads: 56

```
Cheap Option 
https://www.aliexpress.com/item/Free-Shipping-Digital-60V-100A-Battery-Power-Analyzer-Watt-Meter-Balancer-For-DC-RC-Helicopter/32602350560.html?spm=2114.30010308.3.63.losM7q&ws_ab_test=searchweb0_0,searchweb201602_5_10056_10065_10055_10068_10054_10069_10059_10073_10017_10070_10060_10061_10052_10062_10053_10050_10051,searchweb201603_4&btsid=b69c9a7c-5564-4f1a-873a-bd818c456305
```

---
## \#42 Posted by: Okami Posted at: 2016-10-06T17:38:42.547Z Reads: 54

```
I think this is a better option:

https://www.aliexpress.com/item/GT-Power-RC-130A-Power-Analyzer-Watt-Meter-Battery-Consumption-Performance-Monitor-With-LCD-Display/32703905271.html?spm=2114.01010208.3.2.7aH4OI&ws_ab_test=searchweb0_0,searchweb201602_1_10056_10065_10068_10055_10054_112_10069_10059_110_111_10073_10017_109_10070_108_10060_10061_10052_10062_10053_10050_10051,searchweb201603_7&btsid=1b796b6f-7eea-4860-930a-69492f1276cf

Has backlight, better looking. Also higher Peak amps (there''s also a 150A version).
```

---
## \#43 Posted by: Hummie Posted at: 2016-10-06T17:42:32.946Z Reads: 51

```
if you have the vesc you can hook it up to your phone and record more detailed data than a typical watt meter.  easier cheaper and smaller
```

---
## \#44 Posted by: Okami Posted at: 2016-10-06T17:43:44.267Z Reads: 53

```
Cool, will advise this once we complete making the Esk8 database site.. user input will be higly appreciated there, especially in terms of energy use, peak power and so on.
```

---
## \#45 Posted by: sl33py Posted at: 2017-07-03T01:36:00.000Z Reads: 35

```
Reviving an old thread.  I've had the eagletree v4 data logger for a while and just didn't like the wires and form factor...

I want to be able to drop it inline - log data and compare amps of different or similar systems.  Like on the new VESC Six, or a stock v4.xx vs heatsink 4.xx.

Long weekend - list of projects getting knocked out!  Here's the before:
[img]https://goo.gl/snSwfH[/img]
(long wires just made a mess and wasn't happy w/ them)

I got some super beefy copper wire from work i've had for misc:
[img]https://goo.gl/SL3xpR[/img]

Took a few minutes to get angles right:
[img]https://goo.gl/1b5MbL[/img]

heatshrink and cleaned up a bit.  I need to find some more clear shrink for over the top to protect and keep info legible.
[img]https://goo.gl/5QiYCz[/img]

Drop it size now, easy to separate wires, add in-line, and log.  Remove when done.

I want to really double check my amp draw as i'm looking to build some 18650 packs and want to make sure i'm sizing them correctly for the amp draw i need riding.  I think this will be super helpful!

Everyone have a safe 4th!
```

---
