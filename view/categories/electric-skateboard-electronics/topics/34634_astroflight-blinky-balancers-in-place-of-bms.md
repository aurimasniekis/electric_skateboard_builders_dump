# Astroflight blinky balancers in place of BMS

### Replies: 17 Views: 909

## \#1 Posted by: BigBoyToys Posted at: 2017-10-02T22:53:16.575Z Reads: 130

```
I saw a couple of references to these http://www.astroflight.com/106 by @Hummie and a few others, but Im wondering if any others have any experience with them. Im consodering leaving them attached to my batteries https://www.genstattu.com/tattu-9000mah-22-2v-6s1p-25c-lipo-battery-pack-with-na-plug.html and inside my enclousures then just bulk chargiing my lipo packs. Feel free to tell me how bad of an idea this is or otherwise, but I'll probably do it anyway unless you can convince me that it will definately blow up,  or that using BMS's that will add a bunch of wires, be bypassed for discharge anyway and that will take up more space that I dont have, are worth it.

Issues with implementing this idea that Ive consideered this far:

1. Each 6S lipo will need its own Blinky balancer (cost and space).
2. 9AH 6S lipo's are very large for these Blinky's to balance with only 150mA of balancing discharge current capabilty per cell (I will be removing the packs and checking cell balance after the 1st few charges and periodocally thereafter even if all seems to be well).
3. The Blinky's balance by dissipating heat, so laying them on top of my batteries will heat up my packs and the Blinky's some (I will place a small sheet of insulating material between the lipo packs and the Blinky's and could even use small heats sinks if needed). 
4. These may not have been designed to be left on the batteries during discharge(not sure what effect that might have other than them working extra hard trying to maintain balance as I drain the packs, Ive contacted the Astroflight engineers with this queation as well).
5. Ive seen some report of them overheating and not working until they are unplugged and plugged back in( this is my biggest concern, if it tends happen I can create small clear windows over the balancers to visualize the LED's on the Blinky's to ensure they are still functioning).

Reasons I think it may work and other benefits:

1. These 25C lipos will will never see above a 10C discharge rate and only a few seconds at a time at that. 
2. Im estimating that the lipos will be discharging at 2C for 95% of their life, so Im not expecting huge imbalances to begin with.
3. I will be charging 27Ah-36AH (depending on if I go 3P or 4P) of these packs at less than .3 C which will allow the Blinky's many hours to do their job while charging and also minimize the charging stress on the batteries.
4.  They are very high quality lipos by Gens Ace Tattu.
5. Having the battteries automatically discharge to storage voltage while not is use is a nice perk.

Please feel free to share thoughts and experiences.

Thanks,
 BBToys
```

---
## \#2 Posted by: Rinzler Posted at: 2017-10-02T23:18:06.617Z Reads: 105

```
Those are cool. There is something called a battery medic, i got it from hobbyking. It can discharge lipos while charging, and balance them. It is quite large, but it has a screen that shows you the voltages of each cell which gives me peace of mind. Here is the link: https://hobbyking.com/en_us/hobbykingtm-battery-medic-system-2s-6s.html?___store=en_us
Dont buy the knock offs from ebay, they have quality issues. Attached some photos, information is scarse on the hobbyking website.<img src="/uploads/db1493/original/3X/0/a/0a11a739b02d4767a91ba89a972e4b89e166b0ea.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/8/f/8f77c434ce52a191b9e7b78a2fad04ddd5a5f039.jpg" width="666" height="500">
```

---
## \#3 Posted by: BigBoyToys Posted at: 2017-10-02T23:23:48.241Z Reads: 91

```
Wow, those are very inexpensive as well.
```

---
## \#4 Posted by: Hummie Posted at: 2017-10-02T23:26:25.768Z Reads: 91

```
theres also a smaller discharge balancer...see if I can find it now..  cant find the one ones I use but this is very similar.    

they discharge very slowly but work.
I use them with a 500 watt meanwell power supply, so I can charge in like 30minutes all 12 cells and use one plug.  xt90s plug.

get two ofo these or even one is good
https://www.rcplanet.com/batteries/battery-maintenance/great-planes-electrifly-cellmatch-lipo-2-6s-balancer-meter-w-lcd-gpmm3210/?utm_source=bing&utm_medium=cpc&utm_campaign=BPA%20-%20Items&utm_term=4579740807623099&utm_content=BPA%20-%20Items
```

---
## \#5 Posted by: Rinzler Posted at: 2017-10-02T23:26:26.439Z Reads: 80

```
Yup, and they give me peace of mind while charging because of the screen, they are definitely worth the price :wink:
```

---
## \#6 Posted by: BigBoyToys Posted at: 2017-10-02T23:55:21.487Z Reads: 73

