# No BMS needed for charging

### Replies: 12 Views: 568

## \#1 Posted by: DeathByBacon Posted at: 2018-05-19T06:58:18.788Z Reads: 139

```
I've seen some builds not needing to use a BMS for charging their 18650 battery packs given that they rarely drift if taken care of properly. Does the same thing apply to LiPos?
```

---
## \#2 Posted by: MysticalDork Posted at: 2018-05-19T07:03:31.973Z Reads: 139

```
Under no circumstances should you run a lipo pack without some form of balancing, either in the form of a BMS or a balance charger. That's just asking for a fire.

I wouldn't even charge a 18650 pack without balancing, the consequences of failure are simply too high.
```

---
## \#3 Posted by: rojitor Posted at: 2018-05-19T09:12:41.606Z Reads: 123

```
Only very stable chemistry cells can be used without bms. Sony konion and Tesla for example. But even like that a bms is needed for hvc lvc.
MD is right, under no circumstance Skip balance on lipo. Fire hazard!
```

---
## \#4 Posted by: aigenic Posted at: 2018-05-19T10:16:24.256Z Reads: 105

```
I heard Lifepo4 cells could be used without balancing, but it is not recommended...Can somebody confirm that?
```

---
## \#5 Posted by: Acido Posted at: 2018-05-19T10:28:22.945Z Reads: 99

```
maybe if you draw like 0.1A from your battery you wont need balancing
but if you draw 40-100A like we do its totally needed
its like 30$ why cheap out on a part that protects your 200$+ battery
```

---
## \#6 Posted by: Eboosted Posted at: 2018-05-20T04:09:54.301Z Reads: 61

```
I've been runing my 12s4p daily for 3 months, no BMS at all, charging up to 50v and discharging once in a while to 36v, most of the days I just go down from 100% to 70% and charge. 

Yesterday I opened the enclosure and find out the cells are exactly as I left them when I started the build, no. Drifting at all.
```

---
## \#7 Posted by: neverpush Posted at: 2018-05-20T05:20:32.073Z Reads: 52

```
Only joking, but didn't one of your boards catch on fire @Eboosted?
```

---
## \#8 Posted by: mynamesmatt Posted at: 2018-05-20T05:20:53.431Z Reads: 50

```
I think he means drifting voltages bud?
@Eboosted
```

---
## \#9 Posted by: neverpush Posted at: 2018-05-20T05:22:00.518Z Reads: 49

```
I was referring to the @MysticalDork 's concerns of fire hazards.  @mynamesmatt
```

---
## \#10 Posted by: b264 Posted at: 2018-05-20T05:23:41.074Z Reads: 49

```
ANY of these batteries can be charged without balancing.  A FEW TIMES.  They need to be balanced at least every few charges.  There is little to no harm running it a time or two without balance.

Now if you misread what I wrote as "I think I can probably run it 25 more times because he said a few was okay" then you will have a fire eventually.

If you need to go through the effort to balance it all the time, you might as well just build the balancing into the charge procedure -- which typically means using a BMS.
```

---
## \#11 Posted by: mynamesmatt Posted at: 2018-05-20T05:38:52.044Z Reads: 42

```
 @neverpush i was referring to eboosted talking about cells drifting in his enclosure but you guys mean drifting voltages....right?
```

---
## \#12 Posted by: neverpush Posted at: 2018-05-20T05:55:42.112Z Reads: 42

```
That is correct.
```

---
