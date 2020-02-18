# My board suddenly stop braking down a hill

### Replies: 48 Views: 1586

## \#1 Posted by: Silverline Posted at: 2017-07-27T17:20:08.266Z Reads: 160

```
Hallo
Yesterday when i was out riding my board, the motor-breakes stopped working two times, when i was going down a hill and was braking maybe 50-70% at the same time. This was pretty crazy, and it threws me of my board both times.

My setup is a single motor (270kv) on 6s lipo, with a VESC 4.12 from esk8.de (running 2.18fw)

I have attached my settinngs, that i was running with. The funny part is though, that after these two episodes, when i was connecting my computer today to se, the first page in BLDC was set back to default settings, the same goes for the motor detection parameters ??

I have tried with both fault and faults in the terminal, and their is none.

Any help is appreciated
Thanks<img src="/uploads/db1493/original/3X/8/a/8a8055bc461224cec2744dab998da2ca557964f9.jpg" width="690" height="387"><img src="/uploads/db1493/original/3X/2/d/2d9b7c9ede5210713a1e3f122d2c6589048109fe.jpg" width="690" height="387"><img src="/uploads/db1493/original/3X/8/9/896279392313d7448a62aa7429c8cadd124290c6.jpg" width="690" height="387">
```

---
## \#2 Posted by: Martinsp Posted at: 2017-07-27T17:25:44.675Z Reads: 146

```
Hello, 
first of all, didnt you forget to read the configuration (silly but just to get the obvious stuff out of the way)
and can you reproduce this problem at slower speed? The point is to tell how long does it take the VESC to work properly again. If it is a fault it would take like 3 seconds to work again for non-latching errors. Or other option is to try to reproduce it without crashing and turning of the board connect it to the BLDC tool and check for faults in the terminal tab.
```

---
## \#3 Posted by: Silverline Posted at: 2017-07-27T17:30:43.195Z Reads: 143

```
Hallo Martin
Yes i remember to click the read buttom first :slight_smile: (or else all the parameters on the first page is just 0 )
The board is working right after the failure again. So are you saying, that in order to get the fault code from the terminal, this must be done before turning of the board ?
```

---
## \#4 Posted by: Martinsp Posted at: 2017-07-27T17:33:08.114Z Reads: 138

```
Yes because it is stored in a memory that resets itself when turned off unlike the part of storage that keeps your settings etc even when off.
```

---
## \#5 Posted by: thisguyhere Posted at: 2017-07-27T17:34:36.374Z Reads: 130

```
when you were going downhill, was your battery fully charged?
```

---
## \#6 Posted by: Martinsp Posted at: 2017-07-27T17:35:00.299Z Reads: 127

```
What I used to do is just go out and try to get the problem to occur at as slow speed and as close to home as possible and just pick the board up and go home to see WTF is wrong again! :D :D JK :D 
BTW: it seems too popular and even more stupid, some people ride with their laptop to see realtime data... dont be one of them, be wise before you hurt yourself :( :D
```

---
## \#8 Posted by: Silverline Posted at: 2017-07-27T17:38:20.355Z Reads: 125

```
@Martinsp But it happens only two times, with no pattern.

@thisguyhere Sorry i forgot to mention that both time, the battery was about 40-70% full.

@SORRENTINO Sorry but i don`t understand what this has to do with my problem ?? I know for a fact, that both times it happen the battery was not flat, nor was it fully charged ?????
```

---
## \#9 Posted by: Martinsp Posted at: 2017-07-27T17:40:18.865Z Reads: 116

```
@SORRENTINO It is not low, What you say is wrong actually. because at 4.2V you have 25.2V so 26.4 is probably a mistake.

