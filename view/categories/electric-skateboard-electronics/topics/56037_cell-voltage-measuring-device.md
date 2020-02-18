# Cell voltage measuring device

### Replies: 27 Views: 950

## \#1 Posted by: ShakeNBake7000 Posted at: 2018-05-19T22:52:12.604Z Reads: 153

```
So I'm upgrading from a normal balance charger to a bms and since I won't use the Imax b6 charger anymore, I don't really have any way to check battery voltage, each cell's voltages, and basically anything about the batteries.
What device can I buy that will be on the cheaper side, that will be able to check voltages and whatever else may be needed?
nothing fancy. just needs to do the job and be reliable.
Thanks!
```

---
## \#2 Posted by: Hummie Posted at: 2018-05-19T23:01:30.610Z Reads: 153

```
U have multimeter?
```

---
## \#3 Posted by: b264 Posted at: 2018-05-19T23:03:46.876Z Reads: 147

```
The idea is that the BMS does all this and all you do is plug in a charger.  Just like if it's a laptop computer.

![pg-018__79022_zoom__27199_zoom|500x500](upload://rlPhmOMBYzZRdIC8tEWqyHBt8MR.jpg)

To answer your questions, there isn't really a device because it's not needed.  You can buy a [battery level indicator](https://www.ebay.com/itm/ACID-Lead-Battery-Capacity-Indicator-Charge-Level-LED-Tester-Voltmeter-12-48V/172988539709?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D1%26asc%3D20140725133649%26meid%3D30edbb6200894f8699bec18085d90667%26pid%3D100276%26rk%3D4%26rkt%3D4%26sd%3D311832992634%26itm%3D172988539709&_trksid=p2060778.c100276.m3476) but it's for the entire pack voltage, not the individual cell voltages.  Leave the charger plugged-in after it turns green and it will balance the cells.
```

---
## \#4 Posted by: ShakeNBake7000 Posted at: 2018-05-19T23:17:38.948Z Reads: 125

```
No, I was thinking of getting one, but I couldn't find one that can check cell voltages and I'm not sure it's even possible with a bms because the Balance wires are already connected to the bms.
```

---
## \#5 Posted by: ShakeNBake7000 Posted at: 2018-05-19T23:19:06.846Z Reads: 124

```
I know how a bms works, but I still need to be able to check the battery's voltage once in a while, which voltmeter can you recommend for that?
Edit: just saw the link, I already have one of those, but only precentage and not volts. Whats the difference between that small indicator and a full size meter though?
```

---
## \#6 Posted by: b264 Posted at: 2018-05-19T23:24:28.200Z Reads: 121

```
If you push the button, it toggles between percentage and volts.  There is another button inside, you hold that before you turn it on, then push the front button until it says L10 (lithium metal, 10 series) and then install it.  After that the front panel button toggles between percentage and volts
```

---
## \#7 Posted by: Hummie Posted at: 2018-05-20T00:57:09.399Z Reads: 113

```
to get individual voltages I think a multimeter is the usual way.  you couldn't get true individual cell voltages since you likely have some paralleled but you can get the whole parallel group
```

---
## \#8 Posted by: mynamesmatt Posted at: 2018-05-20T02:00:53.254Z Reads: 104

```
I have this:
https://hobbyking.com/en_us/battery-monitor-2-6s.html

You just plug it into the balance connector of your battery and thats it. It shows the total voltage, and each individual cells voltage
Hope this helps :smile:
```

---
## \#9 Posted by: TowerCrisis Posted at: 2018-05-20T03:52:56.454Z Reads: 97

```
All cells in a parallel group will be the same voltage.
```

---
## \#10 Posted by: Hummie Posted at: 2018-05-20T03:56:41.415Z Reads: 95

```
that's what I'm saying
```

---
## \#11 Posted by: TowerCrisis Posted at: 2018-05-20T03:58:19.983Z Reads: 87

```
I'm saying that the true individual cell voltage will be the same. If you disconnect a parallel pack and measure each one, it will always read out the same voltage assuming they've been connected for any reasonable amount of time.
```

---
## \#12 Posted by: Hummie Posted at: 2018-05-20T03:58:47.035Z Reads: 84

```
yea.  I know a paralleled cell will have the same voltage but at that point, measuring a cell that's paralleled, its' voltage isn't telling you much.  I guess what I mean by "true" is it's "useful" voltage as what its voltage reveals about its' capacity or state of health
```

---
## \#13 Posted by: TowerCrisis Posted at: 2018-05-20T04:00:13.772Z Reads: 85

```
[quote="Hummie, post:7, topic:56037"]
you couldn’t get true individual cell voltages since you likely have some paralleled
[/quote]

🤷‍♂️ 10 char
```

---
## \#14 Posted by: ShakeNBake7000 Posted at: 2018-05-20T07:16:14.447Z Reads: 76

