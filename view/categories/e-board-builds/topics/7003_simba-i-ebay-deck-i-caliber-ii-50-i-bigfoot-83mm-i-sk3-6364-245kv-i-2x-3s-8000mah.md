# SIMBA I Ebay Deck I Caliber II 50° I Bigfoot 83mm I SK3 6364 245kv I 2x 3s 8000mAh

### Replies: 25 Views: 2649

## \#1 Posted by: TarzanHBK Posted at: 2016-08-02T11:44:22.766Z Reads: 243

```
Hallo Freunde! (i´m from Germany :slight_smile:)

A while ago I found that funny guy named Casey Neistat cruising around with his Boosted. As a big fan of funny stuff like that i searched a bit and found you guys here and that there is a good way and the possibility of diy your own board. So i bought my first parts after a bit of research from Hobbyking:

- SK3 6364 245 kV Motor - http://www.hobbyking.com/hobbyking/store/__18128__Turnigy_Aerodrive_SK3_6364_245kv_Brushless_Outrunner_Motor.html

- 2 x Zippys 3s 8000mAh
http://www.hobbyking.com/hobbyking/store/__16225__ZIPPY_Flightmax_8000mAh_3S1P_30C_Lipo_Pack.html

- Turnigy T100 Charger
http://www.hobbyking.com/hobbyking/store/__80421__Turnigy_T100_Multifunction_Touch_Screen_Battery_Charger_EU_plug_.html

Few Days ago my Ebay Board (50 Eus) arrived, which gave this project the name
<img src="/uploads/db1493/original/2X/8/82b10069bf53e0c32bbc31513f29bd1a4713d4a4.jpg" width="500" height="260">

Now to the missing parts:
Thanks to @elkick we got a pretty nice party supply here in the EU

- Transmission Kit from esk8.de http://www.hellray.de/shop/#!/eSk8-de-Black-Single-Setup-links/p/56131448/category=15255001
And because im 85kg on single drive, i´ll go for a 15mm drive system 15/36 gearing

- Micro Remote http://www.hellray.de/shop/#!/eSk8-de-Micro-Remote-2-4GHz/p/68315132/category=15842017

Now to the things im still not sure about:

- Getting a VESC and risking a lot of overheating, due to my weight and hilly area?
- Getting a VESC and another 3s battery to go for 9s and a 12/36 gearing? What about charging batterys then?
- Getting a Hobbyking X-Car Beast 150A for cheap, but risking not to be so satisfied because of not having a VESC :D (perhaps upgrading to VESC 6.0 - when its finally here in a few years :stuck_out_tongue_winking_eye:)

Did i miss something?
Thoughts?

:monkey:

EDIT: I know: "Go for a 18650!" -perhaps next time on a dual?! This time i´d like to keep my stuff :slight_smile:
```

---
## \#2 Posted by: Workaround Posted at: 2016-08-02T12:16:33.422Z Reads: 219

```
VESC are the best option then can handle up to 10S. I have seen VESCs handle hills fine. I have never seen anyone doing tests of car ESC doing that. Might just be me not finding those videos on the Internet or people not uploading cause some really bad fail(don't want to look dumb on the Internet for those trolls).

We would need to have the weight and ruff ideas of hilly area's inclines to give accurate information.

I would not go to to 9s because it takes longer to charge all batteries. You could just sacrefice some top speed and go to 14/36. Use http://calc.esk8.it/ to help cause I'm assuming you have tires of 83mm.

Remember that LiPo batteries don't like to go down to 3.75 or bellow so you should get a battery monitor that atleast beeps when they are low.
```

---
## \#3 Posted by: TarzanHBK Posted at: 2016-08-02T12:25:57.921Z Reads: 207

```
I just saw a few guys here, who got heat problems with the vesc and 6s, espacially on an 63mm motor.

9s charging should be possible with a parallel charging board right? But i have to take the batterys out and connect each one on that charging board. Something like that:
http://www.hobbyking.com/hobbyking/store/__41783__Hobbyking_Parallel_Charging_Board_for_6_Packs_2_6S_XT60_EC5_T_Connector_.html?strSearch=charging%20board

If i would get a vesc, i dont need battery monitoring, due to vesc shutdown ability.
If i go the standart esc-way, i think i have to monitor the batterys.
```

