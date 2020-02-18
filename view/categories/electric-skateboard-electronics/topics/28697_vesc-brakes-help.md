# Vesc brakes help

### Replies: 47 Views: 2352

## \#1 Posted by: Bloop Posted at: 2017-07-26T18:02:54.835Z Reads: 145

```
He i tested my eboard today and my breaks are kinda too strong and is not something linear. No matter how much i slide from the remote control it breaks so hard. 

Any opinions for a smoother breaking ? I will post in a few h my settings but are the default from enertion.
```

---
## \#2 Posted by: jmasta Posted at: 2017-07-26T18:04:13.509Z Reads: 145

```
Did you run motor detection?
```

---
## \#3 Posted by: darkkevind Posted at: 2017-07-26T19:12:15.149Z Reads: 134

```
Quite possibly your motor - amperage is too high. What's your motor max/min ?
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-26T19:19:42.941Z Reads: 132

```
What remote do you have
```

---
## \#5 Posted by: Alan_Smithee Posted at: 2017-07-26T19:24:47.041Z Reads: 127

```
post screenshots of you bldc tool if you can
```

---
## \#6 Posted by: Bloop Posted at: 2017-07-26T19:45:04.868Z Reads: 125

```
Ok i just got home here are my settings. I have remote x nano from enertion.

Also i think i should increase the motor max to 60A since i was going full throttle and my board just stoped accelerating ? i guess my vesc cut off the power cause the motor was draining more than 40A ?? 


<img src="/uploads/db1493/original/3X/5/b/5b3d62ddae8ecfcf92b28b37b0242301c71a64d3.png" width="690" height="417">

<img src="/uploads/db1493/original/3X/f/5/f54accae79012d5a68b478f5eb1fae55cd3ff1a6.png" width="690" height="478">

<img src="/uploads/db1493/original/3X/8/3/835575ad4355bba94fba6b4ce42d7c7582192e96.png" width="690" height="411">

<img src="/uploads/db1493/original/3X/f/2/f2928361783db13226caf9f2461ac66237fcbbfb.png" width="690" height="433">
```

---
## \#7 Posted by: Bloop Posted at: 2017-07-26T19:46:19.110Z Reads: 111

```
is only 40A ... and im thinking to make it to 60A since my motor can drain max 60A .. am i wrong ?
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-26T19:47:17.267Z Reads: 109

```
max input voltage should be 57 (default) don't change it.
```

---
## \#9 Posted by: darkkevind Posted at: 2017-07-26T19:48:12.932Z Reads: 107

```
If your motor's max is 60A then yeah, change Motor Max to 60A.

Have you calibrated your controller?

If not, go here: https://youtu.be/OtuofrQr3F8
```

---
## \#10 Posted by: Bloop Posted at: 2017-07-26T19:48:53.307Z Reads: 108

```
i changed nothing . this are all my default settings except the ones from motor detection
```

---
## \#11 Posted by: darkkevind Posted at: 2017-07-26T19:49:32.281Z Reads: 109

```
42v is not default, is your VESC old?
```

---
## \#12 Posted by: Bloop Posted at: 2017-07-26T19:49:51.027Z Reads: 104

```
yes did that too and forward will go to max same for backward i added the values there
```

---
## \#13 Posted by: SORRENTINO Posted at: 2017-07-26T19:49:59.183Z Reads: 103

```
You need to turn your nano x remote on and push till full throttle and then push to full brake. Then turn board on and bind. You need to calibrate the remote everytime you autobind. Same thing happened to me lol.
```

---
## \#14 Posted by: Bloop Posted at: 2017-07-26T19:50:13.809Z Reads: 103

```
i got it last year in december i think
```

---
## \#15 Posted by: darkkevind Posted at: 2017-07-26T19:50:32.121Z Reads: 100

```
Ahhhh yes! I remember this issue. That really sucks about that controller...
```

---
## \#16 Posted by: Bloop Posted at: 2017-07-26T19:51:26.591Z Reads: 100

