# VESC FAQ &#124; !WARNING! - Handle With Care - Read before buying!

### Replies: 41 Views: 7597

## \#1 Posted by: onloop Posted at: 2015-11-15T22:31:26.881Z Reads: 634

```
**This article is a Warning & Guide for how to properly handle the VESC.**


There has been lots of issue lately with people blowing up their VESC.... It's really the worst feeling when this happens! I have now blown 3 myself. If I had better knowledge I could have prevented this from happening.

> **IMPORTANT SAFETY NOTES ABOUT VESC**

>  - The VESC is not a finished product! - It's only just reached BETA stage.
>  - The VESC is a bare PCB with no protective case/cover - It can be damaged very easily!
>  - The VESC should be installed into a protective case OR insulation heat shrink tube before use.
>  - When powered up the VESC can be shorted very easily against ANY conductive material, even carbon fiber!
>  - Electrostatic Discharge could damage the VESC. 
>  - Install a fuse between the VESC and power supply to help prevent damage from short circuits.
>  - Power the VESC using a low voltage low amperage power supply (e.g. from a laptop) when doing motor detection and parameter adjustments in the BLDC tool
>  - Make a Backup of the default VESC settings before you change anything.
>  - The VESC doesn't come with any instructions! - You will need to read up on it yourself!
>  - Handle the VESC with Caution.
```

---
## \#2 Posted by: treenutter Posted at: 2015-11-15T23:42:39.277Z Reads: 589

```
Thanks @onloop I think this will help lot of people using VESC.

Regarding this comment: 

[quote="onloop, post:1, topic:491"]
Power the VESC using a low voltage low amperage power supply (e.g. from a laptop) when doing motor detection and parameter adjustments in the BLDC tool
[/quote]

Could someone perhaps provide a recommendation for what kind of  power supply is right for this usage (maybe show an example)? I've had no issues using my regular batter packs (fed through a battery arming switch) during motor detection, but I may have just been lucky!
```

---
## \#3 Posted by: onloop Posted at: 2015-11-16T02:44:10.440Z Reads: 528

```
A Battery can instantly dump high current into the VESC causing burns, electrocution, equipment damge & fire, better off using a controlled power source such as a LAB POWER Supply.
<img src='/uploads/db1493/original/1X/c6d475bc5a9936aabfd0d9f0d903854ce345ebd7.jpg'>



**Otherwise a 12-20V 3-5A Laptop power supply is the poor-man's alternative.**
<img src='/uploads/db1493/original/1X/eace3685eecc4d736600173cff919472cb11e2d5.jpg'>
```

---
## \#4 Posted by: kai Posted at: 2015-11-16T03:20:22.653Z Reads: 463

```
so the space cell is not safe to do motor detection?
```

---
## \#5 Posted by: onloop Posted at: 2015-11-16T03:28:14.096Z Reads: 462

```
The space cell has a fuse. So it's not too bad, the short will blow the fuse.. But you'd be crazy to put a big lipo on your VESC during configuration. :boom:
```

---
## \#6 Posted by: longhairedboy Posted at: 2015-11-19T14:19:53.975Z Reads: 459

```
Would the charger that comes with the space cell be a good poor man's alternative? What about the 12 volt rails on a PC's internal power supply? 

also, would this work? Its sort of a mini version of the bigger lab power supplies and its only $55 (most are over $300). It looks like it would do ok by putting out up to 30 volts at up to 5 amps. 5 amps should be just fine for no-load bench testing of motors, motor detection, and programming on the VESC, right? 

http://www.amazon.com/Precision-Variable-Adjustable-Digital-Regulated/dp/B00LBOICL8/ref=sr_1_1?ie=UTF8&qid=1447942335&sr=8-1&keywords=lab+power+supply
```

---
## \#7 Posted by: lowGuido Posted at: 2015-11-19T20:32:31.454Z Reads: 444

