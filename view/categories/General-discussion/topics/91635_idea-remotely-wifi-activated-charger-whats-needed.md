# Idea - Remotely (WiFi) activated charger, what&rsquo;s needed?

### Replies: 19 Views: 386

## \#1 Posted by: Okami Posted at: 2019-04-24T18:37:22.748Z Reads: 129

```
Hi, Ive come up a few times with idea to remotely start a charger through a web app.

So far seems like I would need Wifi module, with relay function and leave the board's battery plugged into the charger..

Though.. what Ive heard  - It is not good / recommended to connect the charger to mains voltage while battery is connected.. I dont know the exact reason but I guess it could be with ripple voltage or some other - odd behaviour which might make it bad..

So I would love to play safe and do it the "proper" way, to minimize any risks, if there are any at all..

Any other opinions and thoughts are welcome.. 

![image|505x445](upload://cBykfG3VRL7GXdTjzhfjMI0lWOI.png)
```

---
## \#2 Posted by: mmaner Posted at: 2019-04-24T18:39:29.032Z Reads: 123

```
You could get an old nokia phone, a throw away untraceable sim and some thermite...wait that's a bomb.  Sorry, too many action movies :slight_smile:.
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-04-24T18:41:17.964Z Reads: 119

```
[quote="Okami, post:1, topic:91635"]
It is not good / recommended to connect the charger to mains voltage while battery is connected
[/quote]

nothing wrong with it i believe, its just that it creates a spark

also it turns out that with cheaper chargers the current flows from the battery to the charger (charging the charger?)
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-04-24T18:43:53.520Z Reads: 106

```
[quote="AlanZhou, post:3, topic:91635"]
with cheaper chargers the current flows from the battery to the charger
[/quote]

Can validate this, got some cheap Amazon and eBay 2a cargers and if I pull the AC end out of the wall with the charger port still in the red indicator on the charger goes from red to green
```

---
## \#5 Posted by: Okami Posted at: 2019-04-24T18:44:09.064Z Reads: 101

```
To be honest.. I saw this on some youtube guys charger.. Maybe part of thing is.. it was balance charger, but for these "automatic charging" would be more troublesome, as the charging process to be started, there would be a need for additional physical button pressing or a module which gives voltage to the button.

Anyways.. maybe for reguler bulk chargers this is not as big thing.. But yeh, voltage does flow to charger and I wonder what bad can happen from that

--

Spark happens anyway I think. at least I used to get spark when plugging xt60 with active charger.

--

So yes, this is still open for discussion, as it would require and additional 24-35v relay module, to active the battery circuit later on.

@Deckoz

@SeanHacker

(Forgot the other electronic experts)
```

---
## \#6 Posted by: Okami Posted at: 2019-04-24T19:05:36.803Z Reads: 86

```
This is the module, which could be used for switching on the charger:

https://www.banggood.com/DIY-Wi-Fi-Wireless-Switch-For-Smart-Home-With-ABS-Shell-p-1019971.html?rmmds=search&cur_warehouse=CN

With more functions and "the code way" would probably be this:

https://www.banggood.com/Wemos-ESP8266-Development-Board-WIFI-Relay-Module-220V-10A-Relay-p-1436275.html?rmmds=search&cur_warehouse=CN

Though Im not sure how much im into coding anything now.. 

But I guess with that ESP32 module it would be possible to even monitor battery voltage, otherwise a simple on/off switch wouldnt be a complete "remote charger" ..

--

Other option is also to hook up IP Cam, and physically see the battery and any voltage monitors it has..

----
So in conclusion: 

**Wifi module  + IP can actually might be the best combo**.. 

---
Still on topic is:

 **Need for relay** - and if battery is better disconnected from the chain/charger or not.
```

---
## \#7 Posted by: floyd Posted at: 2019-04-24T19:07:52.064Z Reads: 74

```
Why not just use a wifi smart plug thingie? Like these:
https://www.amazon.com/gp/product/B06XSTJST6/
```

---
## \#8 Posted by: Okami Posted at: 2019-04-24T19:09:16.184Z Reads: 72

```
Seems like neat option.. 

I would need to hookup electricity socket with the modules I showed

Yours already have the socket integrated..

So better option for EU people would be this:

https://www.banggood.com/SONOFF-S20-10A-2200W-Wifi-Wireless-Remote-Control-Socket-Smart-Timer-Plug-Smart-Home-Power-Socket-Support-Alexa-p-1142285.html?rmmds=detail-top-buytogether&ID=532403&cur_warehouse=CN

---
Though im starting to think, if the app/module supported energy consumption meter, it would be a viable method to tell how much to charge the board.. Otherwise it needs the feedback loop and so far the best/most viable option is IP cam, but have to look for how much the cheapest can be bought.
```

---
## \#9 Posted by: Okami Posted at: 2019-04-24T19:23:33.038Z Reads: 66