Wasnt it a loss of signal with your receiver? I know that in my area there are a few spots where the signal is as if jammed or interrupted heavily. Cant that be the case?
```

---
## \#11 Posted by: Martinsp Posted at: 2017-07-27T17:43:15.211Z Reads: 108

```
His cutoff (the upper one i think is what you are saying) is set in the picture at 57V which is more then twice his voltage
```

---
## \#12 Posted by: Silverline Posted at: 2017-07-27T17:44:31.245Z Reads: 106

```
I have the Winning remote (new version bla bla bla :-P ) And i suspect that maybe that could be my problem ? I have read about lot of people with problems using this remote. But when the vesc has been resetting some settings to default, i thought that this could not be the case. I have btw. put a ferrit on my servo lead.
```

---
## \#14 Posted by: Martinsp Posted at: 2017-07-27T17:46:25.830Z Reads: 101

```
@SORRENTINO The battery cutoff start is when the VESC will decrease the power output to give you some more range and to lower the voltage sag (it is bigger with high power/more amps) not an overcharge protection.
```

---
## \#16 Posted by: Martinsp Posted at: 2017-07-27T17:49:36.107Z Reads: 94

```
@Silverline I have that ferrite ring on my setup too but it is still happening (the ferrite ring does not prevent loss of signal just interruption of the "data" transfer from your receiver to your VESC meaning it does notaffect the communication between your antena and remote)
There is only one way to find out, go to the same place and try it, this time be prepared to avoid crash if it happens again. And just to be sure check for faults afterwards. If no faults are saved you found your problem most likely.
```

---
## \#17 Posted by: Martinsp Posted at: 2017-07-27T17:50:31.364Z Reads: 94

```
@SORRENTINO please show me where it says that you are right? I am pretty sure that this information is in Benjamins video on his youtube channel. Go check it out.
```

---
## \#18 Posted by: wafflejock Posted at: 2017-07-27T17:57:19.761Z Reads: 93

```
No he's not wrong battery cut offs are for ramping power down I set mine at 3.6-3.8 per cell so it begins reducing power at 3.8 and cuts off power completely at 3.6 (average) per cell (conservative)
```

---
## \#19 Posted by: Martinsp Posted at: 2017-07-27T17:58:47.591Z Reads: 96

```
@SORRENTINO I like how you were saying I was wrong and the lol at the end got me. :)  skip to 34:15 and educate your self before you try to help someone or point fingers at someone and say they are wrong. I am not trying to be mean just think before you say something that could harm someone in any way. Thank you :)
https://www.youtube.com/watch?v=5HLZaMcYRuY&list=PLICpQdAXJazRzoXJByGA_5wd-B4cifmbh
```

---
## \#20 Posted by: Martinsp Posted at: 2017-07-27T18:00:30.991Z Reads: 93

```
Lets bring this thread back on track shall we? @Silverline so what do you think you are going to do?
```

---
## \#21 Posted by: Silverline Posted at: 2017-07-27T18:01:17.189Z Reads: 87

```
I was hoping you guys could tell me that :-/
```

---
## \#22 Posted by: wafflejock Posted at: 2017-07-27T18:06:18.695Z Reads: 87

```
I just grabbed a Bluetooth modules for the metr app for remote telemetry to try and get more data and see if I can gather more info about the occasional 👻 but could have either been EMI or something coming physically loose due to vibrations over time... What did you do to get it to reconnect, anything?
```

---
## \#23 Posted by: Martinsp Posted at: 2017-07-27T18:07:31.284Z Reads: 91

```
I personally would take my friend with me to carry my notebook on a bike or longboard or whatever (so that you dont destroy it in your backpack in case of a crash) and after it happens check the faults and if it happens in the same place. If you dot have someone like that you can always just walk home or bus etc.. 
After there is no fault you pretty much have the only problem left and that is the signal loss for whatever reason that you cant most probably cant avoid. Try putting the antenna on the very edge of your board so that it wont be affected by the powerrwires.
```

---
## \#24 Posted by: Silverline Posted at: 2017-07-27T18:41:01.716Z Reads: 84

```
I have the Metr app. And will try using that...


And maybe it`s the Winning remote (i have the GT2B remote in the mail)
But don`t you guys think it`s pretty od, that the vesc is going back to default settings by its own, after my braking failure ?
```