```
a cheap alternative to a lab power supply is an old computer PSU.
you can convert them into a desk supply quite easily.
you just need to jumper the "on" signal wire from the mainboard to ground to power it on.

this guy has written up a nice how to:
http://www.wikihow.com/Convert-a-Computer-ATX-Power-Supply-to-a-Lab-Power-Supply

If you guys are anything like me you will probably have 4 or 5 old computers laying around waiting to junk so its essentially FREE!.
```

---
## \#8 Posted by: onloop Posted at: 2015-11-19T21:10:36.968Z Reads: 413

```
the main aim here is to have output of low amps and low voltage. a pc power supply can still pack a punch.
```

---
## \#9 Posted by: lowGuido Posted at: 2015-11-19T23:03:26.549Z Reads: 407

```
Every PC power supply is different but most -12V rails are ~0.5A max
```

---
## \#10 Posted by: onloop Posted at: 2015-11-20T00:01:09.037Z Reads: 394

```
oh, ok... well, maybe that is not enough amps... I actually don't know what the minimum is, in Vedder's video he has the lab power supply set to 21v and during the motor spin up it reaches about 4A.
```

---
## \#11 Posted by: BigAl Posted at: 2015-11-20T01:39:40.663Z Reads: 392

```
@onloop so what if I replace the 30amp fuse on the space cell with say a 5 or 10 amp fuse just for the purpose of configuration?  then replace the 30 amp fuse when finished.

Al...
```

---
## \#12 Posted by: onloop Posted at: 2015-11-20T01:45:50.046Z Reads: 370

```
sounds like a really good idea.
```

---
## \#13 Posted by: disastorm Posted at: 2015-11-20T04:34:46.206Z Reads: 364

```
Can a vesc directly connect with a laptop power supply connector or do you need some kind of connector to xt60 converter
```

---
## \#14 Posted by: onloop Posted at: 2015-11-20T05:07:40.973Z Reads: 347

```
the vesc doesn't have the same connection as a laptop, i suppose you could put one on though. The VESC i sell have an xt60
```

---
## \#15 Posted by: longhairedboy Posted at: 2015-11-20T12:54:41.584Z Reads: 349

```
so it sounds like that 5 amp lab power supply i found would probably be ideal. There's also a 10A version just like it for $30 more. both let you dial in current and voltage.
```

---
## \#16 Posted by: kai Posted at: 2015-11-20T13:04:10.532Z Reads: 349

```
ok so changing the fuse to a smaller fuse on spacecell will work as well? what size fuse do you suggest? 5 , 10 or 15 amp? i hope the november batch of vesc is in on time!
```

---
## \#17 Posted by: onloop Posted at: 2015-11-20T23:43:55.043Z Reads: 350

```
Take precaution not to short the vesc and you don't really need to worry about fuses and high amps, but accidents do happen.

With a fuse in the circuit components will still likely get damaged, but hopefully not as bad.
```

---
## \#18 Posted by: longhairedboy Posted at: 2015-11-23T14:42:02.381Z Reads: 344

```
i ordered one of those 30v 5amp lab power supplies, and another one for my older son for christmas. I'm looking forward to using it with both the VESCs i ordered as well as some Arduino stuff i want to mess around with again. I never did finish building my hall sensor based speedometer with digital LED display.
```

---
## \#19 Posted by: evoheyax Posted at: 2015-12-09T17:16:01.229Z Reads: 335

```
@onloop what is so different about configuration and use? Couldn't you "burn" the VESC while in normal operation?

And what is the max amps and max volts one should use to power the VESC during config?
```

---
## \#20 Posted by: fraannk Posted at: 2016-05-24T16:34:36.360Z Reads: 273

```
The lab power supply I have goes to 20V (maybe 24, can't remember) 2A, will this be enough for motor detection on a SK3 168kv?
```

---
## \#21 Posted by: evoheyax Posted at: 2016-05-24T16:50:09.507Z Reads: 254

