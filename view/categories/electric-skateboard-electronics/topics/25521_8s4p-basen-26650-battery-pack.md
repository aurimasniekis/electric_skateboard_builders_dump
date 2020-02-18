# 8s4p Basen 26650 Battery Pack

### Replies: 18 Views: 1111

## \#1 Posted by: sprocket12 Posted at: 2017-06-16T19:00:35.162Z Reads: 172

```
So, I've graduated from my 2 x Zippy 4s1p 8000 mAh (8s1p) Lipos.  I've ordered my Basen 26650's from Liion Wholesales.  I've ordered enough to make an 8s4p pack.

The Zippy's gave me plenty of torque and speed (~27 mph top speed) but the distance wasn't far enough (~12 miles) and I eventually started getting a puffy pack and my distance on full charge started dropping. An 8s setup seems fine for me.  Yes, I understand I should get a pretty insane distance on the Basen 8s4p pack.

I have a no-longer-called-a-VESC controller dialed in for 8s voltages on the Lipos and have a few questions.

1) I've read just too much on voltage limits and am second guessing myself.  These batteries are the 60A 4500 mAh Flattop.  I know they are more like 30A continuous.  But what are good cutoff values for them in volts for the controller?  Lipo Battery cutoff is set to start at 3.6V and battery cutoff end at 3.2 V?  For this battery configuration???

2) I also bought these to last.  I've read the pros/cons on using a BMS.  It seems that BesTech is the one to use if I do.  Which one? Thoughts?

I was going to solder BMS leads either way.  This would allow me to check each battery individually and charge/balance if needed.  I'd really rather have it set for plug-n-play on charging if possible.

I also purchased a coulometer to keep an eye on the actual mAh and voltage so I don't abuse things too much ;)

So can you provide any insights, tips, or guru direction?

Thanks guys!
```

---
## \#2 Posted by: BigBoyToys Posted at: 2017-06-16T19:19:45.701Z Reads: 156

```
I read like 23A Continuous on those cells
```

---
## \#3 Posted by: Smorto Posted at: 2017-06-16T19:21:31.808Z Reads: 153

```
I think the reason your range is decreasing is because your voltage cutoff is too low IMO. I think you should never run lips lower then 3.4ish volts in order to extend their life. 

A **conservative** cutoff voltage for an 8s lion pack could be 3.4 and 3.0 which is 27.2 and 24 volts.
You probably could go a little lower but in order to extend the life cycle of your pack I think these values could work for you.

As for BMS both BesTech and Supower/battery supports should work fine.

Anyone who knows more or knows something i said is wrong please feel free to add more or correct me.


PS. I know you mentioned it but your pack is going to be a whopping **518WH** assuming they actually are 4500mah per cell. Assuming 10wh per km thats a **32 mile range**! Should be fun :slight_smile:.
```

---
## \#4 Posted by: sprocket12 Posted at: 2017-06-16T19:30:32.941Z Reads: 136

```
Good to know. So I should be fine with 70A continuous and a burst of 160A.

I have been limiting my amp draw to ~40A in the VESC for battery max. My absolute max is set to 130A. I think I should be fine there too.
```

---
## \#5 Posted by: sprocket12 Posted at: 2017-06-16T19:33:14.393Z Reads: 125

```
Ok @Smorto. With such a large pack I figure the drain will be minimal so I'll look at lower cutoff values. 

And yes, the ride should be a blast. Distance and longevity are my reasons to upgrade.
```

---
## \#6 Posted by: Smorto Posted at: 2017-06-16T19:36:19.283Z Reads: 122

```
Awesome I have been looking at cells and saw these and they looked like a good compact cell so Im looking forward to seeing the battery built and hope you plan on making a build log.
```

---
## \#7 Posted by: sprocket12 Posted at: 2017-06-16T19:50:49.276Z Reads: 115

