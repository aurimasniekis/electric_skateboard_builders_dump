# First Build - Daily Driver - Still Looking for Suggestions

### Replies: 4 Views: 792

## \#1 Posted by: plainpat Posted at: 2017-11-19T17:12:31.749Z Reads: 91

```
Hey everyone,

I'm looking to convert an old longboard I have into a dual drive build.  It seems dual rear is most common but I've also wondered if dual-diagonal might be more efficient.  I'm planning to use this for my commute to and from school which is about 4 miles and includes a few decent hills, I have a hard time estimating grade but I'd imagine no more than 15-20%.  Including my backpack, I'll weigh at most 210-220 pounds.  However to be safe I'd like something that could hopefully get up to 10 mile range (if that's realistic), since I think building a board suited to harsher conditions than I'll actually put it through will make sure it is effective and lasts.  I've put a bit of thought into some components to buy but looking for suggestions on what people prefer/what is possible in a dual drive setup.  Additionally, since I'll be using it in the northeast US and winter is around the corner, I don't expect that I'll be able to use it for a few months.  This is nice because it allows me to space out buying my parts between now and then which should make cost somewhat less of an issue.

The deck is a 3ft Land Yatchz with 180mm trucks and 2ft wheelbase.  I'm thinking about upgrading to these 90mm 78a Bigfoot wheels (https://www.amazon.com/dp/B0057IWIG4/ref=pd_rhf_se_p_img_6?_encoding=UTF8&psc=1&refRID=MJZ1ZPVKAQP77KDQ81YC) and probably getting some new bearings/bushings since the current ones are a bit old.

<img src="/uploads/db1493/original/3X/5/5/556b459ea4e9ffdb53d061129b1188f2998d6993.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/8/28369b8fb62ef9033b2e528a2726153cb1d41f26.JPG" width="375" height="500">

I'm thinking 2x Turnigy SK3 6364 213kV for the motors (https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html?___store=en_us) but was wondering if these would have trouble fitting in the dual rear configuration.  Also thought about getting Tacon Bigfoot 5335 245kV's instead but if anyone has suggestions on other motors that might be better please let me know, I'm not sure if I should be going for something with lower kV like a 190.

I'm probably going to buy a pair of the ABEC 36T Pulley kits from DIY (collections/electric-skateboard-pulley-belt-combo-kits/products/36t-abec-pulley-combo-kit)

As far as ESC and batteries I'm a little less certain on what to do and hoping I could get some input from you all here.  I'm planning to go for a VESC but there's a lot of confusing information out there on them.  I've seen that you can spend quite a bit of money here but I'm not sure if I need to go much higher than the $100-150 range.  Is this Torqueboards 12S 120A VESC good enough?  collections/esc-speed-controller/products/torqueboards-12s-120a-car-esc-opto-hv  Does anyone have experience with this one or recommendations for others.  I'm also a little unsure of how 2 VESCs would be wired together, is there some kind of master/slave configuration?  And would I also be able to track stats with this like distances, motor outputs, etc like I've seen some people are able to do?

For batteries I think 6S for each motor would be okay to start and shouldn't overheat anything but could/should I go up to 8 or 10S?  What about adding cells in parallel?  I'm not entirely clear on how parallel batteries change motor output/battery range.

For some of the other things like motor mounts and possibly the housing I have access to some 3D printers and metal machining tools at school that I hope to be able to make some parts in order to cut cost down a bit too.

So anyway, this is kind of my starting point for now.  I'd appreciate any feedback you guys can provide and I look forward to starting to build this soon!
```

---
## \#2 Posted by: Decdog Posted at: 2017-11-20T00:23:10.973Z Reads: 57

```
That ESC that you linked is not a VESC. Here’s their VESC: collections/featured-items/products/torque-esc-vesc-bldc-electronic-speed-controller
```

---
## \#3 Posted by: plainpat Posted at: 2017-11-23T04:51:27.089Z Reads: 35

```
Understood, my mistake.  Knowing this now, would you recommend that one or are significant advantages offered by another that are worth considering?

Thanks!
```

---
## \#4 Posted by: wafflejock Posted at: 2017-11-23T07:18:24.884Z Reads: 33

```
The VESC is mostly better with regard to the ability to configure and expand on the open source and open hardware platform.  One straightforward example is the low voltage cut off which you can set a start and end point for with the VESC through their application and using a USB connection (most proprietary ESCs require programming through voodoo using your controller or special programming cards).  VESC is also more configurable when it comes to specific adjustments in amperage for braking or accelerating and erpm which ultimately allows you to more finely control the ride feel (also multiple control modes like current control or watt control with ackmaniacs version of the vesc firmware).  Speaking of that without using a modified firmware you can also get modules like the one from http://metr.at and the corresponding app to log data on the VESC while using it (this is pretty atypical of a run of the mill ESC).

---

Down sides with the VESC would say you can get hit or miss on errors with the DRV chip or other components causing the DRV chip to fry or use too high a voltage and kv motor combination (above 60k erpm is a problem on older VESCs like the 4.12 hardware, apparently not an issue on the latest VESC6 hardware but also about 2-3 times more expensive).  Search the forum for DRV8302 or drvfault to see some of the cases where things have gone wrong, also FOC mode notoriously caused problems especially for newer users who aren't familiar with diagnosing and fixing problems (BLDC mode is generally safer/simpler but not quite as smooth).  Personally have only had issues with the DRV chip through faults of my own but it does seem to be quite touchy.

---

Conclusion, regular ESC not easy to program or change configuration typically, however likely more of a plug and play experience.  VESC easy to change configuration, but requires you to do so to get it working in the first place and not damage any components.

http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