```
I used a similar power supply and had no issues with motor detection.

According to chaka, another manufacturer of the vesc, you only really need this for the first time you turn it on. After the first time you turn it on, you should be fine using your normal battery.
```

---
## \#22 Posted by: fraannk Posted at: 2016-05-24T16:52:16.256Z Reads: 257

```
So you would recommend doing startup on lab supply, and motor detection on lipo cells? :)
```

---
## \#23 Posted by: evoheyax Posted at: 2016-05-24T16:58:56.615Z Reads: 294

```
I would say it's easier, and you shouldn't have any issues. The only issue you could have by using the lab supply during motor config is if you configure the battery min and max voltages for your battery, the power supply your using may be too low of a voltage (depends on the voltage of your battery of course). If you are giving the vesc less volts than the battery min voltage you have set, you will see a blinking red light, and no motors will spin. You also will likely not be able to get the motors to spin via your controller, as 2 amps is very little. I did do a motor config using the lab power supply at 2 amps and 12 volts, but I had to set my battery min voltage to less than 12 to do so,

Overall, easiest route is to power it on once with the lab power supply, that will charge the capacitors, and then you should be fine using the lipo from there.

It also depends on where you purchased the vesc from. Chaka (ollienboard) powers them before shipping, so lab power supply's are not needed for his.
```

---
## \#24 Posted by: rtasca Posted at: 2016-10-13T14:29:28.940Z Reads: 181

```
For all my stuff testing ESCs I wire a 24V truck headlamp in series with the battery ( up to 6s ) , I even soldered XT male and female plugs and a switch so I can use it easily with anything I need.
```

---
## \#25 Posted by: J-SD Posted at: 2017-02-18T16:43:50.074Z Reads: 143

```
Hi guys, i  linked my esk8.de VESC only a couple of times in USB with my computer, without problems. But 1 hour ago when i plugged my VESC in my laptop, this one shut down, fan 100% spinning, and heatsink really warm (odd considering the fact that it was on only 5 minutes long).
I had to manually disassemble the computer to shut off the battery and stop the fan from spinning. Now the laptop is not charging, not turning on... broken.

Considering that this computer was only 6 months old, was 100% stable under Ubuntu, and precisly shut down when plugging in the VESC. I don't understand something else could be involved !

The VESC himself seems to have issues, it loose it's settings, and was blinking red/blue during the issue. Fault was over voltage with 42,3V (normal, my eskate is 10S) in BLDC. I suppose it transfered somehow this voltage to my computer by USB. Did you heard about a case like this one before ?
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2017-02-18T17:57:51.650Z Reads: 139

```
[quote="J-SD, post:25, topic:491"]
was over voltage with 42,3V (normal, my eskate is 10S)
[/quote]

you should not play with the max voltage... leave it to 57V

