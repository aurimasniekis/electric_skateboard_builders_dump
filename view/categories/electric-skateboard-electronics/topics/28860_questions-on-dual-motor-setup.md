# Questions on Dual Motor Setup

### Replies: 16 Views: 3178

## \#1 Posted by: Snowi Posted at: 2017-07-28T05:57:37.201Z Reads: 254

```
So I am interested in doing a dual motor setup. Is there a way to have only one vesc, or does it require two vescs? Also, how would the two motors communication with each other, especially with one controller? I see CAN, but idk what CAN communication is. I am trying to make my own controller powered by an Arduino. Still have to find a way to do that tho. Another question: will the software of the vesc have an option to have dual motors? How would i configure dual motors in the software?

Thanks in advance!
```

---
## \#2 Posted by: flywithgriff Posted at: 2017-07-28T06:16:48.146Z Reads: 254

```
Here's an answer is a simple way. Dual motors require dual vesc. You can set the vesc up two ways with the BLDC tool. With a CAN cable where you set one as master and one as slave or as I prefer you just use a split servo cable. The single end goes to your receiver and each of the other ends goes to a vesc. The power wire is removed from one vesc cable to make sure the receiver is not overpowered. When setting them up this way you simply configure one vesc and then save the exact same settings to the other vesc. You will still run motor detection on both vesc.
```

---
## \#3 Posted by: Silverline Posted at: 2017-07-28T06:40:32.554Z Reads: 238

