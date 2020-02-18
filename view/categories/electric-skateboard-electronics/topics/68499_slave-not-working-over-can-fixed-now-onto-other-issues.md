# Slave not working over CAN (Fixed) Now onto other issues

### Replies: 25 Views: 323

## \#1 Posted by: ArnhemAnt Posted at: 2018-09-19T05:17:43.958Z Reads: 90

```
The frustrations continue........
I'm finally at the stage where I can set up my dual ESCapes and begin to enjoy the labour of love (and money).
I am running dual ESCapes and connecting over CanBus. I'm also using the Ackmaniac ESC tool to set these up.
First up, I have the CanBus cable disconnected and set up the master. Motor detection and remote all work beautifully.
Then I power down, disconnect and plug in my slave. Still no CanBus cable connected. Motor detection runs perfectly, then in the App section, I set this ESCape as slave. Power down, disconnect. Then plug in both ESCapes to power after the CanBus cable is connected, however, only the motor from the master is spinning. 
I have gone back into the tool and tried to reset it all again (with CanBus cable disconnected again), yet still no joy. 
I've tried to set the master/slave numbers to all sorts of configurations, but this still has no positive result.
Before posting this, I also searched the forum for answers, but none of the assistance from the previous threads has worked for me. 
I'm a little frustrated and hope that someone with a little more understanding can point me in the right direction. I've attached a few pics to show my current configuration.

Thanks in advance.

Ant
![CanBus1|375x500](upload://WFyfktlREezmMDNxMxoyKIPp1T.jpeg) ![CanBus2|375x500](upload://nNh2qdKCOj98Dbj9QxsNcjW2uIV.jpeg)
```

---
## \#2 Posted by: deltazeta Posted at: 2018-09-19T05:49:20.348Z Reads: 80

```
Cable is wrong, flip one of connections

Had this happen to me too :stuck_out_tongue:
```

---
## \#3 Posted by: ArnhemAnt Posted at: 2018-09-19T06:28:11.250Z Reads: 78

```
Dude. I owe you one - thank you so much. I knew it had to be something simple that I had overlooked, yet I recall reading somewhere that the wires had to be 'crossed'. Either way, I swapped the wires on one of the connectors and it now works - Thank you.

This is my first build and I'm a little concerned about wrecking things. I think I have done everything correctly with the settings for the motors, but maybe it is best for me to share what I have, just in case I've stuffed up somewhere. 
I'm running a dual setup, with the Dark Mater 190kv, 3200w motors. Battery is Li-Ion 12s4p HG2's. From what I understand, I have set things a little 'lower' than they can be, so that I can get a feel for this board. Do you see anything that stands out as being horribly wrong. I am completely open to suggestions.
![Settings5|666x500](upload://cHRgFxNJfsAy5SP7n1eIiheu2sB.jpeg) ![Settings4|666x500](upload://vws12ejdNkaMbvHLjm8ylo99pw7.jpeg) ![Settings2|666x500](upload://2g6sMbZfR9WK9KS3mANFrNpQelD.jpeg) ![Settings1|666x500](upload://g1XXKiPForQltFJtPbImo83PXYL.jpeg) ![Settings3|666x500](upload://zmJv3LEzKTnsElkhcuLvZoy36NL.jpeg) ![Settings6|666x500](upload://nrEvHVvd3eSgG1Cv68hbuL9NcWa.jpeg)
```

---
## \#4 Posted by: Andy87 Posted at: 2018-09-19T06:54:04.078Z Reads: 68

```
I would drop the bat min value a bit down, to -15a or so, but as I´m sure you don´t plan to break for a full charge cycle with -20a should be ok too.
The motor max can be set higher without problems, 60-80a sould be fine too.

As you have a LiIon battery you can set your battery cut off start to 3V per cell and cut off end to 2.8V per cell without issues.
You chose values for Lipo cells but they different form the LiIon values.
```

---
## \#5 Posted by: ArnhemAnt Posted at: 2018-09-19T07:02:33.987Z Reads: 68

```
Thanks Andy,
I'll drop the bat min to -15a as you have suggested.

My main aim with keeping the cutoff start and cutoff end as reflected in the pics was to look after the batteries as much as possible. I am aware that I can bring this down, but I figure, by keeping it a little higher, then there is absolutely no risk of damaging the batteries. Does this sound feasible?
```

---
## \#7 Posted by: Andy87 Posted at: 2018-09-19T07:18:22.220Z Reads: 64

```
the under limit for LiIon cells is 2.5V
the under limit for LiPo cells are 3.3V (as far as I know)

I think with 3V for LiIon you still not super low.
If you wanna safe the max life span for your cells you should also take
care about the max voltage you charge them up.
If I rember right the best range is min 30% max 80% and charging with as min amps as you can.

For sure your cut off settings not wrong. just it will take you like 20-30% of your range.
```

