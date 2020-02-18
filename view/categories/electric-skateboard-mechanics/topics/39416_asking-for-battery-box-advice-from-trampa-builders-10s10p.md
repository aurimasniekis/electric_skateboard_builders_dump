# Asking for Battery box advice from Trampa builders - 10s10p+

### Replies: 25 Views: 1489

## \#1 Posted by: dimnsionofsound Posted at: 2017-11-27T03:42:53.907Z Reads: 284

```
Not sure if this belongs in Esk8 electronics or Mechanics category, but I am speccing out my next build which will use a Trampa MTB-572 deck and I am trying to figure out the maximum size case I can fit between the bindings. 

I have already ordered 150 Samsung 30Q cells and I would love to fit at least 100 in whatever battery box I end up using, preferably 120 in a 10S12P configuration. I looked around the Pelican case website and found [the 1300](http://www.pelicancases.com/Pelican-1300-P83.aspx) case which looks like it will definitely let me fit 120 cells inside on the bottom half, leaving the rest open for BMS and 2-4 VESC6. 

The question I have for you all that have a similar trampa deck is whether or not the top of the case is going to rub onto my legs while I am riding. It looks like it will fit between the bindings but given the possible angle of my legs, I don't want to be annoyed with it hitting me.
```

---
## \#2 Posted by: Kug3lis Posted at: 2017-11-27T03:48:36.040Z Reads: 277

```
[quote="dimnsionofsound, post:1, topic:39416"]
10S12P
[/quote]

Are you trying to reach the moon with 1.5kWh battery pack?
```

---
## \#3 Posted by: Kug3lis Posted at: 2017-11-27T03:51:12.674Z Reads: 270

```
With 1500Wh and worst case scenario 30Wh/km you would get 50km best case scenario 150km
```

---
## \#4 Posted by: evoheyax Posted at: 2017-11-27T03:52:56.899Z Reads: 264

```
My feeling is it's more so he can do 200 amp con discharge... This is the problem with 18650's. They have too low of a discharge for high amp situations.
```

---
## \#5 Posted by: dimnsionofsound Posted at: 2017-11-27T03:59:10.535Z Reads: 260

```
You both are right - I want to never worry about range, ever, so that I can do long trips while mashing the accelerator. As well, all terrain wheels killing efficiency, plus 4 VESCs is not going to be easy on something like a 10s4p. 

The seconday purpose for this battery pack in the longboard is to power a 36V inverter for backup power. 

If my calculations are correct, I should be able to pull minimum 5000 watt continuous through 4 VESCs resulting in me probably falling backwards as my board shoots forward from under me :smiley:
```

---
## \#6 Posted by: evoheyax Posted at: 2017-11-27T04:01:20.809Z Reads: 248

```
Which VESCs are you going to use and have any methods to cool them?
```

---
## \#7 Posted by: Cobber Posted at: 2017-11-27T04:02:51.680Z Reads: 255

```
yeah, that is the next obstacle for eSk8, all the cool, fast eBikes run water cooled motors, electronics and batteries...

and I don't mean pushbikes with motors I mean motorbike performance...

like this
https://static1.squarespace.com/static/57a3ad7ae3df28c404a7d817/t/5a03ae2c652deabdd3135b7f/1510190641431/1.jpg?format=1500w
or this
http://images.motorcycle-usa.com/photogallerys/Mission-Motorcycles-RS-rh.jpg
or this
http://cdn.hiconsumption.com/wp-content/uploads/2017/08/Lightning-LS-218-All-Electric-Superbike-0.jpg
```

---
## \#8 Posted by: dimnsionofsound Posted at: 2017-11-27T04:10:49.924Z Reads: 239

```
VESC 6 to get the aluminum casing. I have yet to figure out any special cooling but have ideas such as

* leaving them out in the open with airflow
* airflow channel with filtered/mesh entrance, possibly a fan, leading to heatsinks on each of the VESC

After watching Ben's video about the continuous current capacity on the VESC 6, it looks like each can handle 45 Amps after more than a minute of working hard at more amps than that, so that gives me 4*45 = 180 motor amps.

180 motor amps * (conservative) average voltage of 3.5V = 6300 W VESC power handling.
10P Samsung 30Q -> 10 * 15A rated amps from battery = 150A -> 150A * 35V = 5250W from battery at slightly less than nominal voltage (to account for sag).

Min of those two is still around 5kW. If I can fit 12P instead of 10P than the battery's rated current jumps to 12P * 15A = 180A, bringing it in line with the 4x VESC6 current capacity.
```

---
## \#9 Posted by: Kug3lis Posted at: 2017-11-27T04:12:48.357Z Reads: 222

```
Do you understand that you will need to run a plate not nickel strips on 18650 to cover 150A through the pack?
```

