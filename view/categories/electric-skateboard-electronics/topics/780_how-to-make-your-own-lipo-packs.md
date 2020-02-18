# How to make your own lipo packs?

### Replies: 13 Views: 7328

## \#1 Posted by: evoheyax Posted at: 2015-12-22T16:21:32.310Z Reads: 249

```
Does anyone know of any guides on how to make your own lipo packs from single cells with balancing cables? I saw one about how to make a 3s lipo from cells, but he didn't put any balancing cables.

Basically, I need to make a 12s battery from cells, so I can keep the battery pack thin.

My understanding is that I should put the cells in series (- to +), with a balance cable coming from each + tab of each cell. Can someone confirm this is correct?

And I read from googling around that I can charge the 12s as if it where 2x 6s batteries, allowing me to still use my 6s charger. Can anyone elaborate on what needs to be done to make this possible?

Any help with these questions or point me in the right direction is appreciated.

Just an FYI, I was planning on using these cells:
http://www.hobbyking.com/hobbyking/store/__18562__Turnigy_5000mAh_1S_40C_Lipoly_Single_Cell_.html

Also, does anyone have any advice on how to properly use a battery meter like this?
http://www.ebay.com/itm/LCD-Capacity-Tester-Indicator-For-12V-48V-Lead-acid-Lithium-Cell-LiPo-Battery-/261660579850?hash=item3cec2f980a:g:qF8AAOSwKrxUZFYy

the max amps are very low, and when my board is running, the amps will be much higher than it can take, so I'm confused as to how I could use a battery meter like this.
```

---
## \#2 Posted by: scoobiext Posted at: 2015-12-24T01:36:02.348Z Reads: 224

```
G'day Evoheyax

Making custom LiPo packs is difficult and dangerous and shouldn't really be attempted with out a bit of electrical know-how.  There is a lot of information around on how to do this if you want to proceed though (check the RC forums and Endless Sphere).

If you wanted to use assembled 3S packs to make a 12s pack the easiest way would be to series them up with connectors (similar to this http://www.hobbyking.com/hobbyking/store/__7181__T_Plug_Battery_Harness_14AWG_for_3_Packs_in_Series.html ) as you say from +ve to -ve,   To charge the pack I would then unplug them and charge each 3S pack individually. This way you no not need to worry about extra balance wires and soldering or welding the individual packs.

Charging a 12S pack with a 6S charger will not work, you could series two 6V chargers to get the required output voltage but balancing between the packs would be an issue.

The reason the battery meter works is that it is a volt meter, and volt meters have very close to infinite resistance (i.e. no current flows across the device).  The current quoted in the specifications is the small amount of current required to power the device and not the current your board would be using.

Hope this helps.
```

---
## \#3 Posted by: barajabali Posted at: 2015-12-25T16:47:59.209Z Reads: 202

```
Merry Christmas!

I agree Scoobie, it's very dangerous unless you know something about lipo pack. I've made all of my lipo packs from scratch but only up to 6s. But if I were to create a 12s lipo I would do it the same way -/+ , + gets the balance lead. BUT I'd just invest in a 12s charger.
```

---
## \#4 Posted by: mccloed Posted at: 2015-12-27T05:22:21.183Z Reads: 193

```
I have built many battery packs from the single cells you mentioned. It is not very difficult. Although, I have only built up to 8s. I usually build in the balance plugs to charge as two 3s batteries(for 6s packs) or two 4s batteries(for 8s packs). If I built a 12s pack I would build it to charge as two 6s batteries, unless I was going to use a BMS and a laptop style charger.
```

---
## \#5 Posted by: lowGuido Posted at: 2015-12-27T06:20:43.683Z Reads: 184

```
@mccloed so when you charge do you use 2 chargers at the same time?
```

---
## \#6 Posted by: mccloed Posted at: 2015-12-27T16:34:40.468Z Reads: 177

```
I do. I just use two balance chargers. Like these: http://www.hobbyking.com/hobbyking/store/__21044__Hobbyking_174_DC_4S_Balance_Charger_Cell_Checker_30w_2s_4s.html
for 2 x 3s

And these: http://www.amazon.com/Tenergy-1s-4s-3-7-14-8v-Balance-Charger/dp/B00S1Q0UAA
for 2 x 4s
```

---
## \#7 Posted by: evoheyax Posted at: 2015-12-27T18:07:42.934Z Reads: 174

```
So for a 6s, you charge it like its 2x 3s batteries with two 3s chargers, without disconnecting the series setup?
```

---
## \#8 Posted by: mccloed Posted at: 2015-12-28T02:55:56.769Z Reads: 168

```
Correct. I leave the balance leads outside the enclosure so the batteries do not have to be removed.
```

---
## \#9 Posted by: flywithgriff Posted at: 2017-08-06T03:22:24.780Z Reads: 81

```
@mccloed I know this is a long ago thread but I am interested in it. I currently have 10x 2s 5ah 30c packs. They are wired in two sets of five in series and then the two sets in parallel and managed by a BMS. However, each 2s pack is a hard case pack and much to large when combined. How would I go about disassembling the packs and making the layout smaller?
```

---
## \#10 Posted by: SilentException Posted at: 2017-08-06T13:57:50.374Z Reads: 61

```
It's easy to disassemble any Li-Po pack, just need to take it slow and controlled, do not rush or push/pull anything with much force. Do it on a glass or ceramic table in case of any fire. Few weeks back one of my 4s packs had a puffy and very bad cell so I took it apart and now running 7s :slight_smile: 

You will need a beefy soldering iron, preferably 100W, some sort of cut pliers, a solvent and a credit card type plastic. Last two you need to separate 1s packs because they are glued together, some more than others. Just make sure you don't pull them apart because it will ruin the cell.

For putting it back together, you'll need double sided tape for gluing the cells and a plastic shrink wrap, if you want to wrap it. Also, some 22AWG silicone wire for balance lead and 12/10AWG for discharge.

Honestly it is not that hard, it just takes time. In your case, be careful when opening the hard case as well. You don't want anything to drill or cut into the cells inside, you're gonna have a bad time.
```

---
## \#11 Posted by: flywithgriff Posted at: 2017-08-06T14:10:45.574Z Reads: 54

```
I will be setting everything up on a 10s BMS for charging and balancing.

As I don't have any large shrink wrap would electrical taping the pack be ok?
```

---
## \#12 Posted by: SilentException Posted at: 2017-08-06T14:22:13.554Z Reads: 54

```
Kapton tape would be better.
```

---
## \#13 Posted by: flywithgriff Posted at: 2017-08-06T17:43:25.411Z Reads: 47

```
I know the answer to this question is subjective but anyone know about how thick these 2s packs will be after removing the case? Is it definitely worth removing them?
```

---