```
Yeah so I can check the total and divide that by the number of cells, but the reason I need individual cells voltages is that sometimes the battery doesn't completely balance the cells, once I had a 0.15v lower in one cell than the rest, and I just want to make sure that doesn't happen again.
```

---
## \#15 Posted by: ShakeNBake7000 Posted at: 2018-05-20T07:17:00.527Z Reads: 74

```
When using a bms, the ballance cables are soldered to the chip, so i have no access to them.
Thanks though!
Edit: and connected without the actual port, only the cables.
```

---
## \#16 Posted by: b264 Posted at: 2018-05-20T07:35:52.834Z Reads: 68

```
When you use a BMS, it specifically avoids the cells being unbalanced.  That's what a BMS does.... that's why nobody has a ready-made solution for what you want.  It's not needed.  You can make it yourself, no problem though...

If you have experience with batteries that don't have a BMS, like hobby lipos, then that may be why you've seen them unbalanced.  You can even use a BMS with those as well if you want.
```

---
## \#17 Posted by: ShakeNBake7000 Posted at: 2018-05-20T07:38:30.608Z Reads: 69

```
[quote="b264, post:16, topic:56037"]
When you use a BMS, it specifically avoids the cells being unbalanced.  That’s what a BMS does
[/quote]
Yeah but isn't a balance charger supposed to do the same?

[quote="b264, post:16, topic:56037"]
If you have experience with batteries that don’t have a BMS, like hobby lipos, then that may be why you’ve seen them unbalanced.  You can even use a BMS with those as well if you want.
[/quote]
The batteries I will soon use with a bms are lipos yeah, hoping the bms will balance them better than the Imax b6
```

---
## \#18 Posted by: b264 Posted at: 2018-05-20T07:42:59.175Z Reads: 60

```
A balance charger will do that, yeah -- if you instruct it to.  I used an imax B6 once and didn't realize it was getting unbalanced because I kept putting it on "charge" mode.  You have to use "balance" mode at least every few times.
```

---
## \#19 Posted by: Okami Posted at: 2018-05-20T08:11:38.306Z Reads: 60

```
Ive looked into this and u are after is cell meter, i think.

Go on banggood or aliexpress, theres quite a few options
```

---
## \#20 Posted by: ShakeNBake7000 Posted at: 2018-05-20T08:13:24.594Z Reads: 58

```
I was using balance mode, 5 amps.
```

---
## \#21 Posted by: ShakeNBake7000 Posted at: 2018-05-20T08:14:37.251Z Reads: 57

```
Problem is, the balance cable is already connected to the bms, so i cant connect it to the cell reader.
```

---
## \#22 Posted by: Okami Posted at: 2018-05-20T08:21:17.940Z Reads: 58

```
U need parallel adapter / cable for that.

Also it should stay turned on only when charging or when using the board, as these meters tend to suck down first two cells over longer period of time, if u leave it switched on.

I made a seperate thread about these meters a while ago.

In my experience, if cells are healthy they should stay in line with each other. If they are lipo, then yes more monitoring is advised, as they tend to drift a lot more than 18650 and other li ions.

One more extra note. Usually u can only plug up to 8s in one cell meter. So for 10s u would need 2. Though i suspect u have 6s, since u mentioned b6 charger

---
http://www.electric-skateboard.builders/t/ways-to-tell-you-should-start-to-think-about-going-home-voltage-monitoring/15912/40

Similar to that one can be bought for about 10usd, ISdt one costs about 20usd but is better / more sophisticated in my opinion
```

---
## \#23 Posted by: ShakeNBake7000 Posted at: 2018-05-20T08:37:09.087Z Reads: 52

```
Yeah, I do have 6s, two 3s's in series, thank you for all the information I will look into it.
```

---
## \#24 Posted by: philvanzu Posted at: 2018-05-20T09:05:41.874Z Reads: 55

```
you could always combine a 6 way rotary switch with a cheap lcd panel voltmeter, or get one of those fancy bms's with BT monitoring
```

---
## \#25 Posted by: mynamesmatt Posted at: 2018-05-20T09:07:47.884Z Reads: 54

```
Buy some 6s extensions (or whatever size your battery is) and put the voltage checker in parallel. won't draw much current and will show the right voltage. That's what I'm doing for my board
```

---
## \#26 Posted by: Randyc1 Posted at: 2018-05-21T04:13:55.321Z Reads: 46

```
![20160510_121133-800x450|690x388](upload://dJbHEfLYlEVLN3SdzVd3rVl3cJb.jpg)
```

---
## \#27 Posted by: mynamesmatt Posted at: 2018-05-21T09:15:00.232Z Reads: 39

```
@Randyc1 how did you connect your pulley to your SK3 considering they have a round pinion? DM me
```

---
