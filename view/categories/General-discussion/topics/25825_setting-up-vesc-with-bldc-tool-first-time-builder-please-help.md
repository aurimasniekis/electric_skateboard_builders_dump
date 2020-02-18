# Setting up vesc with bldc tool, first time builder please help

### Replies: 54 Views: 5246

## \#1 Posted by: Shahar9320 Posted at: 2017-06-21T05:20:22.342Z Reads: 394

```
Hi everyone! This is the first time I'm building a board and I don't really understand how to configure the vesc.. if anyone can help that would be great.
Specs of the board:
Motor: single 6374 ,190kv , max power: 3150W, max amps: 80.
Vesc: voltage: 8-60v,  current: up to 240a for a few seconds and 50a continues.
Battery: 12s2p 18650 cells.
Bms: 30a continues, 80a peak.
Gear ratio: 13/36.
Belt: 12mm width 255mm length.
83mm wheels.

Highlighted the things I need help with. Thank you very much in advance 
<img src="/uploads/db1493/original/3X/f/0/f00fb3786d986576a8d102fa917d60340c90cb95.JPG" width="690" height="383"><img src="/uploads/db1493/original/3X/7/8/7836fb6a1fc26219e5e15ed4a6f41f323b6a5174.jpg" width="690" height="361">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-06-26T16:56:21.980Z Reads: 334

```
You can find info about various settings here
http://vedder.se/2015/01/vesc-open-source-esc/
```

---
## \#3 Posted by: Alanhunt123 Posted at: 2017-06-27T03:56:53.059Z Reads: 330

```
Here's another good resource available right here on the forum that will help you understand the VESC a little better.

http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980

I'd try starting with 80A motor max/min and 40A battery max/min. Absolute max, maybe 120A? Maybe someone else can chime in.

Duty cycle can be left alone, and you can put max voltage to 57, and leave minimum to 6, should be fine.

All of the stuff in your second window screencap is generated after doing a motor detection, so not to worry.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-06-27T04:05:39.564Z Reads: 276

```
The Absolute max can go as high as 150a.
I would not recommend setting it too low because it is intended to kick in if the soft back off strategys fail.
I believe this implies that the absolute max if triggered will cause a sudden loss of power.
The info about this setting is in Vedder's page that I posted.
The default setting is 130a.  
I run my dual setups with Lipo battery pack
absolute max at 140a
motor max at 80a
Batt max at 60a
Motor min at -40a
Batt min at -10a
```

---
## \#5 Posted by: Shahar9320 Posted at: 2017-06-27T04:09:06.880Z Reads: 244

```
Thanks very much guys
```

---
## \#6 Posted by: Shahar9320 Posted at: 2017-06-27T08:05:06.192Z Reads: 232

```
Wouldn't -80a motor min  rip the belt? I thought the -60a Is ok and i saw a tutorial in which he said that this is also too much for the belts
```

---
## \#7 Posted by: Shahar9320 Posted at: 2017-06-27T08:06:42.060Z Reads: 229

```
And why the battery min and max is 40? Could you explain? From what I understood the battery min should be lower to maximize battery life and I don't really know about battery max
```

---
## \#8 Posted by: Shahar9320 Posted at: 2017-06-27T08:27:03.394Z Reads: 227

```
If I have a bms that is rated for 30a continues and 80a peak, shouldn't I be setting the battery max to 80? It should I take it down to 60a?
```

---
## \#9 Posted by: Shahar9320 Posted at: 2017-06-27T10:03:18.962Z Reads: 225

```
<img src="/uploads/db1493/original/3X/1/9/19e4dd1bd13d604ffe8b6d32aa61668118153a7a.png" width="690" height="328">
what do you say about those settings?  i dont understand a few things:
1. the motor is rated for 80 amps max but shouldn't it be 3150w / 44.4v = 70.9 amps?
2. is -60a motor min ok? or is it too much for the belt?
3. i dont understand what the battery max should be.. the bms is 30a continues and 80a peak. the battery is 12s2p 18650 2900mah cells.

any help would be much appreciated!
```

---
## \#10 Posted by: Martinsp Posted at: 2017-06-27T10:12:14.870Z Reads: 218