---
## \#4 Posted by: Maxid Posted at: 2016-08-02T12:41:48.713Z Reads: 186

```
You got a link to that deck?
```

---
## \#5 Posted by: TarzanHBK Posted at: 2016-08-02T12:46:42.480Z Reads: 185

```
Here you go with Amazon:
https://www.amazon.de/Longboard-Skateboard-Surfboard-Longboards-00018/dp/B00WX0QNII/ref=sr_1_10?s=sports&ie=UTF8&qid=1470141880&sr=1-10&keywords=longboard

Aaaand here on Ebay:
http://www.ebay.de/itm/Longboard-Long-Board-Skateboard-Surfboard-komplett-Flex-Longboards-medium-high-/400910298419?var=&hash=item5d581dad33:m:mMDbAww75jr3UfiXWTCadZQ
```

---
## \#6 Posted by: anorak234 Posted at: 2016-08-02T16:06:05.968Z Reads: 180

```
Suggestion - don't use a parallel charging board. Make a series adapter. Parallel charging boards send the average of cell voltage to your balance charger, so if 1 cell is at 3.4 on your first battery and 1 cell is at 4.2 then the charger will charge based on the average of those cells, 3.8. Parallel charging can potentially overcharge and unbalance your cells overtime, not a great idea.
```

---
## \#7 Posted by: XIII Posted at: 2016-08-02T16:13:37.595Z Reads: 172

```
How can their be a difference if they are connected to each other? They can't have a different voltage when they are in parallel. 

Thats some of the basics I learned in school. Strange
```

---
## \#8 Posted by: anorak234 Posted at: 2016-08-02T16:21:24.458Z Reads: 164

```
That's if they are also discharging in parallel. He is talking about running the board in series and then charging in parallel
```

---
## \#9 Posted by: elkick Posted at: 2016-08-02T16:28:34.863Z Reads: 165

```
You should go rather for 9s if you're considering to use 63 motors with a VESC. But then again, 245kv is rather high, so 9s might be close to the limit. If you already have that motor I'd go with either VESC v6 or an ESC like torqueboards.
```

---
## \#10 Posted by: XIII Posted at: 2016-08-02T17:01:41.397Z Reads: 162

```
the moment they get connected in parallel they will equal out. 

you can't have a closed circuit where you have 3.7 v in parallel with 3.4V. 
Current will rush towards the 3.4V cell. And the cells will immedialty balance out at (for example) 3.5V
```

---
## \#11 Posted by: XIII Posted at: 2016-08-02T17:02:10.051Z Reads: 150

```
already news from the Vesc V6 ? :slight_smile:
```

---
## \#12 Posted by: chickasskick Posted at: 2016-08-02T18:21:41.054Z Reads: 141

```
Ah nice thank you! I've been looking for a board in the EU that doesn't cost an arm and a leg in shipping! :smiley:
```

---
## \#13 Posted by: TarzanHBK Posted at: 2016-08-03T06:37:44.878Z Reads: 138

```
So it shouldn´t be a problem riding 9s in series and charging in parallel. Also should be possible to run the 245 sk3 with a reduced gearing like 12/36 to reach about the perfect 8000rpm to 8500rpm. Am I right there?

At the moment im still not sure wich way works best for me, so perhaps i´ll buy the x-car beast first and later on the v6 VESC and another 3s lipo for science.
:monkey:
```

---
## \#14 Posted by: bigben Posted at: 2016-08-03T06:50:04.614Z Reads: 133

```
The FVT120 is a cheap 6s esc that is available from bangood with free shipping in the eu. Probably around 45 euros?
```

---
## \#15 Posted by: susplus Posted at: 2016-08-03T11:26:50.875Z Reads: 130