```
i never heard about this.. i will test it out tomorrow .. hmm i had no idea you need to calibrate the remote...
```

---
## \#17 Posted by: Jinra Posted at: 2017-07-26T19:52:18.327Z Reads: 98

```
That's why I asked which remote you had. See full details here

http://www.electric-skateboard.builders/t/nano-v2-full-review/25159/20

But yea change your max input voltage to 57v
```

---
## \#18 Posted by: Bloop Posted at: 2017-07-26T19:53:15.607Z Reads: 99

```
battery cutoff should be at 42V right ? i guess that's why my board just stoped when i accelerated
```

---
## \#19 Posted by: SORRENTINO Posted at: 2017-07-26T19:56:56.677Z Reads: 106

```
You know what the Nano x failsafes to if it loses signal or powers off?
```

---
## \#20 Posted by: Jinra Posted at: 2017-07-26T20:00:26.816Z Reads: 108

```
There is none, it just glides. I also haven't had success in turning the remote back on to pair again unless you reboot the receiver as well
```

---
## \#21 Posted by: Jinra Posted at: 2017-07-26T20:01:24.818Z Reads: 108

```
Battery cut off should **not** be 42v. 33/30 is a good figure for li-ion 18650 cells, but I use 30/27 myself. If you're running lipo 37/35 is a good number
```

---
## \#22 Posted by: Bloop Posted at: 2017-07-26T20:02:17.219Z Reads: 110

```
while i was riding today i saw that the board was accelerating and when i stop accelerating the board will kinda break .. is this normal ? (i guess)
```

---
## \#23 Posted by: Bloop Posted at: 2017-07-26T20:04:17.649Z Reads: 108

```
ye i have 10s4p li-ion 18650. so i have 42v from the battery. why would i have max voltage at 57 if my battery can give max 42V and why the cutoff that low at 30 is kinda out of juice
```

---
## \#24 Posted by: Jinra Posted at: 2017-07-26T20:20:48.934Z Reads: 109

```
[quote="Bloop, post:22, topic:28697, full:true"]
while i was riding today i saw that the board was accelerating and when i stop accelerating the board will kinda break .. is this normal ? (i guess)
[/quote]

Are you sure that wasn't just because of the drag of the motors/belt that you felt like it "braked"?

[quote="Bloop, post:23, topic:28697, full:true"]
ye i have 10s4p li-ion 18650. so i have 42v from the battery. why would i have max voltage at 57 if my battery can give max 42V and why the cutoff that low at 30 is kinda out of juice
[/quote]

Because if you go over the value you put in there the VESC turns off and errors out. You can get voltage spikes from braking so it's wise to leave it at default 57v. There's no benefit to changing this at all.

30v is a bit low but a 10s pack can go as low as 25v. If I'm miles out from home and my batteries are low, i'd still want them to be able to take me back. That said, I try to never go below 3.4v/cell on my pack.
```

---
## \#25 Posted by: Bloop Posted at: 2017-07-26T20:27:13.465Z Reads: 108

```
So this should be a better configuration right ?? 

Or should i keep the batmax and bat min to 25A/-12A. Hmm honestly i have  no idea why are they so low.. in all other examples pll usually used same value for motor max bat max and same value for motor min and bat min . 

What values would you recommend ?

<img src="/uploads/db1493/original/3X/3/8/385099dd09dc5c8f575881b3cad45129aa7d6066.png" width="690" height="417">
```

---
## \#26 Posted by: Jinra Posted at: 2017-07-26T20:31:28.755Z Reads: 103

```
Honestly I would use @Ackmaniac's f/w instead of stock for better throttle control

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286

For current limits yours are okay, but you're battery min is too high, a 10s4p setup can take -16A regen current, though you'll regen so little it probably doesn't make a difference even if it were a little higher. I usually keep my motor min 10 amps less than my motor max too. In this case -50A.
```

---
## \#27 Posted by: Bloop Posted at: 2017-07-27T12:39:14.171Z Reads: 87

