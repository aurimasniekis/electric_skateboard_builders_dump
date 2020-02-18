# DD Mad Speed. Mad hubs DD conversion kit Build

### Replies: 98 Views: 716

## \#1 Posted by: Skyart15 Posted at: 2019-07-01T15:37:56.233Z Reads: 182

```
DD Mad Speed. 12s4p TB battery and enclosure | FSESC 6.6 dual | Mad Hubs DD conversion kit | TB 110 | TB 218mm trucks | sector 9 drop through deck, top mounted.
![20190701_081410|374x500](upload://jSIgMQoOjD1MhccSgFKW1Va7z9e.jpeg) 
![20190701_081426|374x500](upload://4YNU2DLyc9ikUPM9z3fuxRwl6Z0.jpeg) 
![20190701_081419|375x500](upload://1ybPBp7b5mKNnm8hTVqUhdDy9yv.jpeg) 

Simple recepie, lots of hard work, (courtesy of @pookybear) and some borrowed components also @pookybear The results are amazing! So far able to top out at 43MPH...the speed is insane this Direct Drive is nuts! 
Although the drives I received need a little attention, and I believe a loose magnet may have blown two of my vescs, This comunity is really coming through with the support! Thanks to @pookybear who let me borrow his DD kit and also his FSESC 6.6 Dual, I am not only up and boarding, but also boarding on what is a very sweet and smooth set up! I know the TB battery and enclosure is not ideal, due to its size and the discharge BMS, also my old sector 9 deck is not the best, but it works well, and handles beautifully! In the future I am hoping to migrate this build either to a HAYA or maybe a Hummie, but for now this will work. 

A little about the drives themselves. As with other DD set ups and Hub motor builds, breaking at low speeds is not very good, but I'm talking about under 5 Mph. Also hill climbing, still playing with settings but so far it's not as good as my previous belt drive set up...but I wasn't really expecting it to be. Currently my settings are:

Battery 30A
Motor 60A/-60A
Sensorless 

The torgue is great, and I have not tested the 60amp set up on a big hill yet, will test that later today and post my findings. Also I understand that with the gigantic TB wheels I am expecting to see less torgue.

This is all I got for you at the moment, feel free to ask question, this is my first build thread, also input is appreciated. Again big shout out to @pookybear for helping me make this happen! And of course @rey8801 for organizing the group buy!
```

---
## \#2 Posted by: rey8801 Posted at: 2019-07-01T15:45:19.133Z Reads: 148

```
The label on the hub give the final touch...love it :yum:

For the low speed braking that is common with hub motor due to the low rolling resistance. Since you use FESC you can set active braking at low speed.
```

---
## \#3 Posted by: pookybear Posted at: 2019-07-01T15:55:03.887Z Reads: 143

```
Yes, we're going to try that next. Active braking works for elofty drives. So I don't see any reason why it wouldn't work for this drive. :crossed_fingers:t4:
```

---
## \#4 Posted by: rey8801 Posted at: 2019-07-01T15:55:52.821Z Reads: 139

```
It will I think, I didn't try because I don't think you can set it with the Unity :unamused:
```

---
## \#5 Posted by: pookybear Posted at: 2019-07-01T15:56:58.793Z Reads: 134

```
You should be able to. @Winfly  gave me a little hint. I think it's called max reverse erpm.

Credit also goes to @mishrasubhransu for finding the fix!
```

---
## \#6 Posted by: rey8801 Posted at: 2019-07-01T15:57:28.785Z Reads: 123

```
Fxxk didn't know that...I will have a look.
```

---
## \#7 Posted by: pookybear Posted at: 2019-07-01T16:00:46.844Z Reads: 120

```
@Skyart15. You can peel that "pookybear" label off dude.

@rey8801
Just saw that. :rofl:
```

---
## \#8 Posted by: rey8801 Posted at: 2019-07-01T16:01:12.711Z Reads: 111