```
Hey! 

The motor is rated for 80A max which probably is not continuous but peak that the windings can withstand before failing or overheating 
-60A and 60A is OK... most of the people use this setting.. i do on 9mm belt on my dual setup and no problems for over a year.
battery max in your case i would set to 30A which should be OK. Maybe even too much. It depends on the area you live in because on flats you are going to pull 30A from your battery only when accelerating pretty hard or when riding up hills. It also depends on your weight, wind and stuff but generally 30A should be good.
```

---
## \#11 Posted by: Martinsp Posted at: 2017-06-27T10:13:34.484Z Reads: 207

```
oh i didnt notice... with 12S 30A is a lot of power... i have my battery max set to 20 on 10S but again... it is dual setup but it is more than enough
```

---
## \#12 Posted by: Shahar9320 Posted at: 2017-06-27T10:25:15.769Z Reads: 201

```
So bottom line is this ok?
Motor max:70
Mottor min: -60
Battery max: 30/20?
```

---
## \#13 Posted by: Martinsp Posted at: 2017-06-27T10:29:04.351Z Reads: 193

```
Well.. it is ok for the VESC and battery so you should not destroy anything due to this. Id suggest just put it to this:
Motor max 60
Motor min -60
Battery max 25
(with these values you wont destroy anything)
Test it and see if it is OK... If you want faster acceleration or higher hills increase motor max, stronger braking decrease motor min to say 65 and test.
It is all about fine tuning it to suit your needs.
```

---
## \#14 Posted by: Shahar9320 Posted at: 2017-06-27T10:31:33.068Z Reads: 189

```
Thank you so much! And battery min is -12 right? 2 times 6ah
```

---
## \#15 Posted by: TarzanHBK Posted at: 2017-06-27T10:33:00.704Z Reads: 187

```
if you´re using 18650 Liion cells, you have to adjust your Battery cutoff start and end:
3,0V/cell start, 2,8V/cell end.
So if you´re on 12s, thats 12 x 3V = 36V Cutoff start
12 x 2,8V = 33,6V Cutoff end
```

---
## \#16 Posted by: Shahar9320 Posted at: 2017-06-27T10:35:08.358Z Reads: 180

```
I set it higher at 40 and 38 so it wound better on the battery.. what do you think about these settings: 
Motor max:70a, min:-60a
Battery max;30a,min:-12?
```

---
## \#17 Posted by: Martinsp Posted at: 2017-06-27T10:39:54.508Z Reads: 176

```
The charging current should be at 1C per cell in parallel so if you have 2P it is 1C*2=2C which is 2*capacity=5800mA so id set the charging (battery min (regen))to 6A.

The voltages are safe at cutoff end 36V (3V per cell in series) and the cut off start is up to you.. it is pretty much just a notification for you that you are low on battery that your board starts to go slower.

Manufacturers state their mAh when discharging batteries from 4.2V down to 2.5V so you have somewhere around 2500/2600 of actual usable capacity.
```

---
## \#18 Posted by: Shahar9320 Posted at: 2017-06-27T10:40:50.166Z Reads: 174

```
im 70kg but there are a lot of hills where i live.. so battery max is 30? i dont understand why should i set it anyway if i have a bms.. could you please explain this?
```

---
## \#19 Posted by: Martinsp Posted at: 2017-06-27T10:45:27.260Z Reads: 175

```
Ok then set it to 30 even 40 might be still good enough concidering that you wont pull it from the battery all the  time.

You set it in your VESC so that you dont pull those 80A from your battery through BMS (bms would allow say 70A peak (at 80 it disconnects battery due to overcurrent) but VESC could pull it in worst case scenario continuously and therefore destroy your BMS and battery)
```

---
## \#20 Posted by: TarzanHBK Posted at: 2017-06-27T10:51:49.305Z Reads: 172

```
if you have a lot of hills and weight 70kg i don´t recommend a 12s2p. It´s too small for some hills and your cells will sag a lot. What cells are you using?
```

---
## \#21 Posted by: Shahar9320 Posted at: 2017-06-27T11:02:48.374Z Reads: 161

```
The cells are 18650 Panasonic but f cells.. why do you say that it is too small? Isn't the voltage what matters?
```

---
## \#22 Posted by: TarzanHBK Posted at: 2017-06-27T11:07:25.494Z Reads: 157

```
what Panasonic cells? 
Voltage matters too, but in this case it´s their continuos discharge capability
```

---
## \#23 Posted by: Shahar9320 Posted at: 2017-06-27T11:27:47.340Z Reads: 155

