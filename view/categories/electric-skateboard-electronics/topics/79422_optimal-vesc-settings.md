# Optimal Vesc settings

### Replies: 29 Views: 1205

## \#1 Posted by: Turboboard Posted at: 2018-12-30T20:13:52.663Z Reads: 246

```
Can anyone help me with my Flipsky ESC settings? Its based on the vesc, so i can use same tools to program it. I have dual Eskating 6374 190KV 3300w motors with a 10s battery. The vesc is rated for 150A continuous and 300A burst. I’m getting almost no torque at all with the default settings, (I can stop them in mid spin with my hand). I am using HTD5, 14t motor pulley and 72t wheel pulley and 200mm tires. My previous motors were 6374, 190kV, 1650w and had incredible torque and top-end, (50+km/h) and would take my heavy a, (200+lbs) up a 30°ish hill and I want to replicate or exceed that with these new motors and vesc.
```

---
## \#2 Posted by: StefanMe Posted at: 2018-12-30T20:18:03.679Z Reads: 243

```
show your settings... u must miss something.
```

---
## \#3 Posted by: Psmrman90 Posted at: 2018-12-30T20:34:20.270Z Reads: 234

```
Check out YouTube, there are a couple vesc setting tutorials thatll give some good guidance
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-30T20:47:06.613Z Reads: 228

```
Like @StefanMe said, could you post a screenshot of your actual settings from the vesc tool. Seems you miss something.
Do you have a link to the Flipsky esc?
Which battery you have? Lipo, LiIon and 1p or more. In case of LiIon it would be good also to know which cells you use to define the max discharge you can get out of them.
```

---
## \#5 Posted by: J_Dizzle Posted at: 2018-12-30T22:26:36.601Z Reads: 205

```
I believe @mmaner had some good setting for the fvesc
```

---
## \#6 Posted by: Turboboard Posted at: 2018-12-30T22:43:57.501Z Reads: 192

```
Any specific page or pages for screenshot?
```

---
## \#7 Posted by: skatardude10 Posted at: 2018-12-31T01:35:36.106Z Reads: 170

```
VESC Tool has a lot of settings, and it can seem daunting. The most critical things to make sure you do are 

1: run a proper motor detection (either BLDC or FOC), apply the detected values, and write motor config
2: set your battery max based off your battery accurately so you arent pushing more than your battery can handle. Write motor config.
3: map the remotes pulsewidth max, min, and center. Write app config.

This is about as basic as it can be for the things that really matter. Other important steps should not be glossed over though. Off the top of my head, battery configuration and safe cutoff voltages should be set. Motor max based off max amps your motors are capable of. Choose the right App mode, PPM most of the time, and setting the lost connection negative current, I like mine at 0 so that my board doesnt chuck me off if my remote loses connection for a bit.

Really, there are some good 20-45 minute tutorials on youtube that you need to watch. Watch a few of them before attempting anything. Then come back if things still arent clear. It will all make sense in time. Pretty much all vescs are the same to setup using VESC tool, minus the firmware you need to select and update to. Be aware, selecting the wrong HW version for your firmware can brick your vesc and make it difficult to recover.

To answer your question, things that can cause much lower power than expected: too low battery max, too low motor max, improperly mapped pulsewidths, maybe a bad motor detection or none performed at all? Those are the usual culprits ime.
```

---
## \#8 Posted by: mmaner Posted at: 2018-12-31T04:35:08.440Z Reads: 149

```
I would add...

Do a BLDC detection first, save and reboot. If everything is good, then do FOC detection. That will save you a lot of time if you have sensor or wireing issues.
```

---
## \#9 Posted by: Turboboard Posted at: 2018-12-31T05:29:33.295Z Reads: 139

```
Nothing seems to be working. I've done both BLDC and FOC detection on both motors, did the app wizard thing on the VESC Tool program. I guess the only thing I haven't tried is messing with the battery max and motor max but honestly that stuff makes me kinda nervous
```

---
## \#10 Posted by: Andy87 Posted at: 2018-12-31T05:34:54.398Z Reads: 139

```
It’s not that big deal.
You just need to know your vesc and battery limits and set the values after it.
Let us know which vesc you have and make a screen shot from the side of the max min values.
We still don’t know which battery you are rocking...
```

---
## \#11 Posted by: Turboboard Posted at: 2018-12-31T05:52:30.849Z Reads: 140

```
Here's the link for the vesc:
https://flipsky.net/collections/new-accessories/products/dual-fsesc4-20-100a-plus-based-on-vesc-with-anodized-aluminum-heatsink
```

---
## \#12 Posted by: Friskies Posted at: 2018-12-31T05:54:26.923Z Reads: 136

```
I wouldn't be caught running setting close to that at all.