also, you might have a problem with you battery or your power source, the 3.3V or the DRV.... since the blue led should always stay on and never blink.
```

---
## \#27 Posted by: J-SD Posted at: 2017-02-18T18:31:05.620Z Reads: 137

```
Don't bother, the VESC must be faulty. Since i use it, it loose his settings all the time, this should have warned me in first place. This costs me 3 Lipos in low voltage because the battery cutoff start that i registered at 34V was set to the defaut 10V rate...
And now I just burn a 6 months old laptop just pluging it on the VESC by USB ! Crazy thing... (and i'm not a newbie considering computer hardware)

I asked to the guy who sold it to me a refund and will buy a new one.
```

---
## \#28 Posted by: High-roller Posted at: 2017-05-15T12:58:48.207Z Reads: 118

```
I realize I'm coming very late to this thread, but if I happen to have one if these:
http://www.meanwell.com/webapp/product/search.aspx?prod=spv-300
Would that work for the initial power-up and programming of the vesc? What voltage should I use?
```

---
## \#29 Posted by: SageTX Posted at: 2017-05-15T19:35:17.284Z Reads: 122

```
That power supply is rated to 25amps.  You would be better served with a laptop supply (4a ~12v).  
The _reason_  you want lower amp supply is to lessen the damage in case of a short on the board, or in a component.
You _could_ wire in some resistors to reduce the load, or use something like this
 
http://ebay.com/itm/131925513356
  to select voltage and power.  
**However** reputable vendors who have tested their VESC®s will have already powered them on once.  Once this is done, the power supply you have would work fine. Or the battery you have for your board would be fine as well.
You only _really_ need to take this precaution if you built the VESC® board yourself or have a cheap knockoff version.
```

---
## \#30 Posted by: High-roller Posted at: 2017-05-16T08:52:43.510Z Reads: 96

```
Thanks for the info! I'm definitely not planning on skimping here, I'm looking at the ones from scramboards with the built-in heatsinks.
```

---
## \#31 Posted by: Maxid Posted at: 2017-05-16T08:55:31.880Z Reads: 92

```
scramboards sells cheap china VESCs - they are not a "reputable" seller
```

---
## \#32 Posted by: High-roller Posted at: 2017-05-16T09:08:52.385Z Reads: 92

```
Who would you recommend besides enertion? Shipping to me from AU makes it less than worthwhile. All I can find on eBay is maytechs.
```

---
## \#33 Posted by: Maxid Posted at: 2017-05-16T09:10:28.251Z Reads: 95

```
https://www.electric-skateboard.builders/t/worldwide-vesc-directory/16764
```

---
## \#34 Posted by: High-roller Posted at: 2017-05-16T09:53:01.970Z Reads: 90

```
Okay, but I see them on that list too. I went with them because of the heat sink, as it gets really hot where I live. what is a decent one without breaking the bank (though I'm well aware of the wisdom of buying expensive only once instead of constant cheap replacements)?
```

---
## \#35 Posted by: Maxid Posted at: 2017-05-16T10:10:09.740Z Reads: 90

```
Hard to say if you don't tell us where you are from
```

---
## \#36 Posted by: High-roller Posted at: 2017-05-16T10:14:41.064Z Reads: 93

```
Sorry, I'm from Israel. It's 28 Celsius now, so imagine what it can get to in August...
```

---
## \#37 Posted by: Maxid Posted at: 2017-05-16T10:41:26.738Z Reads: 96

```
The VESC only gets hot when using high current continously. This is not the case for us. On Average you will use maybe 10-20A with occasional peaks.
```

---
## \#38 Posted by: High-roller Posted at: 2017-05-16T11:22:32.446Z Reads: 104

```
Well, I am putting 8 inch tires on my board for dirt trails, so perhaps that will increase the strain on the vescs?
What makes the scramboards vesc bad? What's​the difference between that and one from, say, DIY?
```

---
## \#39 Posted by: Maxid Posted at: 2017-05-16T11:40:17.337Z Reads: 109

```
https://www.electric-skateboard.builders/t/new-builder-flier-model-vesc/11843

please do some research on your own - there is so much info on this forum. The VESC is not made for Mountainboards.
In your case you should either wait for V6, get a VESC-X or stick to Car ESCs
```

---
## \#40 Posted by: farnamweb Posted at: 2019-05-18T04:00:21.554Z Reads: 40

```
[quote="onloop, post:1, topic:491"]
* Power the VESC using a low voltage low amperage power supply (e.g. from a laptop) when doing motor detection and parameter adjustments in the BLDC tool
[/quote]

Why would the skateboard's battery pack burn the VESC if you are spinning the motor in the tool? Doesn't the VESC pull the correct amount of amps ? 
I always plug in a 6S lipo when I need to test my drone motors.
```

---
## \#41 Posted by: dareno Posted at: 2019-05-18T04:09:44.708Z Reads: 37

```
This is a very old thread and was concerned with early iterations of the vesc.  Its quite safe now to power the vesc via the battery when detecting motors.
```

---