```
Panasonic pf cells 2900 mah
```

---
## \#24 Posted by: Shahar9320 Posted at: 2017-06-27T11:28:23.442Z Reads: 152

```
Can't afford bigger battery at this voltage
```

---
## \#25 Posted by: TarzanHBK Posted at: 2017-06-27T12:18:26.458Z Reads: 149

```
this cell is capable of 10A max, so with 12s2p 20A max.
You´ll kill them pretty fast!
If you can´t afford it, save a bit longer for proper cells or get lipos.
```

---
## \#26 Posted by: Shahar9320 Posted at: 2017-06-27T13:12:30.634Z Reads: 142

```
How much difference is ther between 12s2p and 12s3p for that setup? Is it really worth it??
```

---
## \#28 Posted by: TarzanHBK Posted at: 2017-06-27T13:59:25.228Z Reads: 141

```
even 12s4p will be too weak with these cells.
Do yourself a favor and do a bit more research here, before you waste your money on wrong parts.
```

---
## \#29 Posted by: Namasaki Posted at: 2017-06-27T17:29:38.551Z Reads: 139

```
I think of the batt max as a peak setting not continuous. 
I set my batt max at 60 with no problem. 
I know someone who has run it higher. With no problem. 
If the Vesc gets too hot the temp protection will shut it down. 
I'm thinking about turning mine up more as well.
```

---
## \#30 Posted by: Shahar9320 Posted at: 2017-06-27T17:34:55.529Z Reads: 133

```
Customer support told me to set it to 70a as it is the peak for my battery
```

---
## \#31 Posted by: Shahar9320 Posted at: 2017-06-27T17:39:10.386Z Reads: 132

```
These cells are 15a discharge so I'll have 30a continues and 70 peak. Also I'm not planning on traveling for much distance each time (something like 3-4 miles) so although I do have some hills here , the sag wouldn't be so bad right?
```

---
## \#32 Posted by: Shahar9320 Posted at: 2017-06-27T17:41:26.287Z Reads: 130

```
I don't have a lot of steep hills here just some streets that are in some incline (nothing really crazy..)
What do you think?
```

---
## \#33 Posted by: Namasaki Posted at: 2017-06-27T19:00:33.455Z Reads: 130

```
[quote="Shahar9320, post:30, topic:25825, full:true"]
Customer support told me to set it to 70a as it is the peak for my battery
[/quote]

Yes, I really should have mentioned that it is important to consider the limits of your battery.
```

---
## \#34 Posted by: Shahar9320 Posted at: 2017-06-27T19:02:28.693Z Reads: 132

```
do you think i should just switch to lifepo battery?
```

---
## \#35 Posted by: Namasaki Posted at: 2017-06-27T21:06:26.945Z Reads: 129

```
I use Lipos for max power in a small light battery
```

---
## \#36 Posted by: Shahar9320 Posted at: 2017-07-01T09:48:32.016Z Reads: 131

```
<img src="/uploads/db1493/original/3X/0/a/0ae81360f55ef13b2e8e67ad79fea89d727b8011.png" width="690" height="258">

what do you think about these settings?
```

---
## \#37 Posted by: cledus Posted at: 2017-07-01T17:38:02.973Z Reads: 124

```
Hi all!!!

Really great answers to a lot of good questions. I´m planning on buying a 18650 10S3P. The cells that will be used is 3400mAh. Would you say that is to small? I will be buying my motor and VESC from diyelectricskatboard.com. (their 3674 190kv) and VESC.

Thanks again!
/Andreas
```

---
## \#38 Posted by: Shahar9320 Posted at: 2017-07-01T17:44:27.260Z Reads: 123

```
isnt too small is a great size.. not too big not too small. what is their discharge rate?
```

---
## \#39 Posted by: cledus Posted at: 2017-07-01T19:01:36.361Z Reads: 123

```
Hi!

I talked to the guy who's making the battery. I misunderstood him. He said that the battery had a max discharge rate of 30A. But he was talking about each parallel pack. So for the whole pack it will be 90A whitch should be enough. The BMS is limited to 40A. Do you think that is to small? Should I have a stronger BMA?
```

---
## \#40 Posted by: Shahar9320 Posted at: 2017-07-01T19:13:36.829Z Reads: 119