```
Hey guys thank for help. I've done some more testings today indoor and i still have some things unclear.

<img src="/uploads/db1493/original/3X/f/4/f4363fb009e65b1252adc06ebdb7bf794088a5ff.png" width="690" height="440">


Here are my latest settings. Hopefully this time they are ok.

My problem:
1. When i move the throttle just a little bit it will start accelerating and continue till it goes to max... so im getting to max with just a little bit of throttle ...
After it gets to max i tried to push it further but no change in rpm or in sound... so thats how i knew it was at max..
a) i did calibrate the remote before i turn my board on 
b) i did the setup with min/max pulsewidth from bldc tool 

am i missing something ?? 


1. i watched the real time data graph from bldc tool and when i break again no matter how hard it will get full breaks on me.. is this normal ? shouldn.t it be in steps depending on how hard i move the throttle ?? 

Thank you.
```

---
## \#28 Posted by: Silverline Posted at: 2017-07-27T12:53:57.451Z Reads: 83

```
Remember also to change your min / max Erpm to 60.000. With a dead / defective DRV chip, you also get weird behaviour
```

---
## \#29 Posted by: Bloop Posted at: 2017-07-27T13:03:34.658Z Reads: 81

```
ok now i hae the erpm to 60.000 but still the same behavior ...  im pushing the throttle really slow to the first position where the motor starts spinning and it will start accelerating to the max .. i was on the realtime data that my erpm it going to 52.000 ..


honestly im expecting it to accelerate when im pushing the throttle more not accelerate on it.s own ?? am i wrong ?
```

---
## \#30 Posted by: Okami Posted at: 2017-07-27T13:11:37.203Z Reads: 74

```
I think there should be seperate tab to see what, your remote does (what signal vesc receives)

So if u can u might as well check that, though.im still an outsider with vesc, but that is what i would look for.
```

---
## \#31 Posted by: rpn314 Posted at: 2017-07-27T13:15:57.401Z Reads: 78

```
[quote="Okami, post:30, topic:28697"]
I think there should be seperate tab to see what, your remote does (what signal vesc receives)
[/quote]

I think you're referring to the display window in a few of the Application tabs (PPM in this case). Here:
[quote="Bloop, post:6, topic:28697"]
https://www.electric-skateboard.builders/uploads/db1493/original/3X/8/3/835575ad4355bba94fba6b4ce42d7c7582192e96.png
[/quote]

@Bloop It looks like the checkbox next to "Display" in this screen shot is unchecked here. I didn't see any comment indicating you'd done much with that box, so can you check it (click it) and do a test (maybe take a video and upload it to youtube or something so we can see it) of that bar when you're slowing going from the middle of the throttle, up to the top, back to the middle, and then the same to the bottom?
```

---
## \#32 Posted by: Okami Posted at: 2017-07-27T13:23:47.686Z Reads: 73

```
Yep, this is to what I was refering to ;) @rpn314 

I wasnt sure he knows about it, so I thought it is a good idea to take a look at it.
```

---
## \#33 Posted by: Bloop Posted at: 2017-07-27T13:31:43.281Z Reads: 71

```
i did check that forgot to update the picture. Here are my new values.

I will make a video shortly so show what i mean ... 

<img src="/uploads/db1493/original/3X/0/9/09f2c6ba469fd4c2169db9af6b8c5e68e057666c.png" width="690" height="431">
```

---
## \#34 Posted by: rpn314 Posted at: 2017-07-27T13:36:02.443Z Reads: 68

```
That's fine. I wasn't worried about the screen shot, just wanted the video to try and help :slight_smile:  Checking it doesn't change anything on the VESC; it just displays that info in BLDC tool. It's quite useful for issues like this. Awaiting your video :nerd: :popcorn:
```

---
## \#35 Posted by: L3chef Posted at: 2017-07-27T13:38:50.688Z Reads: 65