```
Looked up their app functions, this one seems nice:

![image|520x498](upload://4fsydqTVOXul7UaLdsulwBtWcVf.png) 

So, even if you didnt activate charging remotely, it can be started once you arrive home, if everything is connected.
```

---
## \#10 Posted by: lazarus Posted at: 2019-04-24T20:06:43.094Z Reads: 57

```
I use one of these to partial charge manually. Turn on charger, set alarm then turn off when it's up. All can be hooked up to Google home/Alexa but doesn't seem to be able to turn off after the alarm is up. Frankly embarrassing that we can recognize spoken word but can't schedule a switch to turn off.

My next board will use diebiems and will have a esp32 on board to control an external charger, by default partial charge but can schedule or trigger full charge.
```

---
## \#11 Posted by: strattos Posted at: 2019-04-24T20:37:08.909Z Reads: 54

```
Wouldn't a simple wifi smart plug fulfill this need? Am I stupid?
```

---
## \#12 Posted by: lazarus Posted at: 2019-04-24T20:45:31.717Z Reads: 51

```
90% yes. Only advantages will be cutoff on pack% and scheduled charging. Plus just plug it in and walk away, no need to pick charge time. Pretty minor QoL stuff.

Edit: oh, you probably meant why control external charger instead of interrupt charge with BMS, good point. Only advantage would be you could still get a charging CV stage which is probably not worth it.
```

---
## \#13 Posted by: spei Posted at: 2019-04-24T20:57:47.614Z Reads: 45

```
[quote="strattos, post:11, topic:91635, full:true"]
Wouldn’t a simple wifi smart plug fulfill this need? Am I stupid?
[/quote]

 [Exacly](https://www.ebay.com/p/Sonoff-IM1511160022-Smart-Switch-Module/2159289984). Other than this, there is [iMAX b6 wifi module](https://www.ebay.com/itm/New-SKYRC-SK-600075-01-WiFi-Module-Compatible-With-Original-Imax-B6-Mini-B6AC-V2/222573550128?epid=16012105089&hash=item33d26ada30:g:gOkAAOSwOgdYwooH)
```

---
## \#15 Posted by: Okami Posted at: 2019-04-25T06:06:28.165Z Reads: 32

```
The thing on question is - is it advisible to leave battery plugged into charger?

@Gamer43 @JohnnyMeduse your thoughts on this?
```

---
## \#16 Posted by: bsancken Posted at: 2019-04-25T06:19:12.943Z Reads: 32

```
Going further, why would you want to start a charge remotely?.. I've seen way too many fires on here from battery packs and this thread just screams bad idea.. (otherwise just walk on over and start it. Bam saved yah money!)
```

---
## \#17 Posted by: janpom Posted at: 2019-04-25T06:37:10.527Z Reads: 28

```
You could do it with ESP8266 and a MOSFET to switch the current on the DC side of the charger. That's safer than switching the AC. Control it with Blynk. It's very simple to DIY.
```

---
## \#18 Posted by: Gamer43 Posted at: 2019-04-25T07:45:57.462Z Reads: 25

```
Best option would be one of those wifi outlet adapters.

But I still wouldn't leave the charger plugged into the battery. 

MAYBE if the charger were a properly designed, uL certified product, I would be less hesitant, but you never know with these things. 

These chargers are essentially full bridge rectifiers hooked up to a flyback converter whose current limit function realizes constant current mode. The capacitors they use in them can be sketchy sometimes, and if those fail catastrophically, well, we have a problem.

On some chargers the battery voltage will actually back-feed the flyback converter if not plugged into the wall, this leads to some interesting behavior.
```

---
## \#19 Posted by: Okami Posted at: 2019-04-25T08:21:11.635Z Reads: 19

```
@Gamer43 Thanks for feedback. Yeh so the safe way would be to use relay switch, to connect battery to charger, after charger has been connected to mains voltage

--

@bsancken the idea is to start charging before arriving home.. 

Concerning fires.. well if battery is faulty, i think there is very little you can do, so best is to check it is healthy and monitor its physical condition as well.

IP cam would be to counter this.. though if shit happens, it happens. 

Unless u really have bucket of sand and right class fire extuinguisher

--

Best way would be to hold battery in fire proof case, though this is usually not an option unless battery is removable.

I agree that if something starts smoking u would have like minute or two to get it out of house / appartment but otherwise, if u charge while not being in same room same can happen and if flames start coming out it is too late already..
```

---
## \#20 Posted by: kevingraehl Posted at: 2020-01-04T16:13:06.799Z Reads: 4

```
![Screenshot_20200104-080308_RD%20Series|236x500](upload://t6TlwVGC5K2dwEEU1T4MjSExMgH.jpeg) ![Screenshot_20200104-081214_Photos|236x500](upload://uQP3Ga8cgp4ym4ksJrh2ZoVudhN.jpeg) 


Rd6000 off AliExpress.

Get the wifi module.


0-60 volts out.  5-6 amp charging
```

---