```
You think I can get away with 1 or 2 of these? Im running 6-8 separate 6S packs.
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-10-02T23:57:12.943Z Reads: 72

```
Hmm, if only I could find a place to put them
```

---
## \#8 Posted by: BigBoyToys Posted at: 2017-10-02T23:58:44.357Z Reads: 70

```
How do you limit the current draw on your Meanwell to prevent it from having a meltdown while charging?
```

---
## \#9 Posted by: Hummie Posted at: 2017-10-03T00:12:14.599Z Reads: 68

```
All the "switching power supplies"I've seen or used have a tiny screwdriver slot u can adjust the voltage. I also have always put a wattmeter in-line so I can see the current coming out and what voltage it's at. The current will come out based on the voltage u have it set to and if ur pack is at low voltage it will put out a lot of amps at first and then decrease as it gets closer to the voltage max as set by the screw slot. It's very worth adding a wattmeter in line. A wattsup brand is reliable vs others I've gotten.  I've also had a meanwell where I had to adjust the voltage w the screw in higher voltage increments  otherwise it would stutter and be really slow. But now that I have a higher power500 watt one, cheap from china, it's just plug n go. Lipos can take a lot of amps in and li-ion are pretty high too.   I've seen evidence cells decrease performance much more so from over charging than fast charging but there is a limit there. I set it to 4.10 per cell most often just to give some headroom in case. I almost always check every cell w one of those things quickly just as I start to charge.  Then I leave it dangling on the pack w the highest cell while charging.  I don't keep it on when riding.

I can use just one to check packs individually.  It doesn't have the failsafe a true balance charger has if a cell goes too high ( they should integrate an alarm and then it'd be great). But if ur aware of things and check I think it's safe.  I like checking incessantly anyway. Especially knowing the huge powe going in and the speed it's happening gets me on my toes.
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-10-03T01:22:04.807Z Reads: 61

```
I was looking at a 48V Meanwell PS recently rated for 12A (500W). If the battery pack is very large (36AH 12S) wouldnt there be concern that it would draw greter than 12A while the pack voltage is low and potentially damage the power supply?
```

---
## \#11 Posted by: Hummie Posted at: 2017-10-03T01:36:22.870Z Reads: 63

```
I don't know how they work really but I don't think that would happen.  The supplies should have an integrated safety limit.  I did break one once right away and they sent me another.  The addition of a wattmeter between the supply and battery seems essential to me
```

---
## \#12 Posted by: Cobber Posted at: 2017-10-03T02:26:51.411Z Reads: 58

```
what about getting a _plus_ version [with a built in bms]( https://www.genstattu.com/tattu-plus-10000mah-22-2v-25c-6s1p-lipo-smart-battery-pack-with-as150-xt150-plug.html)?

<img src="/uploads/db1493/original/3X/7/d/7d339d82e3c0001c1d6f5853026f973bc21ab27f.png" width="500" height="500">

are they any good?
```

---
## \#13 Posted by: BigBoyToys Posted at: 2017-10-03T03:09:57.156Z Reads: 54

```
Those are the best packs on the market imo, and would have been my 1st choice if their dimensions were better suited for our application. The packs I'm using are only 34mm thick which will allow me to mount them underneath thr deck.
```

---
## \#14 Posted by: Cobber Posted at: 2017-10-03T06:30:00.529Z Reads: 47

```
Tattu plus 22000mah 6s 25c...

<img src="/uploads/db1493/original/3X/1/6/16fe7c78aa67005a09b3ade31471981a26de81d6.png" width="97" height="97">

now I'm thinking about jumping ship :smiling_imp:
```

---
## \#15 Posted by: Cobber Posted at: 2017-10-03T09:47:22.013Z Reads: 43

```
@BigBoyToys, do you think the Tattu lipos can actually discharge at the claimed _C_ rate?
```

---
## \#16 Posted by: BigBoyToys Posted at: 2017-10-03T16:02:16.614Z Reads: 36

```
Yeah that particular pack had me rethinking my need to mount them underneath. Two of those of top of the board would be awesome! Im dead set mounting underneath so they are a no go for me unfortunately. I still wouldn't use lipos if I didnt need 400A's burst. Just not enough charge cycles imo. Maxamps lipos have a lifetime warranty though. If it fails after one year you get a replacement for 50% off MSRP. But no built in balancing on those.
```

---
## \#17 Posted by: BigBoyToys Posted at: 2017-10-03T17:09:57.306Z Reads: 33

```
[quote="Cobber, post:15, topic:34634"]
do you think the Tattu lipos can actually discharge at the claimed C rate?
[/quote]

I don't think it will actually. Im shooting for a max of 15c out of the rated 25C to minimize the sag and extend the life of the packs.
```

---
