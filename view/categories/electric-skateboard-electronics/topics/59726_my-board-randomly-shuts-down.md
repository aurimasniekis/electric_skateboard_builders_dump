# My board randomly shuts down

### Replies: 19 Views: 743

## \#1 Posted by: taz Posted at: 2018-06-22T13:33:54.548Z Reads: 145

```
Does the metr.at also record faults while recording?
I have a problem with my board randomly shutting down.
If I turn it off and on then it may work properly (sometimes it does not).
There is no correlation on what the board was doing before it shuts down. I may be accelerating, braking or simply coasting. It may be cold or hot.
Last time it happened while I was practicing foot braking.
The record is here:

https://metr.at/r/ix9mp

You will see towards the end all the parameters went to 0 but I see no fault codes recorded.
It looks like the board had no power however the battery meter on the board was showing proper voltage.
At the time I did not know about the terminal in the app to check for faults.

The board is an eskating beast with 12S5P battery. (dual 6355, focboxes, metr.at module etc).
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-06-22T14:48:19.961Z Reads: 121

```
Cold solder?
```

---
## \#3 Posted by: taz Posted at: 2018-08-29T16:55:04.267Z Reads: 88

```
So I had lots of problems lately and I traced them down to broken series connections.
I fixed them and the board now works but this problem happened again today.
https://metr.at/r/MylcF?zoom_start=2080&zoom_end=2262
The board shut down, the display on the board showed the correct voltage, the connection light on the remote was on. No faults have been recorded on the metr.at app.
Do you guys have any ideas what the problem could be?
```

---
## \#4 Posted by: taz Posted at: 2018-08-29T21:28:13.380Z Reads: 77

```
Anyone?
10 char
```

---
## \#5 Posted by: Ackmaniac Posted at: 2018-08-29T22:07:03.865Z Reads: 72

```
Just need more info. Does it shut down only for a second or entirely. Do you feel a immediate power loss. Does it happen when you accelerate or brake or when you ride on rough roads only?
```

---
## \#6 Posted by: Jake2k17 Posted at: 2018-08-29T22:08:07.122Z Reads: 69

```
Maybe another broken connection?  Check all solders
```

---
## \#7 Posted by: taz Posted at: 2018-08-30T07:03:57.549Z Reads: 67

```
It shuts down entirely. Most of the times it is while coasting or slight braking.
Although I take my board over some cobblestones during my rides it has never happened there.
If you need any more information let me know.
```

---
## \#8 Posted by: Jebe Posted at: 2018-08-30T07:13:52.983Z Reads: 64

```
I don't know about the metr app, ack's app records faults well. I had a problem where the board would shut down, still showing battery life, and needed to be powered off then up again and rode. Ran Ack's ap and saw that a low voltage fault was being recorded. My problem was a bad connection in the  on/off switch switch circuit, was momentarily opening, enough to trigger the low level cut off.
```

---
## \#9 Posted by: taz Posted at: 2018-08-30T07:18:31.963Z Reads: 63

```
It could be, although I have already done that it is worth rechecking.
When I had the broken series connections I would get an over voltage error.
This problem must be something different since it has plagued the board since the beginning, is entirely random and does not produce any faults in the metr.at app.
```

---
## \#10 Posted by: taz Posted at: 2018-08-30T07:21:00.994Z Reads: 60

```
This sounds exactly like my problem.
What type of switch do you have?
I run a Bestech BMS (charge and discharge) that has an electronic switch.

I can't run Ackmaniac's app at the time. My phone runs android oreo so it can't connect with the Bluetooth module and I use my old iphone to connect to it. I searched for Ackmaniac's software on the App store but could not find anything so I guess there is only an Android version.

I have ordered a metr pro module so when it arrives I will be able to run Ack's app too.
```

---
## \#11 Posted by: Jebe Posted at: 2018-08-30T07:25:59.585Z Reads: 56

```
am using a fet eswitch -  problem was with my connection to it - hot glue seems to have resolved it - touch wood.
```

---
## \#12 Posted by: taz Posted at: 2018-08-30T07:35:14.723Z Reads: 53

```
Do you have a BMS for discharge?
```

---
## \#13 Posted by: Jebe Posted at: 2018-08-30T09:37:56.884Z Reads: 48

```
yes - had a good run on the board since redoing the switch connection and haven't had an issue - BMS cut out at 28 volts I think so it could have been. Did not see voltage gradually drop on the app data ( csv export ) looked like it just dropped. was dropping out at various times - not just under load.
```

---
## \#14 Posted by: DavidBanner Posted at: 2018-08-30T11:43:01.951Z Reads: 44

```
[quote="taz, post:10, topic:59726"]
searched for Ackmaniac’s software on the App store but could not find anything
[/quote]

look for "esc monitor" in the play store or go direct via this link https://www.google.co.uk/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&cad=rja&uact=8&ved=0ahUKEwivnPOw85_WAhUoDMAKHQHMDpwQFgg5MAI&url=https%3A%2F%2Fplay.google.com%2Fstore%2Fapps%2Fdetails%3Fid%3Dackmaniac.vescmonitor%26hl%3Den_GB&usg=AFQjCNEAgx3BBXYCkyL1Q9cYrxyscFIdsg
```

---
## \#15 Posted by: taz Posted at: 2018-08-30T11:45:38.467Z Reads: 40

```
[quote="taz, post:10, topic:59726"]
I can’t run Ackmaniac’s app at the time. **My phone runs android oreo so it can’t connect with the Bluetooth module** and I use my old iphone to connect to it. I searched for Ackmaniac’s software on the App store but could not find anything so I guess there is only an Android version.
[/quote]

:wink:
10ch
```

---
## \#16 Posted by: DavidBanner Posted at: 2018-08-30T11:49:11.951Z Reads: 40

```
missed the iOS bit when reading.

but there are bt modules that work with droid 8 other than the ones supplied with metr...

iOS apps:
https://itunes.apple.com/US/app/id1155084982?mt=8

https://itunes.apple.com/us/app/eskate-vesc/id1276043481
```

---
## \#17 Posted by: Jake2k17 Posted at: 2018-08-30T21:15:16.237Z Reads: 32

```
Bro if I were you and that desperate, I would just bypass the bms for discharge and get an anti spark switch
```

---
## \#18 Posted by: sayekim Posted at: 2018-08-30T21:47:49.944Z Reads: 30

```
I think it is still some battery connection or indeed a switch connection problem. 
Check the battery again. If that checks I would try a different switch or a loopkey.
```

---
## \#19 Posted by: taz Posted at: 2018-08-31T06:06:51.669Z Reads: 27

```
Lol, I am not into despair, yet.
I could bypass the BMS again but I would only do if it will help isolate the problem.
Discharging through a BMS gives you some extra level of safety such as individual p group voltage monitoring that simply is not (easily) possible otherwise.
The most difficult part about this particular problem is that it is completely intermittent.
For example I have made 30km after the last time it happened going over cobblestones, steep hills etc and the bloody thing works great but I know that it will happen again at some point.
```

---
