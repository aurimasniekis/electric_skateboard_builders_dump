# Low range on 12s4p battery

### Replies: 9 Views: 1243

## \#1 Posted by: crustyxpunk Posted at: 2017-09-15T08:47:21.082Z Reads: 227

```
So I've had my build up and running for about a week now and am a little concerned about my battery. I purchased most of my components from Torque Boards. I'm running their 6374 motor, vesc (now with 3.28 using the new tool), and their 12s4p lith ion pack. I figured I would be getting around 20-25 miles with the pack and so far I have been averaging around 14 miles. That's on Mostly flat ground with some hills and going about 20mph. Wheels are 83mm with 36/16 gears.  Here are my settings from BLDC tool that are the same in vesc tool. If there is something I can tweak to help with battery life let me know!

<img src="/uploads/db1493/original/3X/7/f/7ff1ab499fa69afea86ac71c6555829effacf30f.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/5/4/54654143deb87111b19408396a1888baa8d1d516.JPG" width="666" height="500">

The Torque Boards website also says the pack can typically be recharged with their 2A charger in 2-3 hours. I have not seen my battery charge that quickly. Typically takes 6 to 8 hours. Is this abnormal for the size battery I have? Thanks in advance for the help! I've read a lot of posts on this forum and have learned a lot but definitely still have a lot to learn!
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-09-15T11:23:22.850Z Reads: 206

```
Your cutoffs are too high. Change them to 36v start and 33.6 end instead of 43.2v and 39.6. Also the max input voltage should be 57v.
```

---
## \#3 Posted by: i2oadsweepei2 Posted at: 2017-09-15T11:27:51.939Z Reads: 202

```
Also forgot to mention that if the cells are 2500 mah in a 4p config then thats 10000mah total or 10 amps divided by the 2 amp charge rate is 5 hours to charge possibly longer for balancing. If you used the 4 amp charger it would charge in 2.5 hours.
```

---
## \#4 Posted by: crustyxpunk Posted at: 2017-09-15T11:36:08.293Z Reads: 198

```
Thank you! I'll make those changes and give them a shot. I remember watching one of the VESC tutorial videos and someone had the cut off at 50 for some reason, but I can't remember why lol. Also going to buy a quick charger soon. Thanks again!
```

---
## \#5 Posted by: i2oadsweepei2 Posted at: 2017-09-15T11:40:55.665Z Reads: 195

```
Your welcome. I think you need to be careful braking down any significant hills as well with a fresh fully charged battery. With 12s I think its easy to hit the overcurrent cutoff when there is no where for the regen to go. I always keep it in mind with my TB's 12s3p as well. You could also pull the plug early when charging at like 98% too if you live in a hilly area.
```

---
## \#6 Posted by: crustyxpunk Posted at: 2017-09-15T13:19:14.469Z Reads: 184

```
 I hadn't read that anywhere so that's really good to know, thanks! I'll definitely try and do that from now on. 

Do you know if there is a benefit to running sensered and also doing FOC or should I just try and run one or the other?
```

---
## \#7 Posted by: i2oadsweepei2 Posted at: 2017-09-15T14:53:42.191Z Reads: 168

```
Sensored is great for starting from a stand still. You need to kick push in almost all cases to get moving without sensored using vesc.

I can't explain foc to you but I am using it for 12s and 8s. I'm not using sensored foc yet until my new connectors come in. In foc you lose a little top end speed which I am happy to have gone. Coming off my board at 40kmh and hitting the grass last year luckily taught me that I have enough speed for now... 

Search for this ---> Vesc cut out downhill

Number 2 and 3 results talk about the over current thingy :)
```

---
## \#8 Posted by: i2oadsweepei2 Posted at: 2017-09-16T01:38:35.903Z Reads: 138

```
There is more chat [here](http://www.electric-skateboard.builders/t/focing-around-weak-brakes-and-cutout/33203) about the over current. It's all worth reading if you have time
```

---
## \#9 Posted by: crustyxpunk Posted at: 2017-09-16T01:58:08.346Z Reads: 130

```
Cool, just read that thread as well. I'll have to keep following it and see what they find out. Appears that there are always going to be trade offs between BLDC and FOC, at least for now. Thanks again for all of the input!
```

---