---
## \#8 Posted by: ArnhemAnt Posted at: 2018-09-19T09:11:33.182Z Reads: 55

```
I got everything set up and have changed values as @Andy87 suggested.

A few queries.
1: Rather than having to plug in a USB cord every time I want to make changes, is there a reliable way to make changes via Bluetooth? I've downloaded a few apps but they only seem to show data and not enable me to change things. 
2: If no Bluetooth, once I have CanBUs configured and connected, can I just plug into the master to make changes which will then be applied to both ESC's?
3: (last one).....Initial test ride went well, however, trying to go up a very slight incline, the board just runs out of power. What settings would I need to change to get me rolling? Is it the motor amps or the battery current max??

I know these may come across as very silly questions, but I am really at a loss and just want to get things working so that I can enjoy the ride.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-09-19T09:17:45.438Z Reads: 55

```
no worry we will figure out everything.
you can set your motor and battery values via bluetooth app.
I use eSkate VESC or Xmatic for Iphone. Both can change the settings
for master and slave only motor detection is not possible to run.
Should be possible with other apps too, also android.
If I´m not wrong there should even be a tablet version from the vesc tool out.


About the hill climp.
You have some log file?
I think you already hooked up the bluetooth modul.
Just do that run again and record it. Than look what caused the drop out of power.
(or post the log file screenshot and we can have a look)
There are different things which can cause it.
Overheating of VESC or motor, too much battery sag etc. etc.
```

---
## \#10 Posted by: ArnhemAnt Posted at: 2018-09-19T09:22:32.718Z Reads: 52

```
Thanks heaps for your help. 
I have the Xmatic app for my iPhone but it doesn't seem to allow me to make and write changes. I can see info, but no way to make changes.

As for the hill climb, it's dark now so I'll have to try again in the morning. I didn't record any log file. Not exactly sure how to do that either......
Yeah, I'm a dumb-ass and feel as though I am getting too old to try and learn more stuff - frustrating.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-09-19T09:30:24.202Z Reads: 51

```
Ok yes sorry for the Xmatic i never used the upload thing.
I use this app
![image|230x500](upload://aOlti61UALVtZB7nmFxur8MCFLN.jpeg) 

There you can for sure upload the settings.
And you can start a record file which you can get sent per mail after and analys later on a online platform. It’s quite easy if you once got through it.
There is even a map which will show you on which place you had which values from your vesc.
```

---
## \#12 Posted by: Andy87 Posted at: 2018-09-19T09:32:24.284Z Reads: 48

```
[quote="ArnhemAnt, post:10, topic:68499"]
I’m a dumb-ass and feel as though I am getting too old to try and learn more stuff
[/quote]

No man it’s just getting harder but you know, where is a passion there is a way...
Take your time and ask your things here. 
Nothing will run away!
```

---
## \#13 Posted by: Andy87 Posted at: 2018-09-19T09:39:36.565Z Reads: 47

```
and one more add on ;)
I didn´t used the xmatic app for the last 3month maybe.
but i think there you can also record your trip.
just push the start button on the home screen.
than the stop button when you finished the ride.
I think you can see exactly which values you had in which position, but the max and the min already good to know.
Just start the recording close to your hill.
drive till your board drop out and than stop the recording.
you can read out everything than in your trip screen.
```

---
## \#14 Posted by: ArnhemAnt Posted at: 2018-09-19T10:11:01.783Z Reads: 48

```
[quote="Andy87, post:11, topic:68499"]
I use this app
[/quote]

Thanks for the tip. I've downloaded the app you have mentioned and I will try it out in the morning. I'll let you know how I go.

Thanks again for your help with this. I really do appreciate it.
```

---
## \#15 Posted by: ArnhemAnt Posted at: 2018-09-20T03:55:02.682Z Reads: 35

```
Okay - here's my report from this mornings episodes. Apart from a few little frustrations, I was able to get things up and running and this current setup is fucking scary. Anyway, I'll get to that in a minute....

The eSkate VESC app would not work on my iPhone as it would not connect to my HM-10 Bluetooth, so I deleted it and installed the Xmatic app again. This works with the bluetooth module and it logs the trip, but it did not record data such as speed, distance, etc. GPS is enabled and I can see the trip logged on the map, but there is no data available. I'll see if @Ackmaniac can point me in the right direction with this one.

As for the board - fuck, it is way too quick. Even trying to take off nearly throws me off the back.
My current settings are as follows;
Motor
Current max: 70.00A
Brake max: -20A
Battery
Current max: 70.00A
Regen: -10A

I also have the input V max (in the advanced tab) set to: 45.00V

I tried to set up a throttle curve for my Nano-X but it didn't seem to want to stick and I had to revert back to the standard straight line.

With the above settings, what are some suggestions to try and slightly tame this beast, whilst still enabling it to climb hills?

The dual ESCapes seem quite warm after a short run. I presume this is 'standard'??
```

