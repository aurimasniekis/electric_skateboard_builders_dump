# New Builder Parts Check and LCD question

### Replies: 38 Views: 3371

## \#1 Posted by: dstnceswmer Posted at: 2016-06-02T17:20:55.444Z Reads: 190

```
Hi, I'm looking to start my first build in the next couple weeks I have been doing some research and have compiled, at least so far, an electronics parts list. I was wondering if someone with more knowledge could spot check me on these, and is this all I will need electronics wise?

- Turnigy Aerodrive SK3 - 6374-192kv Brushless Outrunner http://www.hobbyking.com/hobbyking/store/__18129__Turnigy_Aerodrive_SK3_6374_192kv_Brushless_Outrunner_Motor.html

- RotorStar 120A LV (2~6S) Brushless Speed Controller with Selectable SBEC http://www.hobbyking.com/hobbyking/store/__55425__RotorStar_120A_LV_2_6S_Brushless_Speed_Controller_with_Selectable_SBEC.html

- (2x) ZIPPY Flightmax 5000mAh 6S1P 20C http://www.hobbyking.com/hobbyking/store/__8582__ZIPPY_Flightmax_5000mAh_6S1P_20C.html

- IMAX B6AC V2 Professional Balance Charger/Discharger http://www.hobbyking.com/hobbyking/store/__58285__IMAX_B6AC_V2_Professional_Balance_Charger_Discharger.html

- Quanum 2.4Ghz 3ch Pistol Grip Tx & Rx System http://www.hobbyking.com/hobbyking/store/__44693__Quanum_2_4Ghz_3ch_Pistol_Grip_Tx_Rx_System.html

Also I've noticed some builds with an LCD/LED screen mounted in the electronics casing. I've been wondering what that is? Battery Monitor? and how to incorporate it into my build. 
Thanks in advance for any help :)
- Justin
```

---
## \#2 Posted by: longhairedboy Posted at: 2016-06-02T17:31:13.042Z Reads: 178

```
[quote="dstnceswmer, post:1, topic:4152"]
Also I've noticed some builds with an LCD/LED screen mounted in the electronics casing.
[/quote]

http://www.ebay.com/itm/172143986261?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

that's exactly what it is. They're great! you can program them to work with packs up to 14S and all you need to get them into a box is a dremel and some hot glue. You can connect the wires either to the ESC side of the switch you're using or even to the motor controller power leads, so long as its not directly to the battery because then it will be always on even if your board is turned off. I wouldn't connect it to your charge port though, i tried that temporarily to test something and the meter got pretty warm while charging.

Also i think you'll be just fine with most of those parts but i'm not sure about the ESC you picked. I have no experience with them so i'm not sure if they're really suitable. Most people use Car ESCs if they' aren't using a VESC or a Torqueboards.
```

---
## \#3 Posted by: Blacksheep Posted at: 2016-06-02T18:14:04.651Z Reads: 164

```
Does that work with li-ion?
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-06-02T18:31:57.445Z Reads: 152

```
Totally. That's what i'm using it with now.
```

---
## \#5 Posted by: Blacksheep Posted at: 2016-06-02T18:35:08.712Z Reads: 149

```
Thank you what kind of bms do you use? And does it matter what kind of bms for a sk3 6374?
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-06-02T18:54:49.622Z Reads: 143

```
i don't think it matters what kind of BMS you use as long as it csan handle the amps you intend to draw. I usually just aim for complete overkill instead of trying to calculate exactly the most i'll need and risk bumping up to the margin.
```

---
## \#7 Posted by: Blacksheep Posted at: 2016-06-02T18:58:02.924Z Reads: 138

```
Ok thank you this will be my first buil
```

---
## \#8 Posted by: Blacksheep Posted at: 2016-06-02T19:37:11.210Z Reads: 134

```
Do you have a bms, battery pack and switch wiring diagram?
```

---
## \#9 Posted by: Jinra Posted at: 2016-06-02T19:46:45.647Z Reads: 132

```
Here's a 10s diagram

http://www.batterysupports.com/36v-37v-42v-10s-80a-10x-36v-lithium-ion-lipolymer-battery-bms-p-389.html
```

---
## \#10 Posted by: Blacksheep Posted at: 2016-06-02T19:53:54.017Z Reads: 135

```
It doesn't show
<img src="/uploads/db1493/original/2X/8/890eda489dd2fc71ce382e8d2f1f1cae39453fb3.png" width="281" height="499">
```

---
## \#11 Posted by: dstnceswmer Posted at: 2016-06-02T19:56:14.963Z Reads: 128

```
Curious, what is a BMS? Also thanks @longhairedboy for the Batt monitor info!
```

---
## \#12 Posted by: Jinra Posted at: 2016-06-02T19:56:30.538Z Reads: 135

```
Link fixed

@dstnceswmer They do a bunch of different things such as overcurrent, overdischarge, etc protection. Main purpose is to balance charge the batteries though.
```