```
On the app I only see the possibility to select forward/reverse I guess I need to use the PC. DOes the unity now support TCP connection or I need to open the enclosure?
```

---
## \#9 Posted by: Skyart15 Posted at: 2019-07-01T16:02:09.653Z Reads: 113

```
Loooool! No that label is staying on! Mostly tho for testing to see him much heat it can handle loooool! I'm surprised it hasn't melted off or set on fire yet!
```

---
## \#10 Posted by: pookybear Posted at: 2019-07-01T16:03:42.211Z Reads: 110

```
BT connection on unity was sketchy when I had it. Not sure about now as well as if it supports TCP connection. I'd open the enclosure up. Post in unit support thread?
```

---
## \#11 Posted by: pookybear Posted at: 2019-07-01T16:04:19.809Z Reads: 104

```
Hahahahaha. Stickers add 5mph more yO.
```

---
## \#12 Posted by: rey8801 Posted at: 2019-07-01T16:11:42.618Z Reads: 100

```
of course...it's known. It goes with the countersunk washer that adds speed, toruqe or range based on the colour.
```

---
## \#13 Posted by: rey8801 Posted at: 2019-07-01T16:15:07.582Z Reads: 100

```
I ma trying with TCp thorugh Metr.pro.

So this the setting I guess:

@pookybear
28 magnets(Or 14 magnetic pole pairs) on the rotor…
24 stator poles. Stator poles don’t count in our analysis.

so this still holds.
7*14*1000000/(60*pi*110)=4726
```

---
## \#14 Posted by: pookybear Posted at: 2019-07-01T16:15:39.065Z Reads: 96

```
Yes, I'd try that.
```

---
## \#15 Posted by: pookybear Posted at: 2019-07-01T16:19:34.964Z Reads: 95

```
7kmh = 4.35mph 

So on flats, I assume it'll move you in reverse. Downhill, depending on steepness level, it "should" hold you. I have not tried this yet.
```

---
## \#16 Posted by: rey8801 Posted at: 2019-07-01T16:28:39.379Z Reads: 97

```
yeh the metr. TCP bridge works nad I set the PPm to Current, Then limited the reverse but if I try in the room it still goes really fast in reverse.

Ok now it works! I will try on street. You calculated 4726 fro the 110mm  wheels?
So for 97mm will be 4167 I guess.
```

---
## \#17 Posted by: Sender Posted at: 2019-07-01T16:54:47.869Z Reads: 101

```
I have a blank canvas Haya ready for customization if you are interested! V2

Also what KV are those 90?

Here is one I am almost finished up with

![20190630_155407|327x500](upload://pNrtBGhIO7HagSMuXVIF5Y4tYub.jpeg) ![20190630_155429|279x500](upload://97qCb8x38xZqsvYIUeCMXVdClF.jpeg) ![20190630_155501|666x500](upload://75chObwNtKX9imNLOBnktj6PNLK.jpeg) ![20190630_155228|281x500](upload://3AXMYxWVbzCDU0kHb9hxgpB1Sg9.jpeg)
```

---
## \#18 Posted by: rey8801 Posted at: 2019-07-01T16:56:19.026Z Reads: 95

```
Amazing deck.
No they are 75Kv 😁
```

---
## \#19 Posted by: rey8801 Posted at: 2019-07-01T16:58:52.886Z Reads: 96

```
Ok rode home with this setting. It works 200%. Even too much. I would say half of the value you calculated are already good. I could fully brake because the first time I did I approced the cross by sliding the last meter 😁. It also held me on slope. But you have to be more conscious about brakong because otherwise they try to go reverse that's why better to lower it I think. I will try around 2000 next time.
I aspected as I'm the Ackmaniac firmare thst reverse is only engaged from fully stop wheels but actually no if you go full reverse or even close to that it will start trying to go reverse and lock your wheels.
```

---
## \#20 Posted by: pookybear Posted at: 2019-07-01T17:00:13.425Z Reads: 91

