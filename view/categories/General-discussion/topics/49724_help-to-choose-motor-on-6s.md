# Help to choose motor on 6s

### Replies: 13 Views: 517

## \#1 Posted by: MonkeyFist Posted at: 2018-03-21T13:42:42.422Z Reads: 58

```
Hello.
Which motor will be best on 6s.
[This one (5060, 280kv)](https://www.aliexpress.com/item/High-Quality-Racerstar-5060-BRD5060-280KV-4-12S-Brushless-Motor-Electric-RC-Motor-For-Balancing-Scooter/32824820002.html?spm=2114.search0104.3.35.743a46555LAf4g&ws_ab_test=searchweb0_0,searchweb201602_2_10152_10151_10065_10068_10344_10342_10343_10340_10341_10696_10084_10083_10618_10307_10313_10059_10534_100031_10103_10624_10623_443_10622_10621_10620,searchweb201603_2,ppcSwitch_4&algo_expid=e67a777d-137f-459a-82ba-d580678108f2-5&algo_pvid=e67a777d-137f-459a-82ba-d580678108f2&priceBeautifyAB=0) or [this one (6368, 280kv)](https://www.aliexpress.com/item/High-Quality-Racerstar-6368-BRD6368-280KV-6-12S-Brushless-Motor-Electric-Motor-For-Balancing-Scooter/32825934403.html?spm=2114.search0104.3.15.743a4655OMygk1&ws_ab_test=searchweb0_0,searchweb201602_2_10152_10151_10065_10068_10344_10342_10343_10340_10341_10696_10084_10083_10618_10307_10313_10059_10534_100031_10103_10624_10623_443_10622_10621_10620,searchweb201603_2,ppcSwitch_4&algo_expid=e67a777d-137f-459a-82ba-d580678108f2-2&algo_pvid=e67a777d-137f-459a-82ba-d580678108f2&priceBeautifyAB=0)?
6s, 15/36 gearing, 83mm wheels. Top speed around 34 km/h.
Which motor will be the best when using FVT120a, and why?
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-03-21T14:36:11.621Z Reads: 50

```
The 6368 will be better. Bigger is better :wink:
```

---
## \#3 Posted by: MonkeyFist Posted at: 2018-03-21T15:06:49.922Z Reads: 44

```
So it wont be too powerful for the 120a esc?
```

---
## \#4 Posted by: aigenic Posted at: 2018-03-21T15:14:26.593Z Reads: 41

```
I would go for [this one (5060, 270kv)](https://hobbyking.com/en_us/propdrive-v2-5060-270kv-brushless-outrunner-motor.html)...the difference is this one can take more amps on 6S, which means more power :)
```

---
## \#5 Posted by: FredrikHems Posted at: 2018-03-21T15:25:41.503Z Reads: 39

```
more amps doesn't necessarily means more power.. 
The 6368 will have a bigger stator, which means more torque/ability to take amps. 

Also, many people means that the 5060 propdrive really cant take 90 amps.. It gets burning hot.

@MonkeyFist No, you should be good. The best would be too buy a vesc though..
```

---
## \#6 Posted by: MonkeyFist Posted at: 2018-03-21T15:29:12.641Z Reads: 35

```
i've heard that vesc is not recomended for 6s. Because of the 50A limit. What do you think. How not to blow the vesc on 6s? :thinking:
```

---
## \#7 Posted by: bimmer Posted at: 2018-03-21T15:40:11.359Z Reads: 30

```
I doubt you will blow the Vesc on 6S.
```

---
## \#8 Posted by: MonkeyFist Posted at: 2018-03-21T15:42:17.471Z Reads: 27

```
Is it just to set Motor Amps and Battery Amps low to avoid vesc from blowing?
```

---
## \#9 Posted by: FredrikHems Posted at: 2018-03-21T16:01:56.654Z Reads: 27

```
In most vesc failures its the DRV who blows because of exceeding the 60k eRPM limit. 
This should be a problem for you since this setup will never reach over 50 eRPM.. 
An upgraded vesc, like focbox would be even better.
```

---
## \#10 Posted by: MonkeyFist Posted at: 2018-03-21T16:05:30.321Z Reads: 27

```
Okay. So exceeding the 60k erpm limit is the most common way to blow the vesc. But how do you set it up to not get too much heat? The amp limits?
```

---
## \#11 Posted by: Tuomalar Posted at: 2018-03-21T16:25:29.438Z Reads: 24

```
Kv x voltage x 7(poles?) equals erpm if i'm correct
```

---
## \#12 Posted by: MonkeyFist Posted at: 2018-03-21T16:27:20.426Z Reads: 24

```
You are correct.
```

---
## \#13 Posted by: FredrikHems Posted at: 2018-03-21T16:52:45.951Z Reads: 21

```
Yea, pushing way to much amps is also a way to destroy your vesc. But with like 40 (Many push 60+) battery amps, and 60 (Many do 100+) motor amps, you should be good. Its all about having the vesc stay cool. So if you add extra heatsinks + fans, the vesc can do a lot more than originally.
```

---