---
## \#10 Posted by: dimnsionofsound Posted at: 2017-11-27T04:14:54.561Z Reads: 223

```
Yes, the I^2R losses do really come into play here. I'll do more research on how I want to connect the batteries together, including the resistivity of multiple nickel strips on top of each other. Nothing else has been ordered yet and I'm not going to do this 3/4-assed like my last build heh
```

---
## \#11 Posted by: Kug3lis Posted at: 2017-11-27T04:16:07.644Z Reads: 218

```
and also learn of current flows, because in parallel connections current does not divide equally and every 90º corners and etc cause some serious problems.
```

---
## \#12 Posted by: Kug3lis Posted at: 2017-11-27T04:19:49.839Z Reads: 218

```
P.S. vesc will not handle 6kW motors, not even 4kW
```

---
## \#13 Posted by: dimnsionofsound Posted at: 2017-11-27T04:19:58.299Z Reads: 211

```
Yup. Ideally each battery in each parallel strip will have an equal resistance path to move to the next parallel strip, and the lower the resistance for each one, the better. That's another opportunity for research/calculation/simulation to try to come up with the best solution. 

I would love to avoid a connection system that has each P group connected from the same end, giving the single cell in each P group closest to the connection much more stress due to the lower resistance connection between it vs the ones at the end of the P group in such a configuration
```

---
## \#14 Posted by: dimnsionofsound Posted at: 2017-11-27T04:20:33.676Z Reads: 198

```
> 4x VESC6
```

---
## \#15 Posted by: Kug3lis Posted at: 2017-11-27T04:21:28.403Z Reads: 190

```
Oh you meant in total.
```

---
## \#16 Posted by: dimnsionofsound Posted at: 2017-11-27T04:23:10.029Z Reads: 198

```
Yeah, I am trying to be conservative in my usage of each part of the drivetrain, and with the acceleration and continuous power I would like, it seems the best way to do that is to spread the stress over a large battery and 4 separate ESC/motor sections.
```

---
## \#17 Posted by: Kug3lis Posted at: 2017-11-27T04:24:16.468Z Reads: 197

```
Then you step into high current world, you can forget simple stuff, my parallel connection board for LiPos will consist or literal copper bus bars, and load switcher of BMS Mosfet's will sit literally on 5mm copper plates instead of PCB
```

---
## \#18 Posted by: Okami Posted at: 2017-11-27T22:48:15.211Z Reads: 178

```
Ask @celica39 about his batt "box".. it is a good question how high battery can be before being in the way..

I suppose it should be less than your 1/3 knee.height or similar.

Otherwise kudos for the monster board building plan.. thats real huge battery you are planning to incorporate not to mention 4x vesc 6 :)
```

---
## \#20 Posted by: Acido Posted at: 2017-11-28T15:34:49.900Z Reads: 159

```
Man that battery is INSANE hope you post a build thread after you finish it, you will need an HUGE enclosure for that
```

---
## \#21 Posted by: sk8l8r Posted at: 2017-11-28T15:44:52.920Z Reads: 154

```
how much extra performance would watercooling esk8 parts give? (used to water cool PCs back in 2005 and have many parts lying around)
```

---
## \#22 Posted by: Cobber Posted at: 2017-11-28T16:23:02.074Z Reads: 150

```
It is a lot, imagine you could not overheat your batteries, your esc and motors could produce numbers closer to peak continuously... a limit to performance is heat. if your general ride conditions do not involve major load then helping load performance will not do much, but if you like climbing hills for example then it is a different story. esc is the first, then batteries, depending on motor mass I think.
```

---
## \#23 Posted by: gravitycarve Posted at: 2017-11-28T16:24:13.048Z Reads: 147

```
:heart_eyes:That Alta Supermoto tho :heart_eyes:
```

---
## \#24 Posted by: Cobber Posted at: 2017-11-28T16:30:49.390Z Reads: 147

```
yeah and now they have Dale Lineaweaver helping them tune it, a switched on dude... even all the way in Australia I used to run his custom needles on my Husaberg.

<img src="/uploads/db1493/original/3X/7/1/715e6ddfe49eaf6173653ff79d6f2d601709151e.png" width="651" height="450">

but I'd prob. go a Dale Lineaweaver flat track special first ;) dude is a dead set dirt track whisperer
```

---
## \#25 Posted by: meesie Posted at: 2019-06-25T13:17:51.639Z Reads: 42

```
sorry for the bump, but i'm really damn interested in what he went for in the end
```

---
## \#26 Posted by: murdomeek Posted at: 2019-06-25T16:55:14.814Z Reads: 36

```
[quote="Cobber, post:22, topic:39416"]
the fir
[/quote]

seconded!
wheres that build thread? =D
```

---