```
Plan to.

I really want to get this as simple as possible regarding the charging/maintaining. I have multiple 4s chargers and a standard 33.6 'smart' charger.

I'd really like feedback on using a BMS. I don't need one with a switch, I have all that. I just need one for charging/balancing.  Does anyone have specific model suggestions?
```

---
## \#8 Posted by: Smorto Posted at: 2017-06-16T19:59:28.710Z Reads: 112

```
I would just recommend an 8s BMS from Batterysupports but I have little to no knowledge about BMSs so I am not the right person to help you with that.
```

---
## \#9 Posted by: sprocket12 Posted at: 2017-06-16T22:52:26.978Z Reads: 107

```
Do I miss out on anything by using a BMS like this from HobbyKing?

https://hobbyking.com/en_us/8s-li-ion-pcm-charge-4a-discharge-10a.html

I was thinking of using it solely to charge the batteries.  Correct me if I'm wrong please, but I thought the 10A limit discharge is if I use the BMS to monitor/restrict the output from the cells.  Do I need to use a BMS that way?  Or can I use the BS to balance/charge and just use the +/- from the pack to my VESC?

This one I read that I run my power through it to the VESC and keep it to 60A.

http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html
```

---
## \#10 Posted by: Smorto Posted at: 2017-06-16T23:33:10.124Z Reads: 96

```
If you use the BMS for discharge as well you get all the discharge protection features listed on the page of the battery supports BMS. You can bypass it simply for charging in which case you can use a low A BMS like the hobby king one but you lose those features.
```

---
## \#11 Posted by: wmj259 Posted at: 2017-06-17T02:44:07.508Z Reads: 89

```
I have my lipos set to 3.6v cutoff, but I have my lipo alarms set to 3.7v. That way I don't have the hassle of recharging the lipos back to storage 3.7v from 3.4v
```

---
## \#12 Posted by: Smorto Posted at: 2017-06-17T14:06:18.459Z Reads: 77

```
This is for lipos though, lion packs can be discharges much lower.
```

---
## \#13 Posted by: wmj259 Posted at: 2017-06-17T15:54:28.887Z Reads: 78

```
Yes that is true,.
```

---
## \#14 Posted by: Glenn Posted at: 2017-06-18T00:54:06.704Z Reads: 63

```
I have 2 of my builds without bms and haven't had a single problem. Of coarse I use all the same batteries(lg he2's) and use a lithium ion smart charger. My first build is going on 2 yrs.
```

---
## \#15 Posted by: sprocket12 Posted at: 2017-06-18T12:48:32.060Z Reads: 54

```
Do you ever balance your cells?  If so, how?
```

---
## \#16 Posted by: Glenn Posted at: 2017-06-18T20:42:08.639Z Reads: 47

```
No but ran bms wires for future on one of my builds. But even at that I  only can charge 3 batteries at a time with the bms so your not really making it that much better. I have a 8s X 3p. So to do it right you would have to have 24 wire leads coming out  of your battery pack not including your main charging leads. In a perfect world you would charge each cell individually.
```

---
## \#17 Posted by: sprocket12 Posted at: 2017-06-19T15:35:38.543Z Reads: 43

```
So I've been reading other posts on the batteries. Can anyone chime in on the voltage lag mentioned?

The pack I'm building is an 8s4p. I've used Lipos in the past with the same 8s setup. The amps were 120. My new pack should be 100-120 amps at 16,000 to 18,000 mAh's. The voltage is the same (3.7 x 8 = 29.6 or 4.2 x 8 = 33.6). 

What's the lag? I've tried to really over build this pack for uninterrupted riding and would appreciate any advice. Should I go with higher voltage?  Say 10s4p?
```

---
## \#18 Posted by: BigBoyToys Posted at: 2017-06-20T01:48:19.126Z Reads: 40

```
Voltage sag occurs when u draw more amps from the battery pack than it can discharge without its voltage dropping. Sagging voltages also mean reduced range, hotter battery cells, less life cycles etc.
```

---