In saying that we need to know the battery and type of cells that you are running. Without that we can't really help you
```

---
## \#13 Posted by: Turboboard Posted at: 2018-12-31T05:54:33.899Z Reads: 135

```
I don't know exactly what my battery specs are, (I bought it pre made) I only know its 10s4p
```

---
## \#14 Posted by: Friskies Posted at: 2018-12-31T05:55:12.914Z Reads: 126

```
Pretty hard to work out the correct battery settings for you without knowing the cell type
```

---
## \#15 Posted by: Turboboard Posted at: 2018-12-31T05:56:20.067Z Reads: 122

```
I "think" its 4.2v per cell?
```

---
## \#16 Posted by: Andy87 Posted at: 2018-12-31T05:57:07.491Z Reads: 122

```
Read through this
https://www.electric-skateboard.builders/t/flipsky-dual-fsesc4-20-info-review/71079?u=andy87
It explain the best settings for this esc.
This settings will just work if your battery can do that too.
Did you get it made from somebody here?
```

---
## \#17 Posted by: Andy87 Posted at: 2018-12-31T05:58:51.030Z Reads: 111

```
If it’s made out of 18650 cells than sure it’s 4.2v but we need to find out the max discharge of your cells. That’s usually not written and can only be found in the data sheet of the cell.
```

---
## \#18 Posted by: ARetardedPillow Posted at: 2018-12-31T06:00:02.461Z Reads: 110

```
Just show us your settings man
```

---
## \#19 Posted by: hoeksame1 Posted at: 2018-12-31T06:23:08.756Z Reads: 107

```
I personally would advice to not put high settings on the 4.2 vesc! 
Those thing wil warm up quickly. Also you need to do detection with your motor and remote etc.. if your torque isnt enough from dead start, you can also change your throtle mapping. This means you can decide how much percentage of extra power you want to give at the start. 
I had multiple kind of vescs.
Had problems with the flipsky 4.2..

I recommend to switch to either focbox/unity or flipsky dual 6.6.. I had 0 negatieve experience with those esc so far. 

You can read it and forget this or take my advice and be safer on the road :stuck_out_tongue:



Hoeksame
```

---
## \#20 Posted by: Turboboard Posted at: 2019-01-01T20:22:32.623Z Reads: 85

```
So some of you have been wanting me to send screenshots of my settings but I didn't want to take 20 screenshots so here is a video of my settings. I hope this helps. Sorry about the quality
[https://drive.google.com/file/d/1__qhIwiBWTjjC9QwqpLCGOX7r-OmXoRc/view?usp=drivesdk]
```

---
## \#21 Posted by: JensSjogren Posted at: 2019-01-01T20:45:16.713Z Reads: 73

```
Well i don't know if this is related to your torque problem but your voltage cutoff is way to low, cutoff start at 32v and end at 30-28v is what you want for your 10s pack. does your battery use a discharge BMS? otherwise you might have discharged your cells to low.
```

---
## \#22 Posted by: Turboboard Posted at: 2019-01-01T20:49:53.804Z Reads: 73

```
Thank you, I'll change the voltages. No, it doesn't use a BMS that I know of unless it's wrapped up in the battery pack.
```

---
## \#23 Posted by: JensSjogren Posted at: 2019-01-01T20:53:12.668Z Reads: 76

```
most likely it has a BMS if you bought it from a vendor, however it might be a charge only BMS and in that case it doesnt protect your pack when discharging, meaning that you rely on your ESC to cut of the battery before the cells voltage drops down to a critical level. 

where did you buy your pack?
```

---
## \#24 Posted by: Andy87 Posted at: 2019-01-01T20:54:01.071Z Reads: 76

```
I repost this
https://www.electric-skateboard.builders/t/flipsky-dual-fsesc4-20-info-review/71079?u=andy87
Please set your vesc up to the values mentioned there.
With 80a as batt Max your Flipsky 4.20 will cut out very soon or in worst case even overhead or fry the drv.
```

---
## \#25 Posted by: Turboboard Posted at: 2019-01-01T21:08:42.327Z Reads: 75

```
Should I keep the values at 60v?
And I bought my battery pack from China.
xSuperbProductions 31MPH Off Road Electric Skateboard – Motorized Mountain Longboard with Dual Motors - 11 Layers Canadian Maple, All-Terrain, 4 Wheels, Remote Controlled High Speed Board https://www.amazon.com/dp/B07K9LLLT6/ref=cm_sw_r_cp_apa_i_Vx9kCb3RRDB8Y

This is the original board. Now the only things that are still stock are the deck and the battery.
It was bought off alibaba not amazon but exactly the same
```

---
## \#26 Posted by: Andy87 Posted at: 2019-01-01T21:19:04.474Z Reads: 68

```
Which 60V?

If it was a pre build board you can guess there is a bms included in the pack (ok, you never know what you get from China) but it would be kind a risky to don’t include one.
If it’s a discharge bms you can have what ever esc you want and set values you want but if it’s over the current limit the bms can handle the bms will cut your power off.
```

---
## \#27 Posted by: Turboboard Posted at: 2019-01-01T21:32:23.309Z Reads: 66

```
Sorry, meant 60A. The default settings on the VESC tool are 60A motor max and 60A battery max. I have them both set at 80A.
Also, would it work to have 2 BMS's? (If I bought one and there's one inside the pack?
```

---
## \#28 Posted by: Turboboard Posted at: 2019-01-01T21:35:26.039Z Reads: 66

```
Thanks Andy87, I'll set my specs to the ones you used on your vesc
```

---
## \#29 Posted by: Andy87 Posted at: 2019-01-01T21:38:19.348Z Reads: 69

```
80a will not work 60a probably also not.
Please read the thread I linked.

Two bms will also not work.
You need to bypass the the one you have (if not bypassed already, but this we don’t know)
Or change the bms to a new one. That would only make sense if your cells can handle more.
If your bms fit to the output of your battery pack a new bms will also not help.
As you can see, as long as we don’t know what battery exactly it is (cells, bms etc), nobody can really recommend you anything.
```

---
