# Drop in the plug

### Replies: 28 Views: 653

## \#1 Posted by: Davideariel Posted at: 2018-05-23T11:04:18.478Z Reads: 228

```
Hi everybody, 
i was riding when it started raining, i stopped immediatly.
but apparently a drop of water got into the plug of the space cell pro 4 plug.
i noticed when, once at home, i plugged in the charger; it sparked, i pulled the plug. I tried again a couple hours later, but it wasn't charging.
what might be broken? the power supply? the bms? the plug? how can i check?
any help is appreciated =)

have a nice day
```

---
## \#2 Posted by: dg798 Posted at: 2018-05-23T11:39:18.149Z Reads: 213

```
Open up your board and check all the wires are insulated and nothing is wet and then check all wires from charging port to BMS and see if u can see anything that can be a problem.
```

---
## \#3 Posted by: Battosaii Posted at: 2018-05-23T11:45:25.534Z Reads: 206

```
It could also be a faulty charger too
```

---
## \#4 Posted by: EverBlade21 Posted at: 2018-05-23T11:57:57.954Z Reads: 196

```
If there was a spark, something shorted. Its as simple as that, and assuming the spark came from the plug and you didn't say your breakers popped then unfortunately you no longer have a working battery pack.
```

---
## \#5 Posted by: pat.speed Posted at: 2018-05-23T12:19:08.750Z Reads: 169

```
How did you come to that conclusion? If the fuse didn’t blow then the short was not from the battery.

@Davideariel how loud was the pop? Was the spark big? Will the board turn on? And pictures will help a lot
```

---
## \#6 Posted by: Davideariel Posted at: 2018-05-23T12:39:33.835Z Reads: 152

```
The board does turn on and it shows the correct battery percentage, I checked the wires and they seem to be fine only the plug on the battery pack seems fried, but other than that everything seems fine, the motors spin and everything works, but it doesn't charge. 
I don't know if I have to change the plugs or get another BMS or buy another charger...
```

---
## \#7 Posted by: koralle Posted at: 2018-05-23T12:40:28.676Z Reads: 151

```
[quote="Davideariel, post:1, topic:56469"]
it sparked
[/quote]

What sparked? Open your enclosure and check thoroughly, usually you can see the burn marks

Edit: ok just read your reply. Usually the charger has a fuse inside methinks. Could also be blown
```

---
## \#8 Posted by: Davideariel Posted at: 2018-05-23T12:41:17.780Z Reads: 134

```
The only burn marks are one the plug, the one on the battery, everything else seems ok and not burnt.
```

---
## \#9 Posted by: koralle Posted at: 2018-05-23T12:42:56.069Z Reads: 129

```
[quote="Davideariel, post:8, topic:56469"]
the one on the battery
[/quote]

pics pls 
10char
```

---
## \#10 Posted by: dg798 Posted at: 2018-05-23T12:48:23.021Z Reads: 122

```
You may just have to replace the charging port and if there is a burn mark on the battery connector but it still works then I think that’s fine. I mean if it just doesn’t charge and there are no burn marks on the bms than it’s probably just the port
```

---
## \#11 Posted by: EverBlade21 Posted at: 2018-05-23T20:38:07.702Z Reads: 110

```
As I said before you definitely shorted something, if you can take the bms out and check if it works properly independent of the esk8. If it doesn't replace it. If the charging port is charred in any way you should replace that too but if the wires are fine then it should be a-ok
```

---
## \#12 Posted by: b264 Posted at: 2018-05-23T21:20:55.662Z Reads: 104

```
When something electronic gets wet, never ever use it or turn it on until a week has passed and it's completely dry.

Also like @koralle said, photos would help immensely
```

---
## \#13 Posted by: Martinsp Posted at: 2018-05-23T21:29:46.783Z Reads: 104

```
Actually in terms of electronics it is not a very good idea to leave something to dry out. At least not something that is powered like your phone notebook skateboard... remove the battery immediately from the circuit and then it is ok to let it dry. The presence of electricity speeds up corrosion which can be conductive (cause complete shorts or affect the resistance etc.) It is much better to displace the water with something noncorrosive like alcohol etc but still removing power source from the circuit is the best first step

In your case, measure the output voltage of the charger and if there is voltage present  on the charging port of the board. Be careful not to short stuff. If the board turns on, the problem is not the battery but maybe some fuse on the charging port if there is any, or part of the BMS or the charger (maybe fuse on output of the charger or input which is generally lower than breaker current which would explain why it did not flip if that was the case)
```