```
Good to know! Thanks for trying this. It's the max reverse erpm, correct?
```

---
## \#21 Posted by: rey8801 Posted at: 2019-07-01T17:01:21.774Z Reads: 79

```
I set it to 4167. I made a quick proportion from your value. But I think half is fine
Since you don't want to go reverse lower should prevent thst a bit, stil not final solution for me. Should make an active braking mode that stops as soon you actually go reverse. Maybe I will try a - 500/1000. Just for science. It really brakes hard. Now slide is so easy 😂
```

---
## \#22 Posted by: pookybear Posted at: 2019-07-01T17:04:54.116Z Reads: 79

```
Maybe -1000erpm.
```

---
## \#23 Posted by: rey8801 Posted at: 2019-07-01T17:07:18.357Z Reads: 84

```
Yes that what I am gonna try next. Plus the nano X has short throw. I am waiting the Flipsky for a while now. I will play with the curve to make it less invasive during braking so to engage the 100% really at the end.
```

---
## \#24 Posted by: mishrasubhransu Posted at: 2019-07-01T17:08:23.284Z Reads: 79

```
The value doesn't matter. The less the better because you are not thrown off the board if you accidentally forget to let go of the brake as the board will start moving back.. However motor cogging happens if it's too low. You can set it to 1000, 500 etc and see the effect.

It doesn't affect the braking strength, only the reverse speed...what affects the braking strength is the -motor current.
```

---
## \#25 Posted by: rey8801 Posted at: 2019-07-01T17:09:23.490Z Reads: 74

```
That's true. Maybe my - 70A is too much! 😁I will lower it. Although sliding is pretty cool I left nice C sign at the turns.
```

---
## \#26 Posted by: pookybear Posted at: 2019-07-01T17:10:47.120Z Reads: 76

```
Yea, we have set -55 on @Skyart15 s units. Board was literally rolling downhill while he was on full brakes with no load. So I figured the only way to have better downhill brakes is your active braking method.

* 60
* -55
* 30
* -14
```

---
## \#27 Posted by: rey8801 Posted at: 2019-07-01T17:11:49.662Z Reads: 70

```
Yeh if you brake at lower than 5 kmh they just sill. I am use to step off or foot stop the last 3km but better like that.
```

---
## \#28 Posted by: rey8801 Posted at: 2019-07-01T17:12:27.017Z Reads: 69

```
I have reached - 20A battery min but Yeh same thing.

Anyhow you don't have to open the enclosure. If you have metr for unity or a hm10 bluetooth too for the other vescs in TCP works great
```

---
## \#29 Posted by: mishrasubhransu Posted at: 2019-07-01T17:15:07.704Z Reads: 63

```
Yeah yeah, I understand that and know that would happen with direct drives. All I am saying is that is with the "current" mode, the value of reverse erpm doesn't affect the braking strength, only the reverse speed of the board. 

Your -55 motor current will work a lot better with "current" mode, because before when the ESC would effectively short the three phases, not even close to -55 would be passing.
```

---
## \#30 Posted by: pookybear Posted at: 2019-07-01T17:15:12.210Z Reads: 62

```
There was a post by longhairedboy in esk8 news forum that you don't really need anything beyond -7 or -14. You only hurt your battery cells if you go beyond that.
```

---
## \#31 Posted by: rey8801 Posted at: 2019-07-01T17:16:28.775Z Reads: 64

```
I know but then I read what Temapa explained and indeed I never see that value anyway in my riding logs. Anyway now with active braking doesn't need to be high anymore.
```

---
## \#32 Posted by: pookybear Posted at: 2019-07-01T17:19:07.269Z Reads: 66

```
We have been figuring out his BT module he got from flipsky. It's not connecting for some reason. I suspect it doesn't support Android OS 9.
```

---
## \#33 Posted by: rey8801 Posted at: 2019-07-01T17:20:30.971Z Reads: 63

