# Switch Battery on Buffalo A3

### Replies: 22 Views: 1153

## \#1 Posted by: Manola1027 Posted at: 2017-11-19T15:57:47.325Z Reads: 96

```
Hello,

I recently bought a Buffalo A3. It has a defective battery so it only last about 2 km. Its a 22V 4.4Ah battery. I am looking for a new one and found an interesting 6s5p on aliexpress.
I am thinking it should be an easy switch. I'll have to come up with a new enclosure but I have a 3d printer so that wont be much of an issue. The only downside to this battery is probably the way the cells are positioned, making it very bulky. But it will fit the board. I just want to make sure it will work.

<img src="/uploads/db1493/original/3X/f/7/f7346fda5ed15b9b79fb2c44d36cf6a7673e0cfe.jpeg" width="304" height="500"><img src="/uploads/db1493/original/3X/0/5/050c253de33bc0b2e59529fea106696c9a1b0d9a.jpg" width="666" height="500">

https://www.aliexpress.com/item/HK-LiitoKala-Brand-cells-24V-10Ah-6S5P-battery-pack-lithium-350w-e-bike-li-ion-25/32810076088.html?ws_ab_test=searchweb0_0,searchweb201602_1_10152_10065_10151_10344_10068_10345_10342_10343_10340_10341_10171_10541_10562_10084_10083_10307_10301_10303_10060_10155_10154_10539_10312_10059_10313_10314_10534_10533_100031_10103_10073_10594_10557_10596_10595_10142_10107,searchweb201603_25,ppcSwitch_5&btsid=674fbf17-7466-4a3e-b939-5c9cd9c8db67&algo_expid=d829df9c-cb03-4c0e-9d23-0ac25bd5749b-0&algo_pvid=d829df9c-cb03-4c0e-9d23-0ac25bd5749b&rmStoreLevelAB=0
```

---
## \#2 Posted by: aigenic Posted at: 2017-11-19T16:06:25.510Z Reads: 88

```
No, it wont work for two reasons:
1. Its too big
2. It cant output enough amps, its too weak...
```

---
## \#3 Posted by: aigenic Posted at: 2017-11-19T16:08:25.076Z Reads: 83

```
If you want that to be as cheap as possible, buy 6S lipo battery :)
```

---
## \#4 Posted by: Manola1027 Posted at: 2017-11-19T16:19:23.675Z Reads: 83

```
[quote="aigenic, post:2, topic:38752, full:true"]
No, it wont work for two reasons:
1. Its too big
2. It cant output enough amps, its too weak...
[/quote]

It's not too big. I can make it work:)
Not having enough output might be a problem though. On the website it says
The maximum peak current: 36A
 Maximum operating current: 18A
Is that too weak? It is advertised as an electric bike battery so it should work right?

[quote="aigenic, post:3, topic:38752"]
If you want that to be as cheap as possible, buy 6S lipo battery :slight_smile:
[/quote]
I looked it up. If we take this one for example:
https://www.ebay.com/itm/You-Me-6S-5000mAh-22-2v-50C-Lipo-Battery-Pack-Helicopters-Airplanes-RC-DJI-Drone/112275694687?hash=item1a2427245f:g:Xo8AAOSwc~BZkV5K
That should get me a max output of 5.0 x 50 = 250A.
Is that correct? For higher than the ali express battery
```

---
## \#5 Posted by: aigenic Posted at: 2017-11-19T16:37:59.769Z Reads: 66

```
Ok, lets do the math...
Buffalo A3 has 1200W motor running on 22.2V battery...that means it needs 1200W / 22.2V = 54 A of pea current :) They LiPo you have linked is okay :) you can choose LiPo with lower discharge rating...5AH 20C battery would do the work easily :) ALso I would rather buy 2 3s lipos and connect them in series to make the build less bulky, but thats up to you :) 
Where are you from?
```

---
## \#6 Posted by: Manola1027 Posted at: 2017-11-19T17:35:03.668Z Reads: 59