```
Why not canbus with master / slave and traction control ?
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-07-28T06:46:19.319Z Reads: 228

```
That is certainly an option. When I built my dual setup all I found were horror stories with canbus and shorting out vesc and connections coming loose so I went with a Y cable. Also if one of my vesc fail the other one will still get me home. If the master goes down on a canbus you are dead in the water. It's all preference. @longhairedboy has built several boards that utilize traction control and I'm sure he can give the pros for canbus.
```

---
## \#5 Posted by: Snowi Posted at: 2017-07-28T07:50:48.183Z Reads: 218

```
Is there any place to buy there parts/wires? CAN cable and the split servo cable?
```

---
## \#6 Posted by: rojitor Posted at: 2017-07-28T11:23:32.914Z Reads: 206

```
[](10 unids/lote RC Servo y Extensión arnés de Cable Conductor de Cable 26AWG 300mm Para FUTABA JR Servo Servo RC Helicóptero Avión de Coches receptor  http://s.aliexpress.com/fuMF3q26  (from AliExpress Android))

[https://youtu.be/F70Kr9w4sj0](https://youtu.be/F70Kr9w4sj0)

Also some people said this is working fine:
[http://www.ebay.com/itm/302332736118](http://www.ebay.com/itm/302332736118)
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-07-28T11:27:00.546Z Reads: 203

```
i like can bus. lots of pros there. Mostly better use of energy due to the communication happening between the ESCs. That's a benefit of traction control. It won't waste energy spinning up a wheel more than the one next to it if its not accomplishing anything while riding. So when you carve hard on tight trucks and come up on two wheels the other one doesn't spin wildly. It also helps when you're on pavemnt with slimy wet patches. Its subtle but worth it in my opinion. 

But yes, if you don't have solid connections or solid mounting of your components and things disconnect because they come loose you'll have more problems with can bus then with split ppm. take the plastic off your connector, slip the connector on the pin, one drop of flux, one drop of solder, done.
```

---
## \#8 Posted by: Malakai Posted at: 2017-08-13T16:39:51.363Z Reads: 181

```
I've been riding longboards for years and I'm just recently started getting in to powered setups. I baught motor mounts and electronics but I'm struggling with to put it all together because of a few power issues 

The electronics I picked up are;

2 Motors are 192kv 12s 
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html?___store=en_us
2 VESC(s) 12s 60a contentious 300a peak
http://www.enertionboards.com/electric-skateboard-parts/vesc-x-programmable-brushless-motor-controller/
I'm using two 6s 10000mah 30c batteries 
http://www.ebay.com/itm/like/292181460283?ul_ref=https%253A%252F%252Frover.ebay.com%252Frover%252F2%252F0%252F8%253Fbu%253D44809890090%2526segname%253D16TE1798429_T_GENERIC_CT1%2526crd%253D20170810090000%2526mpre%253Dhttps%25253A%25252F%25252Fwww.ebay.com%25252Fulk%25252Fitm%25252Flike%25252F292181460283%2526ch%253Dosgood%2526url%253Dhttps%25253A%25252F%25252Fwww.%252524%25257Bprefix%25257Debay.%252524%25257Bdomain%25257D%25252Fulk%25252Fitm%25252Flike%25252F%252524%25257BITEM1_NUMBER%25257D%2526osub%253Dc9865e14250eaeb90646221224dc16f0%25257E5473d7cc868f380a6efae9eb6ccaa7ee%2526sojTags%253Demid%25253Dbu%25252Csegname%25253Dsegname%25252Ccrd%25253Dcrd%25252Curl%25253Durl%25252Cch%25253Dch%25252Cosub%25253Dosub%2526srcrot%253D0%2526rvr_id%253D0&ul_noapp=true
Remote Enertion Nano-X 2.4Ghz 
http://www.enertionboards.com/electric-skateboard-parts/nano-x-enertion-2-4ghz-controller/

I'm going to mount them on a hifiber Makako
 https://www.hi5ber.com/makako
With carbon gt trucks
https://evolveskateboardsusa.com/collections/gt-carbon-parts/products/gt-truck-assembly
Mounted with trampaboard motor mounts
http://www.trampaboards.com/street-carver-truck-carbon-fibre-motormount-panel-with-t6-aluminium-clamping-mount-motor-shaft-bearing-support-kit--p-13616.html
7in Onda motion wheels 
http://shop.ondamotion.com/7-0-polymer-wheels-set-of-4/

The plan was to hook the batteries up in series and then Y-split it to the two VESC(s) but I ran in to issues with connecting everything properly. The focbox (s) I received from Enertion boards has a 300a peak so I wanted to change my connections to accommodate them, due to my lack of understanding I've been struggling to find the right parts to do so. Also when I do change out the connections between my VESC and batteries will I'll need to change the ports from the VESC(s) to the motors too?
I am so close to completion but I'm just starting to understand just how lost I really am.

 any advice is appreciated thanks again
```

---
## \#9 Posted by: L3chef Posted at: 2017-08-13T16:49:42.501Z Reads: 156

```
@Malakai What pulleys are you going to use with the onda wheels? I used them on my first board aswell.

On your other question I'm not really sure what you are asking? The xt60 or is it xt90 on the focbox is fine for your battery. You won't be drawing 300amps.
```

---
## \#10 Posted by: Malakai Posted at: 2017-08-13T16:56:34.930Z Reads: 152

```
I have 3D printed carbon fiber hdt5m 60t 16mm belt width and as for the power I'm sure I won't get the full 300 but the connections between  my VESC and batteries don't fit right now so I have to replace some of them either way. I guess I was just wondering how far I can scale it up
```

---
## \#11 Posted by: Malakai Posted at: 2017-08-13T16:59:10.258Z Reads: 145

```
@L3chef how'd you like the Onda wheels? They are crazy light for the size but super thin. Do they slide around a lot?
```

---
## \#12 Posted by: L3chef Posted at: 2017-08-13T17:09:45.923Z Reads: 138

```
I didn't like them. They deformed after a couple of months for me. But before that they ran good.
Check out thingiverse and the faradaymotion spine. They have a good setup of different onda wheel pulleys
```

---
## \#13 Posted by: L3chef Posted at: 2017-08-13T17:12:37.348Z Reads: 133

```
Your drive train is off tho. With 12s and 190kv motor with that gearing. You would reach a top speed of over 60kmh
```

---
## \#14 Posted by: Malakai Posted at: 2017-08-13T17:43:48.842Z Reads: 130

```
@L3chef i don't think I mentioned the motor pulley so the ratio before now has been undetermined as far as I know. I used to hit 90kmh pretty regularly back when I had hills to bomb but now everything around me is flat so the extra push is intended. I have gearing for 1:2 1:4 and 1:5.45 ratios if it's too much
```

---
## \#15 Posted by: rich Posted at: 2017-08-15T09:40:48.662Z Reads: 115

```
[quote="Malakai, post:14, topic:28860"]
I used to hit 90kmh pretty regularly
[/quote]


Whaaaa? I would piss in my pants :joy: Jesus!
```

---
## \#16 Posted by: Malakai Posted at: 2017-08-16T20:50:29.168Z Reads: 108

```
@rich if you have a long enough road and the right set up it's easy to get to those speeds and and it doesn't even wobble.its  always funny seeing people's faces as you pass their car going down the biway
```

---