---
## \#14 Posted by: Davideariel Posted at: 2018-05-24T07:51:26.784Z Reads: 80

```
Today I will check the power supply, and the charging port with a tester, and post pics
```

---
## \#15 Posted by: Acido Posted at: 2018-05-24T10:24:14.094Z Reads: 74

```
Chargers have short protection
Its probably the bms fried
```

---
## \#16 Posted by: Davideariel Posted at: 2018-05-24T12:55:24.204Z Reads: 67

```
how can i know if the bms is fried? is there any way to check?
```

---
## \#17 Posted by: Davideariel Posted at: 2018-05-24T14:57:35.387Z Reads: 69

```
![IMG_20180524_165425655|375x500](upload://md8Co2T18807InTx9gU4oK4Zsvj.jpg)![IMG_20180524_165359706_HDR|375x500](upload://lziwFLbrelXdVEsriOgELmDRSUo.jpg)![IMG_20180524_165331045|666x500](upload://aya9bxQEB8fYE9a2xy0A1unR82b.jpg)![IMG_20180524_165258005_HDR|666x500](upload://weI8gokMDcbrMMFcC8H9wc5NWtq.jpg)

The board is dried and working (motors spin etc.). But it doesn't charge, I'm now trying to change the plugs... 
As soon as I didn't my tester I will check the powerbrick
```

---
## \#18 Posted by: skatardude10 Posted at: 2018-05-24T15:04:45.995Z Reads: 60

```
I shorted my charge port a few days ago. Just had to replace the port, everything else is fine. Hopefully this is also true in your case.
```

---
## \#19 Posted by: Acido Posted at: 2018-05-24T16:24:50.979Z Reads: 52

```
see if you get any voltage from your charger if not open up the battery and inspect from inside
```

---
## \#20 Posted by: Davideariel Posted at: 2018-10-30T12:35:55.425Z Reads: 38

```
I finally had time to check my e-board.
The charger doesn't output anything.

What are the specs of the charger? 
Because I now need to replace it, and I have some that might be compatible. (I'm going to change the plug since it was also fried)
```

---
## \#21 Posted by: Acido Posted at: 2018-10-30T13:25:23.618Z Reads: 31

```
The charger needs to be the same voltage as your battery

I think space cells are at 42v 
So a 42v 2A charger should do it
```

---
## \#22 Posted by: Davideariel Posted at: 2018-10-30T13:39:32.512Z Reads: 27

```
Is there any way I can check the voltage?
```

---
## \#23 Posted by: Holyman92 Posted at: 2018-10-30T13:40:02.427Z Reads: 27

```
Same thing happened to me a coyple days ago, i blew a comoonant on my bms...

Make a solution of 1:1 90%-100% isopropyl alcohol to 100% acetone and get a tooth brush and clean all ur electronic parts. While cleaning look for burn marks on all ur components... if the board turns on but isn't charging u only have the bms or charger to look at
```

---
## \#24 Posted by: Holyman92 Posted at: 2018-10-30T13:41:29.777Z Reads: 28

```
Connect a multimeter to the charger
```

---
## \#25 Posted by: Davideariel Posted at: 2018-10-30T13:45:08.172Z Reads: 27

```
I already checked and it's the charger which is fried, at least it looks like it since there is no output.
I was asking about the battery voltage, and I will use the multimeter.
The BMS looks fine and not burnt....
```

---
## \#26 Posted by: Holyman92 Posted at: 2018-10-30T13:46:00.518Z Reads: 24

```
Oh, just use a multimeter on the terminals the check the battery
```

---
## \#27 Posted by: Davideariel Posted at: 2018-10-30T14:14:59.721Z Reads: 22

```
The battery works, but should be there any sign of "life" on the charging cables? The ones which are connected to the plug.
```

---
## \#28 Posted by: Sn4pz Posted at: 2018-10-30T15:30:08.884Z Reads: 20

```
with the space cell, near the display if you press around it youll feel a small button click. Once you turn the board on and do this it should switch from percentage to voltage

![image|500x500](upload://hg2qNk5a6vQ7kNIjg8BMrN3NDsp.jpeg) 

press around the area pointed to by *Hassle Free esk8 Battery System*, the screen should switch modes
```

---