---
## \#16 Posted by: Andy87 Posted at: 2018-09-20T05:59:24.742Z Reads: 33

```
wow wow wow... wait.
that´s settings for one or for two escapes?

if only for one than you changed some things in the wrong direction.
The settings for one of your escapes should be somiting like this:
Motor max 70 (60)
Motor min -55
Battery max 40 (35)
Battery min -10

in brakets the values I would start with.
If you set 70A for each escape you got the reason why they get hot fast.
and your battery probaly too....

About the app. I had the same issue with my eSkate VESC app, as the Xmatic app still where using the bluetooth signal. I deledet Xmatic, after it was no problem to connect.
```

---
## \#17 Posted by: ArnhemAnt Posted at: 2018-09-20T06:08:20.079Z Reads: 29

```
Shit. Thanks - again. Yeah, I am running a dual ESCape setup. 
Okay, so if I drop just the battery max from 70.00A down to 35/40.00A then that will make a big difference??

Is this the reason that the board wants to kick me off like a brumby?

As for the apps, I tried to delete the Xmatic and just use eSkate, but it still wouldn't connect to the bluetooth, so I reverted back to Mmatic again.
```

---
## \#18 Posted by: ArnhemAnt Posted at: 2018-09-20T06:27:39.588Z Reads: 27

```
One other query. Once I initially set up each ESCape individually, and then connect them via CanBus, do I have to disconnect the CanBus and configure each ESCape every single time I make a small change? Bluetooth doesn't work so i have to use the USB to computer every single time I make a change.
If not, what is the 'correct' way to make small changes each time?
```

---
## \#19 Posted by: Andy87 Posted at: 2018-09-20T06:30:44.876Z Reads: 26

```
it will make the difference that your escapes will not become hot anymore.

make sure that you also set your motor min to -55
if no you will have very weak brakes.

the reason why your board want to kick you off can come from different things.
I think you use the nano x remote. I think you just need to get a bit a feeling for it how much
you can push the trigger. than everything will be good.
if it´s still too much for you, degreese motor max and battery max down till it´s comfortabel for you.
```

---
## \#20 Posted by: Andy87 Posted at: 2018-09-20T06:32:34.038Z Reads: 25

```
you can use the CAN button on the right side of your VESC tool
just connect to the master and from there you can setup your slave via CAN too.
no need to disconnect the can bus every time.
```

---
## \#21 Posted by: ArnhemAnt Posted at: 2018-09-20T06:34:13.901Z Reads: 25

```
[quote="Andy87, post:20, topic:68499"]
no need to disconnect the can bus every time.
[/quote]

That sounds awesome. I gotta say, after the amount of times I have had to disconnect, then reconnect, it is starting to drive me mad. I'll try your recommendation - again - thank you.
```

---
## \#22 Posted by: Andy87 Posted at: 2018-09-20T06:37:33.304Z Reads: 27

```
you can also connect to each vesc by micro usb and update your settings without to disconnect the CAN bus. 
Just don´t switch off one without the other.
If you just change settings and upload them it will not make any problems.
I soldered mine together on one XT90 plug, with it they always switch on together and off together ;)
```

---
## \#23 Posted by: ArnhemAnt Posted at: 2018-09-20T07:40:48.222Z Reads: 24

```
Thanks @Andy87, you have been a huge help over the last few days. I've just made the changes you suggested and the board feels a lot better now. Still pretty 'angry' but a lot more controllable.

The setup over CanBus didn't work, but I just plugged USB in each ESC one at a time and got through it that way.
 
Tomorrow I will ride some more so that I can start to get used to this board.
```

---
## \#24 Posted by: Andy87 Posted at: 2018-09-20T07:50:34.546Z Reads: 24

```
have a nice ride ;)
```

---
## \#25 Posted by: Sender Posted at: 2018-09-20T08:32:07.838Z Reads: 22

```
Also don't forget to calibrate your nano x everytime you turn it on

1.  Turn on remote, go full throttle, full brake 

2. Turn on Board

And yes going from 70 motor max down to 35 or 40 will make a big difference.
```

---
## \#26 Posted by: ArnhemAnt Posted at: 2018-09-20T10:35:58.949Z Reads: 20

```
Thanks man. Yeah, I've been aware of the calibration, every single time I turn the darn thing on....Believe me, it's been a LOT over the last few days. LOL.
```

---