```
Does your motor have hall sensors? It say that hall sensor detection failed.
Run the detection again and do the read/write configuration and reboot.
```

---
## \#36 Posted by: Jinra Posted at: 2017-07-27T13:43:23.310Z Reads: 64

```
I'm surprised no one mentioned that this is expected behavior. Current control mode will always ramp up to full speed of it overcomes load. Bench testing will always get you max speed at low throttle since there's virtually no load. Same for braking. You'll see much different behavior when you actually ride the board, but the speed will still not be throttle dependent.

Remember, the throttle controls acceleration, not speed.
```

---
## \#37 Posted by: Bloop Posted at: 2017-07-27T13:50:02.651Z Reads: 63

```
i have no sensor
```

---
## \#38 Posted by: Bloop Posted at: 2017-07-27T13:52:05.319Z Reads: 64

```
oh i see now. well so even when i will ride it . it will eventually accelerate to max even if im only pushing a little on throttle ?? 

is there a better more so it will maintain my speed unless i push further the throttle ??
```

---
## \#39 Posted by: Jinra Posted at: 2017-07-27T13:55:06.000Z Reads: 67

```
It depends on load, if you only push a little bit while you're on the board it will probably maintain a slow speed because the current supplied isn't enough to overcome load.

there are modes where throttle position determines speed (duty cycle/pod control), but it also means when you let go to neutral it will brake and slow down since you're technically moving the throttle back to resting position (complete stop)

Current control is the "better" mode, you just have to get used to it
```

---
## \#40 Posted by: Bloop Posted at: 2017-07-27T13:57:48.347Z Reads: 65

```
when i tested the current control i had trouble breaking .. but yeah i guess if i get used with it will be fine. i will do some more testings tonight and come back with updates. thank you .
```

---
## \#41 Posted by: Jinra Posted at: 2017-07-27T14:07:40.281Z Reads: 65

```
What trouble? While you were in the board?
```

---
## \#42 Posted by: Bloop Posted at: 2017-07-27T14:12:03.399Z Reads: 64

```
Yes while i was on the board. sometimes it was no breaking/moving backwards. i was accelerating and then break/throttle back and it would not respond ... then when i stop and do reverse it would go reverse with no problem .. i have no idea what happened then but after that i changed back to no reverse with break
```

---
## \#43 Posted by: Bloop Posted at: 2017-07-27T18:06:51.724Z Reads: 64

```
Ok new update once i tested again. 

Everything seems to work just fine with me on the board the break and the acceleration. Thank you @Jinra for all you help. 

I tested now with both no reverse with break and current mode and both are working good. Altho im a little scared to break when high speed. 

I think ill use it in current because the break is easier to control. 

Sadly the rain ended my happiness so i had to stop for today. If anything else comes up ill update.
```

---
## \#44 Posted by: rpn314 Posted at: 2017-07-27T20:40:49.682Z Reads: 56

```
I think someone mentioned it above, but give @Ackmaniac's firmware a go. I think you'll like the throttle curves
```

---
## \#45 Posted by: Bloop Posted at: 2017-07-27T20:54:09.669Z Reads: 57

```
i had no time to read about that and i dont understand if that is to be installed on the vesc or is just like bldc tool ... i will read about it and check that out :D tnx
```

---
## \#46 Posted by: rpn314 Posted at: 2017-07-27T20:56:58.147Z Reads: 58

```
Definitely read about it. It's basically a custom firmware to replace the firmware that's on the VESC and a modified BLDC-Tool to configure it. It's based on the originals, but @Ackmaniac has done an amazing job and added some very good control features (throttle curves for example) that make it much more intuitive and natural.

https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286?u=rpn314
```

---
## \#47 Posted by: Bloop Posted at: 2017-07-28T11:33:53.450Z Reads: 51

```
I tested the button that is supposed to change the mode beginner/advanced but i see no difference in speed or acceleration with button up or down ? 

Do i need to make anything else ? (i read something that is on reverse from the specs down is high speed and up is begginer) 

Thank you.
```

---