---
## \#13 Posted by: Ulfberht Posted at: 2016-06-02T19:58:31.173Z Reads: 132

```
@dstnceswmer
Looks like you have a couple of issues with this line up. 
Your battery looks like it could be a 6s2p or a 12s1p, Both choices would be out of optimal efficiency when used with that sweet 192kv motor. You would be much better off with a 10s battery. If you are going with Lipos, then two 5s packs would be perfect. Your esc is top end rated@6s, so you might want to consider the choices available.  Best to give yourself some wiggle room. 
Check out this thread about the matter:
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
Also check out Ollinboardco!! Simply the best parts...
http://www.ollinboardcompany.com/product/om5065-200kv

Hope that is helpful! :grin:
```

---
## \#14 Posted by: dstnceswmer Posted at: 2016-06-02T19:59:03.012Z Reads: 118

```
So is that not something that is necessary if you are using a balance charger such as the one I listed at the beginning of this thread?
```

---
## \#15 Posted by: Jinra Posted at: 2016-06-02T19:59:55.352Z Reads: 116

```
It's not necessary, just make sure you use a fuse and monitor your voltages carefully.
```

---
## \#16 Posted by: dstnceswmer Posted at: 2016-06-02T20:04:10.698Z Reads: 115

```
@Ulfberht Thanks for the info! I was planning on a 6s2p setup. I figured that would give a max current of (20C*5000mAh/1000)=100A with 22.2V well within the max tolerances of the ESC and motor. Are you saying it is out optimal efficiency since my voltage is lower? would it still be as strong as if I just had a motor rated closer to 6s? I was under the impression that as long as the motor rating was greater than the battery that you were good to go.
```

---
## \#17 Posted by: Ulfberht Posted at: 2016-06-02T20:14:15.685Z Reads: 115

```
I'm not saying that it won't "work", but it will work much more optimally with a higher voltage. Also the higher the voltage, the less juice the motors will need to pull to do the same work. Also less heat will be produced. @22.2-24v that motor will get pretty hungry for juice and heat up pretty good. Unless you are a very lightweight person, I would suggest rethinking 6s, IMO. Check out that thread link, Chaka explains it all really well.
```

---
## \#18 Posted by: dstnceswmer Posted at: 2016-06-02T20:16:42.066Z Reads: 110

```
Ok thanks! I'l take a look into it, just was trying to hopefully keep costs down with a lower voltage ESC, but I'll keep looking I guess.
```

---
## \#19 Posted by: dstnceswmer Posted at: 2016-06-02T20:46:05.799Z Reads: 113

```
@Ulfberht
 So Would this be closer to Ideal then With either a 10s battery or two 5s's in series?
http://www.hobbyking.com/hobbyking/store/__38787__Turnigy_Sentilon_V4_100A_5_12s_HV_Bulletproof_Speed_Controller_w_RPM_Sensor.html

@Jinra
What exactly are you referring to about monitoring the voltages and using fuses? Is this in regards to charging the batteries? Should this info be displayed on the charger or do I need to break out the DMM? Sorry for all the questions, I'm new to LIPO's
```

---
## \#20 Posted by: Jinra Posted at: 2016-06-02T21:05:59.805Z Reads: 102

```
Fuse for overcurrent protection. Monitoring voltage meaning not letting it completely die and damage the lipo.
```

---
## \#21 Posted by: Ulfberht Posted at: 2016-06-02T22:03:22.462Z Reads: 101

```
@dstnceswmer That one looks pretty good. I like how it has spark suppressor connections on the positive power lead. One less thing to worry about wiring up. If you need to power anything else, you will need to add a BEC. Cheap and easy. If you do go with this one, I'd suggest getting a programming card with it(around $10). Makes is a lot easier to get everything tuned up. You can also program using the controller on this model, but I don't know if that would be easier or harder to deal with.
```

---
## \#22 Posted by: dstnceswmer Posted at: 2016-06-03T00:02:25.058Z Reads: 95

```
Awesome! As far as batteries go then am i correct in thinking it's better to go with 2x 5s in series vs 1 10s. In terms of  chargers it looks more affordable to find a 4/6s charger then a 10s one. Im assuming they would need to be disconnected and charged separately though?
```

---
## \#23 Posted by: Jinra Posted at: 2016-06-03T00:06:10.373Z Reads: 93

```
It's essentially the same. The main difference being how you're going to balance charge. The Imax b6 doesn't support 10s charging so you'll have to charge each 5s pack individually. You can go with a single 10s pack but you'll have to find a charger that supports it.

I would wire 2x 5s packs using a series adapter (xt60 or other head) and charge the 2 packs individually.
```

---
## \#24 Posted by: Ulfberht Posted at: 2016-06-03T01:46:15.135Z Reads: 97