---
## \#25 Posted by: Martinsp Posted at: 2017-07-27T18:44:04.270Z Reads: 80

```
I completely forgot! Then the problem might be your firmware. Try updating that to the newest version. Just search for firmware there is a thread where people put the newest bestesteset firmwares :D try that hope it works for you :/
```

---
## \#26 Posted by: Jinra Posted at: 2017-07-27T18:44:54.931Z Reads: 75

```
Could you link/take a pic of your remote?

Also did you configure min/max PPM on the PPM page of BLDC tool? if you didn't and your PPM signal gets lower than the minimum on the tab, the VESC can cut out.
```

---
## \#27 Posted by: Silverline Posted at: 2017-07-27T18:49:01.519Z Reads: 77

```
@Jinra  I have this remote : https://www.aliexpress.com/item/Wholesale-New-arrival-2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32678995218.html


When i push my remote al the way down on the bench, the gui shows 1%, mid position is around 50 % and max 100 %
```

---
## \#28 Posted by: Jinra Posted at: 2017-07-27T18:51:13.492Z Reads: 79

```
You want to make sure the actual PPM value (not %) is not lower than minimum PPM on BLDC. However, I would toss that remote immediately. It's the cause of many an injury on the forum including myself. That is the winning v1 remote which is notoriously unreliable.
```

---
## \#29 Posted by: Silverline Posted at: 2017-07-27T19:07:35.251Z Reads: 75

```
@Jinra
I would blame the remote 100% for the failure under normal circumstances, hence why i have GT2B remote in the mail.
But the "reset to default bug" got me thinking that something else is wrong ?
```

---
## \#30 Posted by: darkkevind Posted at: 2017-07-27T19:14:59.374Z Reads: 71

```
Just to throw a spanner in the works here, I have the benchwheel remote, which I've been having no problems with for about 8 months on my previous setup, everything the same except running 6s 5000mah 25c Lipos.
Now I'm running 8s4p 80A Li-ions and I've had this issue maybe twice now.

If I'm going along, and then almost 'slam' on the brakes, it seems like the VESC powers down and I have zero control, and then I gain control again in a couple of seconds. Then if I'm gentile with the brakes, ie. apply gradually, it's fine.

To add to this, sometimes (not always) when I'm accelerating hard, (maybe up a tiny bt of an incline), it will cut out too. Thrown me off my board a couple of times.

I think this may be a similar issue. My motor is rated at 60A but my battery can deliver 80A, does this have anything to do with it? Max motor in BLDC is set to 60A.
```

---
## \#31 Posted by: Silverline Posted at: 2017-07-27T19:23:51.656Z Reads: 68

```
@darkkevind  Cut off for a second going up a hill with almost full throttle, is something i also has tried. My amp motor max is set to 50amp in BLDC, but looking at the recording in the metr app afterwards, is only showing amp peak at 33amps.... hmmmm
```

---
## \#32 Posted by: darkkevind Posted at: 2017-07-27T19:26:13.077Z Reads: 65

```
Interesting..... :thinking:
```

---
## \#33 Posted by: Jinra Posted at: 2017-07-27T19:29:32.093Z Reads: 64

```
Sounds like it's rebooting, might be overcurrent from braking going over the absolute maximum
```

---
## \#34 Posted by: darkkevind Posted at: 2017-07-27T19:33:12.423Z Reads: 65

```
Absolute max being the default 130A you mean? or going over the motor min I gave it?
```

---
## \#35 Posted by: Jinra Posted at: 2017-07-27T19:37:46.405Z Reads: 65

```
Do you have a UART module and app for it? You could try getting it to happen to see what fault code you encounter. I'm just guessing it might spike over the 130A absolute maximum, but I'm not sure.
```

---
## \#36 Posted by: darkkevind Posted at: 2017-07-27T19:39:31.951Z Reads: 67

```
I don't :frowning:

How do I sort that out?
```

---
## \#37 Posted by: Jinra Posted at: 2017-07-27T19:40:12.712Z Reads: 67