```
Ebay.de has a lot of options also....even better i might say :D
```

---
## \#16 Posted by: chickasskick Posted at: 2016-08-03T11:48:49.204Z Reads: 132

```
Hi, yep have been checking them out all morning thanks! So glad I saw this post, really been struggling to find a board that I want without having to pay horrendous shipping fees :frowning:
```

---
## \#17 Posted by: Maxid Posted at: 2016-08-03T11:51:30.471Z Reads: 133

```
on amazon.de there is a 38" santa cruz complete board for 62€ (original price ~210€) - might be worth a look.
https://www.amazon.de/Santa-Cruz-Longboard-Armageddon-SANLOBARM/dp/B01AA9TUGK/ref=sr_1_24?ie=UTF8&qid=1470147549&sr=8-24&keywords=madrid+longboard
```

---
## \#18 Posted by: chickasskick Posted at: 2016-08-03T12:28:00.135Z Reads: 128

```
Thanks! I'll add it to my list of boards to check out :smiley:
```

---
## \#19 Posted by: Workaround Posted at: 2016-08-04T13:54:59.141Z Reads: 112

```
Charging boards are a bunch of Bull. You are going to have problems charging more then 6s at a time.

The problems are if your charger is designed for 3s(most chargers are designed for 3s but can to 6s) it will take twice as long to charge 6s. Most chargers have a time protection in them so they don't stay on and keep charging the batteries when they are already charged(not charge but keep heating them up which may damage then or cause a fire). Protection from damaging the batteries is great but it means you need to unplug and plug back in.

I would just buy more chargers then do this parallel charging. I also have a voltage leveler for 6s which is my setup.

Edit: If it it not clear why it takes longer to charge your batteries it is the fact your charger is not going to pull more watts to charge more batteries.
```

---
## \#20 Posted by: WeeChumlee Posted at: 2016-08-04T14:20:25.023Z Reads: 104

```
Hi
If you are going to use the batteries listed above then a relatively cheap 6S charger will be fine.
Personally I would not use the VESC on 6S and 63mm motor as they do overheat - mine did even on 8S while going up steep hills. The FVT120 or FVT150A ESCs are very cheap and are decent enough. In my opinion you should start with one of them, You can always upgrade to a VESC 6 later if you wish but you may well be happy enough as it is.
Like many of us, if the first board works well you may well build a second so use the first board as a test run. 6S battery, charger, FVT ESC and you are good to go without experimenting to much and keeping costs low.
```

---
## \#21 Posted by: TarzanHBK Posted at: 2016-08-04T15:30:42.938Z Reads: 92

```
yea, i think i have to try it and see how long this will take with my charger..
never heard of a "voltage leveler" before? what should that do ? :D
```

---
## \#22 Posted by: TarzanHBK Posted at: 2016-08-04T15:35:05.173Z Reads: 90

```
my descision for now is a cheap esc like the x-car beast or a fvt and my 6s and i´ll see how that turns out.
but later on, i´ll definitaly try my motor with a 9s setup, because of science
:monkey:
```

---
## \#23 Posted by: Workaround Posted at: 2016-08-04T17:02:48.939Z Reads: 90

```
You probably have one built into your charger but what I have is a little device that you connect to a 6s(two 3s packs in series) pack and it will level out any huge differences in voltage from each cell.
```

---
## \#24 Posted by: TarzanHBK Posted at: 2016-08-05T11:09:15.609Z Reads: 89

```
Okok you mean a balancing unit like a BMS or, how i´d like to do it, a simple balancing cable to connect my 2 3s lipos with my charger (which is able to balance cells to 6s).
Another simple way of balancing batterys is to connect them in parallel.
```

---
## \#25 Posted by: Workaround Posted at: 2016-08-05T12:15:37.879Z Reads: 87

```
I do recommend just using 6s2p or what I do cause my case(mini fish box with no sorting) can only hold 2 3s 5ah packs I just swap them when needed. BMS motors when charging or discarding is what I believe. I have this thing that just levels stationary batteries.
```

---