```
It'll be awesome man! I just ordered the 12s2p and it has 30/70 amps , but i don't need much range..
```

---
## \#41 Posted by: Shahar9320 Posted at: 2017-07-01T19:14:30.390Z Reads: 120

```
Is it 30a peak or continues? It should be really great
```

---
## \#42 Posted by: cledus Posted at: 2017-07-01T19:35:40.064Z Reads: 115

```
Its 90A peak :-D!
```

---
## \#43 Posted by: cledus Posted at: 2017-07-01T19:36:11.221Z Reads: 114

```
But I wonder if 40A BMS is to small
```

---
## \#44 Posted by: Shahar9320 Posted at: 2017-07-01T19:47:27.581Z Reads: 114

```
I think you should go a little higher. Maybe 60 or even80
```

---
## \#45 Posted by: Namasaki Posted at: 2017-07-01T22:51:17.020Z Reads: 113

```
I run the motor min at -40 and the brakes are fine
Your battery cutoffs are not correct 
You need to put the temp cutoffs back to default.
```

---
## \#46 Posted by: Shahar9320 Posted at: 2017-07-02T06:10:20.473Z Reads: 113

```
<img src="/uploads/db1493/original/3X/d/8/d89db43fb1f20e7c52f75fa471262d903c03423d.png" width="690" height="259">

?? thanks again :slight_smile:
```

---
## \#47 Posted by: Namasaki Posted at: 2017-07-02T06:12:47.873Z Reads: 112

```

These are my settings for dual Vescs powered by 5000mah / 60C  10s Lipo battery.

<img src="/uploads/db1493/original/3X/4/b/4b39e9378b7259eb355725d9995eb6d11a5129dd.png" width="690" height="362">
```

---
## \#48 Posted by: cledus Posted at: 2017-07-03T09:44:43.733Z Reads: 101

```
Namasaki What's your BMS at?
```

---
## \#49 Posted by: Namasaki Posted at: 2017-07-04T04:41:18.100Z Reads: 98

```
my bms is 80a continuous and 200a peak
with 2 Vescs set at 60a max, I have not tripped the bms by current or heat.
```

---
## \#51 Posted by: NickTheDude Posted at: 2017-07-07T23:57:57.933Z Reads: 96

```
Using the 10S battery should be fine. Make sure you set your voltage hard and soft cutoffs to around 3.6V per cell and 3.4V per cell. 40A battery amps and 80A motor amps should be good for that setup. If you want more juice you could probably raise them to ~50 and ~100 without trouble.

Also be veeeery veeeery careful when you  solder your battery leads. Make sure they don't touch each other or boom.
```

---
## \#50 Posted by: Shahar9320 Posted at: 2017-07-08T00:34:02.590Z Reads: 97

```
hi guys, first time builder and i want to avoid any mistakes so please tell me if im going to destroy something.
i got the vesc and 6374 motor from DIYes, and my battery is 10s3p with 25r cells (60amp discharge, 7.5 ah).
before i do anything with the vesc, i intend to remove the xt90 connector on the vesc and solder the battery's discharge wires directly to the vesc's wires. (the battery will have a switch).
and i will be configuring the vesc with this 10s battery (the guy on the diyes website said its okay but some people said its not).
any help would be much appreciated :slight_smile:
```

---
## \#53 Posted by: Shahar9320 Posted at: 2017-07-08T07:11:19.581Z Reads: 84

```
of course . its not me who does this its the pros who are building the battery for me. thanks for the help man
```

---
## \#54 Posted by: cledus Posted at: 2017-07-14T13:34:10.425Z Reads: 74

```
Thanks for the reply! But after I have done some reading I wounder why would you need a BMS to handle anything else but the charging of the battery if you have a VESC where you can set the max and min that the motor can draw from the battery?
```

---
## \#55 Posted by: Namasaki Posted at: 2017-07-14T14:40:06.565Z Reads: 68

```
The Vesc limits amps drawn from the battery. 
The BMS monitors the battery on a individual cell or cell group level and protects against over discharging and external shorts. 

The Vesc can't do that because it can only monitor the battery pack as a whole.
```

---
## \#56 Posted by: cledus Posted at: 2017-07-14T15:27:38.292Z Reads: 69

```
Ok. But if the VESC limits the amps drawn from the battery the BMS doesn't have to be bigger/stronger than what you specified in the VESC right?
```

---