```
Is he using Fesc or what? It's a possiblity. I have modules that works on all the Android version or you can flash them. In the past I was doing that for people. I flashed so many 😅
```

---
## \#34 Posted by: mishrasubhransu Posted at: 2019-07-01T17:20:47.822Z Reads: 62

```
The Bluetooth will directly connect from the app. It's not a regular Bluetooth that you need to pair. Try the vesc-tool app
```

---
## \#35 Posted by: Skyart15 Posted at: 2019-07-01T17:20:57.925Z Reads: 60

```
Yeah fsesc
```

---
## \#36 Posted by: pookybear Posted at: 2019-07-01T17:21:00.646Z Reads: 64

```
Yes. Fsesc6.
```

---
## \#37 Posted by: Skyart15 Posted at: 2019-07-01T17:21:39.633Z Reads: 62

```
The vesc tool android app?
```

---
## \#38 Posted by: mishrasubhransu Posted at: 2019-07-01T17:22:05.768Z Reads: 60

```
That's what I use with my fs 6.6
```

---
## \#39 Posted by: pookybear Posted at: 2019-07-01T17:22:22.084Z Reads: 63

```
He is on ackmaniac fw. Not sure if Vesc tool app supports it.

We have been trying it on ackmaniac app.
```

---
## \#40 Posted by: rey8801 Posted at: 2019-07-01T17:22:29.655Z Reads: 63

```
Of course @mishrasubhransu you are talking about the vesc app that require metr or tranpa module is more advance. Hm10 is a simple BLE that will work with the vesc tool on PC in TCP bridge. It's slow but works
```

---
## \#41 Posted by: rey8801 Posted at: 2019-07-01T17:24:02.335Z Reads: 51

```
How the bluettoh module shows up on the app? Like it usually has a code. If you tell me I know which ones are compatible or flashable
```

---
## \#42 Posted by: pookybear Posted at: 2019-07-01T17:25:07.456Z Reads: 54

```
I personally have 2 metro pro and my buddies boards I built has bkb BT modules. They all work great.

I'm helping @Skyart15 out. He has the flipsky one.
```

---
## \#43 Posted by: mishrasubhransu Posted at: 2019-07-01T17:26:08.750Z Reads: 61

```
Ah okay. Well the nrf51-vesc is also available from flipsky to but for $9, not not at all expensive.

Some people don't want to support trampa and hence don't want to use vesc_tool, but otherwise there is no reason not to use the latest developments with vesc-tool. It's really nice. 

I put up an instruction how to use the app. It's easy peasy. 

https://forum./t/all-new-2019-vesc-tool/3244/18?u=mishrasubhransu
```

---
## \#44 Posted by: rey8801 Posted at: 2019-07-01T17:26:24.313Z Reads: 58

```
Anyhow you can try with older phone or iPhone if there is a app for IOS. Since the version compatibility problem is only with Android.
```

---
## \#45 Posted by: pookybear Posted at: 2019-07-01T17:26:29.608Z Reads: 59

```
I also learned a while back that w these BT modules, you dont pair them using your phones' BT settings. You always use the app to do it.
```

---
## \#46 Posted by: Skyart15 Posted at: 2019-07-01T17:27:07.110Z Reads: 63

```
Unfortunately I did not leave it plugged in the board but this is i believe how it shows up ![Screenshot_20190701-102617_ESC%20Monitor|243x500](upload://8sEOOzttD2vatCzLSRUiZbPOdJ3.jpeg) 
Titled superman
```

---
## \#47 Posted by: rey8801 Posted at: 2019-07-01T17:27:18.550Z Reads: 59

```
Yes they are BLE modules so low energy one. You can dowload BLE terminal app that it's made to check them out and work with Arduino. It tells you more about the module.
```

---
## \#48 Posted by: mishrasubhransu Posted at: 2019-07-01T17:27:20.262Z Reads: 60