```
[quote="aigenic, post:5, topic:38752"]
Ok, lets do the math...
Buffalo A3 has 1200W motor running on 22.2V battery...that means it needs 1200W / 22.2V = 54 A of pea current :slight_smile: They LiPo you have linked is okay :slight_smile: you can choose LiPo with lower discharge rating...5AH 20C battery would do the work easily :slight_smile: ALso I would rather buy 2 3s lipos and connect them in series to make the build less bulky, but thats up to you :slight_smile: 
Where are you from?
[/quote]

Thanks, i didn't realise how to calculate what I need:) I will look into Lipos som more. But if I get that I would need a charger as well right? Or maybe BMS if I want one port charging? 
I am from Sweden:)
```

---
## \#7 Posted by: aigenic Posted at: 2017-11-19T18:03:05.848Z Reads: 48

```
there should be BMS in your Buffalo skateboard already...you could use that one :) it should work even with Lipos :)
```

---
## \#8 Posted by: Manola1027 Posted at: 2017-11-19T18:15:33.057Z Reads: 51

```
[quote="aigenic, post:7, topic:38752"]
there should be BMS in your Buffalo skateboard already...you could use that one :slight_smile: it should work even with Lipos :slight_smile:
[/quote]

This is how the old battery was connected.
<img src="/uploads/db1493/original/3X/6/1/616a55f153c90f21427f1817a421bc286773a038.jpg" width="375" height="500">

The charging port is in the bottom left of the picture and the battery connects to the electronics on the other end. Do you mean that the bms is build in along with the electronics? Because if thats true then the bms is on the opposite side from the charger. I thought it had to be between the battery and the charger? 


Anyway I found some LiPos I like. 
This one is the most interesting:
https://hobbyking.com/en_us/zippy-compact-5800mah-6s-25c-lipo-pack.html

And possibly a charger if I cant figure out how to use the one I have
https://hobbyking.com/en_us/imax-b6-ac-dc-charger-5a-50w-with-us-plug-copy.html
```

---
## \#9 Posted by: Youssless Posted at: 2017-11-19T18:17:45.819Z Reads: 43

```
How would a 6S5P not give out enough amps? If 30Q cells are used (which are rated safely to 20A continuous) then that's 100A or 75A if you take the 15A discharge rating.

I get that his pack is low voltage at 6S but surely 5P would have ample current?
```

---
## \#10 Posted by: Manola1027 Posted at: 2017-11-19T18:30:35.107Z Reads: 44

```
[quote="Youssless, post:9, topic:38752, full:true"]
How would a 6S5P not give out enough amps? If 30Q cells are used (which are rated safely to 20A continuous) then that's 100A or 75A if you take the 15A discharge rating.

I get that his pack is low voltage at 6S but surely 5P would have ample current?
[/quote]

I can't find any information on what kind of cells are used. Probably not 30Q. They tell you information about the discharge rate

The maximum peak current: 36A
Maximum operating current: 18A

It would be great if this pack works though:)
```

---
## \#11 Posted by: Youssless Posted at: 2017-11-19T18:39:04.796Z Reads: 40

```
Ah I misread and thought you were thinking to make your own pack.

Yeah I'm sceptical of 'Big brand 18650 cells . Good quality!' Stick with a lipo I'd say, you'd definitely need a balance charger if you don't have one already.
```

---
## \#12 Posted by: aigenic Posted at: 2017-11-19T18:49:42.260Z Reads: 36

```
The battery pack you have has build in BMS probably...you are connecting just the two wires to the charger when you are charging am I right? 
The charger you linked will be ok :) Imax is comonly used by builders :)
```

---
## \#13 Posted by: Manola1027 Posted at: 2017-11-19T18:55:43.741Z Reads: 40

```
[quote="aigenic, post:12, topic:38752"]
The battery pack you have has build in BMS probably...you are connecting just the two wires to the charger when you are charging am I right? 
The charger you linked will be ok :slight_smile: Imax is comonly used by builders :slight_smile:
[/quote]

That could be it:) which to wires do you mean? I plug in a laptop style charger

It's an Imax clone. Will look around a bit. Is it possible to get a bms for the lipo?
```