```
It's tough because since it sounds like your VESC is rebooting the error code with flush and clear when that happens, you'll only have a moment to see what error code it's giving you.
```

---
## \#38 Posted by: Silverline Posted at: 2017-07-27T21:04:18.039Z Reads: 61

```
So things that i will try now to resolve my problems is.

1. Change the Winning remote to GT2B remote, and do the sparkle "hack" case mod.
2. Flash my VESC with the custom firmware from @Ackmaniac to se if this changes anything. Also to get a more natural throttle curve, without the "turbo boost" i have now.
```

---
## \#39 Posted by: Jinra Posted at: 2017-07-27T21:06:21.151Z Reads: 61

```
You can also get the benchwheel or nano v2 remotes. Those have proven to be very reliable.
```

---
## \#40 Posted by: Silverline Posted at: 2017-07-27T21:08:31.090Z Reads: 63

```
I could not find the benchweel including the RX (I`m from EU) and people seems to like the GT2B, so....
```

---
## \#41 Posted by: Jinra Posted at: 2017-07-27T21:12:45.569Z Reads: 62

```
Just giving you additional options that don't need to be modded :) DIYES sells the nano v2 and ships to EU i believe.
```

---
## \#42 Posted by: darkkevind Posted at: 2017-07-27T21:14:55.322Z Reads: 63

```
You can't actually get the benchwheel receiver now :frowning:
```

---
## \#43 Posted by: Jinra Posted at: 2017-07-27T21:17:03.726Z Reads: 65

```
Weird, I'm sure they'll have it up again eventually. Good thing I stocked up...
```

---
## \#44 Posted by: ShaunPieso Posted at: 2017-07-27T21:23:14.475Z Reads: 65

```
If any of you guys is interrested I use this APS remote and it is absolutely bulletproof.. I had a bunch of other RC remotes and this one is the best! http://alienpowersystem.com/shop/radio-transmitters/alien-power-system-2-4ghz-electric-skateboard-remote-control/ and it is in stock!
```

---
## \#45 Posted by: darkkevind Posted at: 2017-07-27T21:57:51.984Z Reads: 58

```
Too big and expensive imo

@Jinra you selling any?
```

---
## \#46 Posted by: ShaunPieso Posted at: 2017-07-27T21:58:54.273Z Reads: 60

```
Yeah it is not the smallest one :D I cant find a 3D printable design of a mod :(
```

---
## \#47 Posted by: darkkevind Posted at: 2017-07-27T22:00:50.034Z Reads: 62

```
G2tb sparkle mod is the smallest I think. Can't go wrong with the mini remote or g2tb.

Benchwheel has been bullet proof for me... Once my initial problems were sorted.
```

---
## \#48 Posted by: Jinra Posted at: 2017-07-27T22:49:55.696Z Reads: 62

```
Sorry using them as spares right now. Plus, aren't you in EU? Shipping from California would be killer.
```

---
## \#49 Posted by: darkkevind Posted at: 2017-07-27T23:00:26.062Z Reads: 61

```
Nah would only be about $10-15
```

---
## \#50 Posted by: Jinra Posted at: 2017-07-27T23:01:25.100Z Reads: 64

```
I'll let you know if I decide to part ways with one then :)
```

---
## \#51 Posted by: darkkevind Posted at: 2017-07-28T04:36:21.248Z Reads: 60

```
Oh! I forgot to mention... This only happens in BLDC mode, when I was running FOC it seemed slightly less powerful but it never happened under the same circumstances....

But my motor doesn't seem to like FOC which is why I changed back...
```

---
## \#52 Posted by: Silverline Posted at: 2017-07-28T15:27:59.591Z Reads: 50

```
first part done :slight_smile:<img src="/uploads/db1493/original/3X/f/c/fc9eef9743f0ded9ee900b6d573eb9850920f3e6.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/f/f/ff69346e01033393c1dc83bd06aca3db90062109.jpg" width="690" height="388">
```

---