```
If @Skyart15 has flipsky Bluetooth modules then he can use the vesc-tool mobile app. 100% 

It's pretty intuitive by itself, but otherwise I have a small guide in the link posted above..
```

---
## \#49 Posted by: pookybear Posted at: 2019-07-01T17:28:15.188Z Reads: 63

```
I wonder if the Vesc tool app supports the ackmaniac fw.
```

---
## \#50 Posted by: rey8801 Posted at: 2019-07-01T17:28:39.033Z Reads: 57

```
No it doesn't. Trampa mentioned in some discussion. I wouldn't dare. Ackmaniac is based on watt mode. @Skyart15 you can flash the latest  original vesc tool and try. Although if the module doesn't connect to the phone then that shouldn't be related with the vesc but only incompatibility between phone and module
```

---
## \#51 Posted by: mishrasubhransu Posted at: 2019-07-01T17:28:51.752Z Reads: 62

```
Why do you need ack firmware? Before ack had some advantages but now it has all those features like watts control and a lot more. Also Ben, is spending a. Lot more time on it. You can see it on the GitHub commmits.

@rey8801, regular firmware has watt control now.
```

---
## \#52 Posted by: pookybear Posted at: 2019-07-01T17:30:58.296Z Reads: 56

```
Better throttle feel for me personally. And the new Vesc tool GUI is too "automated". I'm just so old school and used to the old interface. 

It is mostly the throttle feel. Yes, I have tried the new FW. I didn't like it so I went back.

I tried it on Vesc tool 1.08
```

---
## \#53 Posted by: rey8801 Posted at: 2019-07-01T17:31:51.812Z Reads: 54

```
I know. I am saying that original won't be 100% compatible with Ackmaniac's one. Better to switch it original if you want to use the app.
@Skyart15 do a quick test with an iPhone phone or older Android phone. If they see the module then it's done.
```

---
## \#54 Posted by: mishrasubhransu Posted at: 2019-07-01T17:33:00.409Z Reads: 53

```
Okay, after those automated steps are done, you still have all the same settings and all the same parameters to manually change like before.
```

---
## \#55 Posted by: pookybear Posted at: 2019-07-01T17:33:06.538Z Reads: 51

```
He has a work iPhone but xymatic app is $6 lol
```

---
## \#56 Posted by: pookybear Posted at: 2019-07-01T17:35:00.431Z Reads: 54

```
@Skyart15

Wanna give the new FW a shot? All for science. Lotta work just to get BT module up and running. :joy:
```

---
## \#57 Posted by: rey8801 Posted at: 2019-07-01T17:35:08.865Z Reads: 56

```
Too much for a try. 😥
```

---
## \#58 Posted by: pookybear Posted at: 2019-07-01T17:35:25.463Z Reads: 60

```
Exactly.
10missingjasons
```

---
## \#59 Posted by: rey8801 Posted at: 2019-07-01T17:36:23.444Z Reads: 57

```
What I am saying is that the firmware won't change the BLE compatibility. Better to try it out with old Android then. Or flash the Flipsky module if it is possible. I think they use a variation of the classical HM10
```

---
## \#60 Posted by: Skyart15 Posted at: 2019-07-01T17:36:50.219Z Reads: 53

```
I'm down, maybe sometime this coming weekend? You talking about flashing vesc tool firmware to the fesc?
```

---
## \#61 Posted by: Skyart15 Posted at: 2019-07-01T17:38:13.025Z Reads: 48

```
I see, il download the iphone version of ack on my wife's phone and maybe we can try that @pookybear
```

---
## \#62 Posted by: rey8801 Posted at: 2019-07-01T17:39:35.173Z Reads: 59

```
You don't need to pay for the app just for testing. Search for a BLE terminal app or similar for IOS on the market. They are able to detect the BLE module. If you see it and can connect then you know the module will work

BLE scanner is easy to use and works great. Check if an IOS version exists. 

![blescanner|281x500](upload://rX47UU7PpFxbxSYfhDv7cVZasEW.png)
```