---
## \#14 Posted by: aigenic Posted at: 2017-11-19T19:00:05.409Z Reads: 39

```
Yes, it is possible to get BMS for the lipo :) they are quite cheap :) you would use the lapop style charger you alredy have :) You just need to solve the proper wiring to the BMS, some basic soldering (charging cable to BMS) will  be probably needed :)

If you plug it into a laptop style charger then it has BMS build inside the battery pack :)
```

---
## \#15 Posted by: Manola1027 Posted at: 2017-11-23T13:06:41.811Z Reads: 22

```
[quote="aigenic, post:14, topic:38752"]
Yes, it is possible to get BMS for the lipo :slight_smile: they are quite cheap :slight_smile: you would use the lapop style charger you alredy have :slight_smile: You just need to solve the proper wiring to the BMS, some basic soldering (charging cable to BMS) will  be probably needed :slight_smile:

If you plug it into a laptop style charger then it has BMS build inside the battery pack :slight_smile:
[/quote]

Do you know if this one would work?

http://www.diyeboard.com/7s2p-lg-18650-lithiumion-battery-pack-252v-4400mah-11088wh-p-457.html

It's made for electric longboards. Cant find information on the dischargerate though?

It's 7s though...
```

---
## \#16 Posted by: aigenic Posted at: 2017-11-23T14:58:28.119Z Reads: 20

```
Its 7s as you said, that could be a problem...I didnt find any discharge specs, try asking their support...but I wouldnt buy that, the higher voltage could destroy your board...
```

---
## \#17 Posted by: Manola1027 Posted at: 2017-11-24T22:46:19.406Z Reads: 20

```
What about this one?

https://www.aliexpress.com/item/24v-8ah-8000-mAh-6-series-of-lithium-battery-electric-vehicle-battery-moped-lithium-battery-battery/32646976118.html?ws_ab_test=searchweb0_0,searchweb201602_1_10152_10151_10065_10344_10068_10345_10342_10343_10340_10171_10341_10541_10562_10084_10083_10307_10301_10303_10539_10312_10059_10313_10314_10534_10533_100031_10604_10603_10103_10594_10557_10596_10595_10142_10107,searchweb201603_25,ppcSwitch_5&btsid=d44c29de-6401-4d81-a930-d2b0ea0d6924&algo_expid=2c52c96e-c2c6-440c-abc4-4f08bbf32d55-17&algo_pvid=2c52c96e-c2c6-440c-abc4-4f08bbf32d55&rmStoreLevelAB=1

3: Maximum instantaneous current: 60
 
4: Maximum operating current: 45

According to your calculation (1200/22.2 = 54 peak) 
Does that mean this battery works since 54 is between 45 and 60?
```

---
## \#18 Posted by: aigenic Posted at: 2017-11-25T07:44:59.244Z Reads: 20

```
Yep, this one would work, but it is so huuuuge...also chinesse Li-Ion batteries does not have the best quality...
```

---
## \#19 Posted by: Manola1027 Posted at: 2017-11-25T13:52:53.273Z Reads: 19

```
[quote="aigenic, post:18, topic:38752, full:true"]
Yep, this one would work, but it is so huuuuge...also chinesse Li-Ion batteries does not have the best quality...
[/quote]

I bought it now. We'll see how it works out hehe:)
```

---
## \#20 Posted by: aigenic Posted at: 2017-11-25T14:00:33.809Z Reads: 18

```
Good luck...
```

---
## \#21 Posted by: Holgerq Posted at: 2018-05-02T08:21:19.335Z Reads: 14

```
@Youssless I am thinking about making a 6s5p with 30Q. Do you think it will work?
```

---
## \#22 Posted by: Youssless Posted at: 2018-05-07T03:37:22.849Z Reads: 9

```
I don't see why not, though you need to consider other parts of your build. Remember that 6S will deliver a lower voltage and this will result in more heat output. 6s works and plenty of people have used it successfully, I just wanted to make you aware.
```

---