```
[quote="dstnceswmer, post:22, topic:4152"]
As far as batteries go then am i correct in thinking it's better to go with 2x 5s in series vs 1 10s
[/quote]

Yes sir! Much more affordable to charge 2x5s packs in parallel! Plus you have to consider space. 2 smaller packs will give you a lot more flexibility for fitting everything on your build! 
There are tons of videos on Youtube about it, but here's a link to Dexter@ discussing it. 
https://www.youtube.com/watch?v=ydhyWHsc9rg https://www.youtube.com/watch?v=ydhyWHsc9rg
```

---
## \#25 Posted by: Blacksheep Posted at: 2016-06-03T03:10:42.795Z Reads: 92

```
Thank you I can see it
```

---
## \#26 Posted by: dstnceswmer Posted at: 2016-06-04T01:08:54.921Z Reads: 89

```
@longhairedboy 
@Ulfberht 

Ok so here's my new electronics parts list, Look ok? 

- http://www.hobbyking.com/hobbyking/store/__36657__Turnigy_Aerodrive_SK3_6374_149kv_Brushless_Outrunner_Motor_US_Warehouse_.html

- http://www.hobbyking.com/hobbyking/store/__8582__ZIPPY_Flightmax_5000mAh_6S1P_20C.html

- http://www.hobbyking.com/hobbyking/store/__58285__IMAX_B6AC_V2_Professional_Balance_Charger_Discharger.html

- http://www.hobbyking.com/hobbyking/store/__38787__Turnigy_Sentilon_V4_100A_5_12s_HV_Bulletproof_Speed_Controller_w_RPM_Sensor.html

- http://www.hobbyking.com/hobbyking/store/__40274__Hobbyking_YEP_20A_HV_2_12S_SBEC_w_Selectable_Voltage_Output.html

- http://www.hobbyking.com/hobbyking/store/__43272__XT60_Panel_Mounting_Kit.html

- http://www.hobbyking.com/hobbyking/store/__2169__TURNIGY_BESC_Programming_Card.html

Also I am around 175lbs, wondering what kind of top speed I could expect with this setup? And how it would do on average hills?

-Thanks in advance :)
```

---
## \#27 Posted by: torqueboards Posted at: 2016-06-04T17:03:49.321Z Reads: 85

```
Looks ok but not too sure if that ESC will work. That ESC might have a firmware for an airplane/heli. With 6S, you should be able to get about 18-22mph. That 149kv though is pretty low KV so you might even be way less then that as far as mph goes.
```

---
## \#28 Posted by: dstnceswmer Posted at: 2016-06-04T17:09:51.183Z Reads: 82

```
actually I was going to have the batteries in series for 12S

How would you know if the esc is compatible or not? Is there a reason airplane/heli esc's dont work?
```

---
## \#29 Posted by: zool774 Posted at: 2016-06-04T18:03:53.657Z Reads: 81

```
Would a bms necessary for balancing  the 
discharge process is a vesc is used?
```

---
## \#30 Posted by: Ulfberht Posted at: 2016-06-04T18:29:15.266Z Reads: 78

```
@dstnceswmer IF it is a heli/plane esc you might not have the best brakes for an ESK8. Ideally you want a car esc.  
This thread may interest you. 
http://www.electric-skateboard.builders/t/best-esc-for-a-new-build/563/2
```

---
## \#31 Posted by: Jinra Posted at: 2016-06-04T20:39:14.026Z Reads: 76

```
no bms is not necessary for operation
```

---
## \#32 Posted by: zool774 Posted at: 2016-06-04T21:51:31.092Z Reads: 75

```
Thanks for clarifying that
```

---
## \#33 Posted by: dstnceswmer Posted at: 2016-06-05T18:32:00.766Z Reads: 71

```
so sounds like VESC is the best option for my 1 motor 12s setup?

Also curious, if I were to add another motor down the road would that require a second ESC? or can one ESC drive 2 motors?
```

---
## \#34 Posted by: flatsp0t Posted at: 2016-06-05T19:19:48.525Z Reads: 68

```
Shot answer:
In our sport it is not possible.
you will need a second esc.
```

---
## \#35 Posted by: dstnceswmer Posted at: 2016-06-06T01:44:36.771Z Reads: 68

```
ok good to know, thanks for the info :slight_smile:
```

---
## \#36 Posted by: dstnceswmer Posted at: 2016-06-06T22:21:24.461Z Reads: 60

```
Is enertion boards the best place to order a VESC from?
```

---
## \#37 Posted by: treenutter Posted at: 2016-06-20T16:30:14.456Z Reads: 33

```
6 posts were split to a new topic: [Genex's Build Thread](/t/genexs-build-thread/4912)
```

---
## \#38 Posted by: Hummie Posted at: 2016-06-20T16:56:43.032Z Reads: 32

```
  U can get just as hot and just as good efficiency with any voltage in a motor. The esc prefers higher voltage and otherwise will get hot but if the kv x volts gives u a speed range that is good and not too high its all the same in the motor with any voltage.  The motor still needs amps and just as many to the motor to produce needed torque
```

---