---
## \#63 Posted by: pookybear Posted at: 2019-07-01T17:42:44.633Z Reads: 54

```
Ack app sees it but it won't connect to it.
```

---
## \#64 Posted by: pookybear Posted at: 2019-07-01T17:44:29.715Z Reads: 53

```
Yes, if you are up to it. I can remote in again. The whole idea of you getting up and running is to ride. So you can enjoy it while you work on your DDs magnets. But if you are down to do it, I do not mind at all.
```

---
## \#65 Posted by: pookybear Posted at: 2019-07-01T17:45:55.267Z Reads: 51

```
[quote="rey8801, post:59, topic:97640, full:true"]
What I am saying is that the firmware won’t change the BLE compatibility. Better to try it out with old Android then. Or flash the Flipsky module if it is possible. I think they use a variation of the classical HM10
[/quote]



Yup. That is what I'm getting at.
```

---
## \#66 Posted by: rey8801 Posted at: 2019-07-01T18:05:46.743Z Reads: 50

```
Ah ok then I think the original vesc app will work after have flashed the original vesc firmware
```

---
## \#67 Posted by: DJase Posted at: 2019-07-01T18:13:06.963Z Reads: 48

```
This shit is mad yo 😏
```

---
## \#68 Posted by: pookybear Posted at: 2019-07-01T18:18:10.069Z Reads: 52

```
[quote="rey8801, post:66, topic:97640, full:true"]
Ah ok then I think the original vesc app will work after have flashed the original vesc firmware
[/quote]

We're gonna try it and post back w the results.
```

---
## \#69 Posted by: deucesdown Posted at: 2019-07-01T19:33:42.683Z Reads: 53

```
[quote="mishrasubhransu, post:51, topic:97640"]
Why do you need ack firmware?
[/quote]

There are a bunch of reasons, with pros and cons of course.

- ackmaniac app compatibility for modes (ackmaniac app has nice csv log files, and starts logging immediately on connect, nice if you try to log every ride)

- better failsafe behavior

- cruise control using second ppm channel

- works with hm-10 modules which helps if you've been building for a while or have many boards

- I remember reading a post from ack saying most of the code changes are for UI, and that nothing significant changed in the motor control loop, which I agree is the important part

BTW @Skyart15 @pookybear nice build, thanks for posting! Love the tape!
```

---
## \#70 Posted by: pookybear Posted at: 2019-07-01T19:52:55.011Z Reads: 48

```
Also, for the record:

I'm not anti trampa. I own 2 trampa vesc6. My friends and I pre-ordered 3 trampa wand remote. I chose ackmaniac due to personal preference and it works for me. Just that. In fact, I recommended it to @Skyart15 when 2 of his fsesc6  broke.
```

---
## \#71 Posted by: Skyart15 Posted at: 2019-07-01T20:16:31.336Z Reads: 55

```
So I just got back from a ride, and it was a spirited ride for sure ![Screenshot_20190701-130343_Speedbot|690x335](upload://u7fAodV5niTxahfDXHCloXz4k6R.jpeg) 
The question I have is, i can barely touch the motor casings lol they are pretty hot I'm guessing in the 160-170f range how does that kind if tempraturw not melt the insulation on the motor leads? ![20190701_131301|375x500](upload://8vR889tnn4qz1P1sNBoXcpK6IFh.jpeg)
```

---
## \#72 Posted by: pookybear Posted at: 2019-07-01T20:17:39.269Z Reads: 52

```
Well. You should rephrase that to, "how is the sticker/tape still there and not melted?" :rofl:
```

---
## \#73 Posted by: Skyart15 Posted at: 2019-07-01T20:18:52.382Z Reads: 50

```
RoFL!! Maybe next time @rey8801 can use blue painter's tape instead steel casing for the dd conversion kit 😆 seemed to be indistructable!
```

---
## \#74 Posted by: rey8801 Posted at: 2019-07-01T20:21:21.734Z Reads: 52

