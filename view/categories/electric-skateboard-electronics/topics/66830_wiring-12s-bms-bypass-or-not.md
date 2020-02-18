# Wiring 12s bms bypass or not

### Replies: 17 Views: 627

## \#1 Posted by: 12meterkuk Posted at: 2018-09-02T12:08:52.323Z Reads: 146

```
![image|690x422](upload://z25f89rbx0MTVkugioZv1odhE8J.jpeg)

This is the bms I have, how do I wire it for bypass? It only has p- and b- 

It’s rated for 40amps should I bypass or not? I’m using turnigy lipo 4s 5ah 20c x3 in series so I should get about 100a at most
```

---
## \#2 Posted by: Jake2k17 Posted at: 2018-09-02T23:39:39.895Z Reads: 127

```
If you have a Vesc there is not reason to discharge through bms. As for the wiring, attach a wire coming from your negative lead to the b- port, and your negative charge wire to the p- port. Good luck building!
```

---
## \#3 Posted by: dareno Posted at: 2018-09-03T00:55:57.015Z Reads: 120

```
Yeah that bms at 40 amps is a discharge bottle neck.  The VESC actually does a stand up job balancing on discharge.  It’s witch craft to me but I have a 10s 3p with a blown bms that I have been running without now for a couple of months and every now and again test the p packs to check and all show the same voltage.  If you’re going to run 12s make sure the bms if wired for discharge can handle it or it will take control and either pop or shut down the board.  No fun at all. you have to also consider over voltage with regenerative braking.  Full charge downhill braking will shut down the battery if wired for discharge.  KSSS.
```

---
## \#4 Posted by: thisguyhere Posted at: 2018-09-03T01:00:04.812Z Reads: 116

```
https://www.electric-skateboard.builders/t/warhorse-2-custom-hollow-core-integrated-build/53428/13
```

---
## \#5 Posted by: 12meterkuk Posted at: 2018-09-03T06:03:32.854Z Reads: 105

```
Thanks guys!
```

---
## \#6 Posted by: Acido Posted at: 2018-09-03T09:23:19.801Z Reads: 99

```
Yes there is, the only reason people do not use discharge bmss is because of their side
You loose a lot of protection when you bypass
```

---
## \#7 Posted by: Namasaki Posted at: 2018-09-04T05:55:33.528Z Reads: 85

```
[quote="dareno, post:3, topic:66830"]
The VESC actually does a stand up job balancing on discharge.
[/quote]

If your battery stays balanced without a bms, it is because your battery's cells are well matched in terms of capacity and internal resistance so that they charge and discharge evenly. 

The Vesc has nothing to do with it.
```

---
## \#8 Posted by: dareno Posted at: 2018-09-04T07:30:36.315Z Reads: 79

```
Like I said its witch craft to me  Thanks for that.  Got to say though I must be pretty lucky considering the battery in question is a cheap and nasty item.  Could you elaborate please?  I was under the wrong impression and I don't like that. :neutral_face:
```

---
## \#9 Posted by: Namasaki Posted at: 2018-09-04T11:59:57.474Z Reads: 74

```
The Vesc only monitors the voltage at its input and initially cuts back power before shutting down when that voltage reaches the low voltage values set in the Vesc tool or BLDC tool. 

A BMS (battery management system) monitors the voltage of each cell or cell group and trims the cells with higher voltage to match cells with lower voltage to balance the pack.
```

---
## \#10 Posted by: dareno Posted at: 2018-09-04T18:04:36.025Z Reads: 75

```
Thanks man, I understood that because of the low voltage cut off the battery stays even across the cells.
Goes to show don't believe everything you see on you tube.  In your opinion is it better to have the bms wired for discharge then?
```

---
## \#11 Posted by: Namasaki Posted at: 2018-09-04T21:48:32.019Z Reads: 72

```
Discharging vs bypassing.
There are many different opinions on this topic.
I guess they both have their pros and cons.
For example, discharging through a quality bms protects against over discharging, short circuits and over charging by regen braking.
Some have reported problems with their brakes when discharging through a bms and some have reported less power output when discharging through a bms. You have to make sure that your regen current does not exceed the max charge current of the bms and that the bms has adequate cooling.

I am currently discharging through the bms on my builds and have had no problems with my brakes even when braking constantly down hill on a full battery.

I can't tell if I'm loosing any power output because I have not tried bypassing to see.
For me, having more power is not necessary so the extra protection is of more value to me.

So whether it is better to bypass discharge or not is really up to the individual.

The only thing that I would strongly recommend is to buy a quality name brand bms for either type of setup.
And of course a high amp bms for discharge or a low amp bms for bypass.

Bestech and Supower are good brands though I prefer the Bestech because of the built in E-switch, FET heat sinks and higher balancing current.
```

---
## \#12 Posted by: dareno Posted at: 2018-09-04T23:31:35.257Z Reads: 67

```
Great info thanks,  I am running a 12s bestech atm wired for discharge and haven't really had a chance to try it out properly but one thing I did notice was it gets pretty hot when charging but the cells stay cool.  Does it dissipate heat from the cells also because batteries usually warm up a bit while charging.
```

---
## \#13 Posted by: Namasaki Posted at: 2018-09-05T02:10:24.443Z Reads: 64

```
The bms won't dissipate heat from the battery. It will only dissipate it's own heat.
The Bestech has heatsinks to dissipate heat from it's FET's.
It also has over temp protection with a sensor attached to the heat sinks.
It will shut down if it gets too hot.
This is one reason I like to mount the bms separately and not packaged with the battery. The more it is open to air the better it will dissipate heat. Mine is inside an enclosure but with ample room around it and it has never overheated.
![JPG|375x500](upload://yXlwL2g81uwBRq8aKiwEpA1glX3.jpeg)
```

---
## \#14 Posted by: Wraith Posted at: 2018-09-05T02:12:58.131Z Reads: 58

```
Do you have a separate enclosure for them BMS as well? kind of like the enclosures produced for the DieBieMS? I realized just now that it may actually heat up more if kept in those enclosures
```

---
## \#15 Posted by: Namasaki Posted at: 2018-09-05T02:20:57.387Z Reads: 57

```
I have one enclosure that covers everything.
![jpg|375x500](upload://kfH9URMFnPuVa7uzkHzcJBCjGPf.jpeg)
```

---
## \#16 Posted by: Wraith Posted at: 2018-09-05T02:23:34.266Z Reads: 53

```
That looks sooo clean really well done! So I should be fine without those separate 3d printed BMS cases? It would save me some space as well if It wouldn't make a difference in wirebulk or heat generation on the bms
```

---
## \#17 Posted by: dareno Posted at: 2018-09-05T03:21:13.118Z Reads: 55

```
can we move in together?:rofl:
Thats the same as my unit but mines 12s  bloody great thing.  I was actually thinking that very same thing when i felt the heat it produces.  Needs space for that to escape.  I'll pull it away from the battery and make it comfortable.  Those are graphenes aren't they?   You have been seduced by the dark side.
```

---