```
On my prototype I am still using 3d printer case. Then you can choose the colour you want!
```

---
## \#75 Posted by: rey8801 Posted at: 2019-07-01T20:23:43.293Z Reads: 51

```
well insulation should be good up to 220C. Anyhow you really got them hot. Even if I push them a lot they are hot but never got so high. I guess I leave them the time to cool down a bit while riding.
```

---
## \#76 Posted by: pookybear Posted at: 2019-07-01T20:44:56.642Z Reads: 52

```
Not sure if this applies to esk8 motors. In the RC world and in most situations, we gear it based on temps and laptimes. Stock racing. Optimal temp for RC motors is ~160. Anything over ~170ish is just wasted heat because they don't get any faster despite gearing it heavier. 

I don't know anything about these Mad DD motors. IMO, 160F at the end of a ride is still acceptable. Of course I have no data to back this up. This is solely based my experience w RC 10th scale motors since '06. RC brushless didn't start until maybe a few years later after that.
```

---
## \#77 Posted by: Skyart15 Posted at: 2019-07-01T22:53:25.828Z Reads: 53

```
Ok so this set up is working for climbing this particular hill ![Screenshot_20190701-155020_Speedbot|690x335](upload://5CR7D9mFUOgagWGQpFrpomXfAfS.jpeg) 
As you can see at the top of the hill I was doing around 14mph, this is with me entering the hill at the bottom at about 21mph. Ideally I would like more torgue, what do you think @pookybear shall we try 80 motor amps? 😆 is my only saving grace at this point...smaller wheels?
```

---
## \#78 Posted by: pookybear Posted at: 2019-07-01T22:56:52.132Z Reads: 49

```
Hahaha. You need a temp gun w you when you ride so we can watch the motors temp.
```

---
## \#79 Posted by: rey8801 Posted at: 2019-07-02T07:10:03.358Z Reads: 49

```
I tried up to 70A and didn't feel to much difference. To me 60A is the max current for this motor. I use 70A but do;t feel to much difference and you already get them really hot. For more torque you need smaller wheels.
I really don't feel the need of more torque with my wheels. It's constantly accelerating.
Also depends on the rider weight of course. I am 83-85kg now while riding.

Btw: factory rates them at 50A. So we are already over the limit. Also a belt drive will need new gear  ratio going from 90mm wheels to 110mm. This hubs where designed for 90mm.
```

---
## \#80 Posted by: rey8801 Posted at: 2019-07-02T07:13:50.052Z Reads: 51

```
So tried these new setting max reverse - 2000 and motor min - 60A. Now the active braking is smoother and predictable. I like it. It really stops you no problem
```

---
## \#81 Posted by: mishrasubhransu Posted at: 2019-07-02T07:19:22.641Z Reads: 47

```
Too much current and you can demagnetize the permanent magnets or weaken them. These are low kv so for the same current they produce a lot stronger magnetic field than for the same current on a high KV motor.
```

---
## \#82 Posted by: rey8801 Posted at: 2019-07-02T07:24:42.224Z Reads: 47

```
True. They need less current to output same torque. They use magnets rated up to 150C. I won't risk to go close to that. With the wheels you are using it's clearly speed oriented as you could see so torque has to go down a bit. Probably still fine but if you search only hills climbing then better gear or belt drive to me. If it's a mix for riding around and have fun then it's fine. If you want more torque go down with the wheels size. Already 100mm should give you more.
```

---
## \#83 Posted by: Skyart15 Posted at: 2019-07-02T12:35:27.644Z Reads: 44

```
This all makes sense. Going to try 100mm this week!
```

---
## \#84 Posted by: rey8801 Posted at: 2019-07-02T14:21:02.611Z Reads: 49

```
Which one do you have? Just out of curiosity sic e I can not find any 😁
```

---
## \#85 Posted by: pookybear Posted at: 2019-07-02T16:04:44.118Z Reads: 51

```
MBS 13401 - Black All-Terrain Longboard Wheels - 100mm X 65mm - Black https://www.amazon.com/dp/B015GJN0BA/ref=cm_sw_r_other_apa_i_2b4gDbRAHYTF3
```

---
## \#86 Posted by: rey8801 Posted at: 2019-07-02T16:09:08.921Z Reads: 51

```
Ok thanks. I thought some cool urathene one to replace BOA. I like wider contact patch.
```

---
## \#87 Posted by: Skyart15 Posted at: 2019-07-10T04:45:37.927Z Reads: 44

```
Ok here is what I found
![20190709_214211|375x500](upload://1YLwjv5UTjcJZfDOxBxmh0J1iEr.jpeg) ![15627338286033597427967937172779|375x500](upload://vd8jeSIg3BwvM3tpEspUpFNlt7W.jpeg) 
Magnets seem to be in place, but there are quite a few what look like shavings of some sort in the bottom of the black can cover.
```

---
## \#88 Posted by: Skyart15 Posted at: 2019-07-10T04:46:54.019Z Reads: 43

```
![15627339475796106422355013740812|375x500](upload://9UFSTsqad1Cxm03QQZDiJOaEF46.jpeg)
```

---
## \#89 Posted by: Skyart15 Posted at: 2019-07-10T04:50:49.659Z Reads: 43

```
https://youtu.be/J9RMj7Wvf-o
```

---
## \#90 Posted by: rey8801 Posted at: 2019-07-10T05:56:25.138Z Reads: 39

```
Ok. Well the CAN with magnets is glued to th front so you should have remove the front panel and then remove the CAN with magnets thst comes off with the front bearing ecc...
Anyhow the can looks ok. I think the problem is probably in the stator then but then it's difficult to say it. When you hand spin the motor try to short 2 of the phase wires at the time and feel if becomes harder to turn.
```

---
## \#91 Posted by: Skyart15 Posted at: 2019-07-10T20:14:04.005Z Reads: 30

```
So when i go to reassemble it do i have to glue the rotor back down to the can before i reassemble?
```

---
## \#92 Posted by: rey8801 Posted at: 2019-07-10T20:49:08.539Z Reads: 26

```
yes I would remove the front screws and take the front panel and glue it with the motor can. Check my tutorial video and you will see that the motor is assemble together since the beginning. The parts slide on top of it.

I was checking the video. The first wire you are pointing seems the junction of the 3 motor phase wires in the wye configuration. the second thing attached to the sensor is like a heat shrink or what?
```

---
## \#93 Posted by: Skyart15 Posted at: 2019-07-10T20:50:45.059Z Reads: 25

```
what kind of glue should i use?
```

---
## \#94 Posted by: rey8801 Posted at: 2019-07-10T20:52:08.636Z Reads: 23

```
loctite 380 is good. Also for magnets in case.
```

---
## \#95 Posted by: Skyart15 Posted at: 2019-07-10T21:03:36.921Z Reads: 24

```
cant seem to find that video, could you link it here? and Thank you!!!
```

---
## \#96 Posted by: rey8801 Posted at: 2019-07-10T21:14:17.603Z Reads: 25

```
Anyhow if this one shorts on the metal can you need to heat shrink it back. Otherwise the motor won't work. You can test it with a meter.

![58|690x330](upload://tOGTKJDk9NUihNXm5jdjlgO9w68.png)
```

---
## \#97 Posted by: Skyart15 Posted at: 2019-07-10T21:26:04.863Z Reads: 23

```
It shorts to that piece that backing piece that you see on there, can I trim it a little and then heat shrink it? I think part of the problem is that, that tail is to long
```

---
## \#98 Posted by: rey8801 Posted at: 2019-07-10T21:46:44.325Z Reads: 23

```
It should be after the not of the 3 phase wires so it doesn't have any role. Maybe remove the old heat shrink to be sure. A short in that spot is definitely a problem.
```

---
