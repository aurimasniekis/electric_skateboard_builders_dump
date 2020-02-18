# What&rsquo;s a decent Battery &amp; Power for my Motor (first build)

### Replies: 22 Views: 2493

## \#1 Posted by: streamrash Posted at: 2016-07-22T13:32:46.530Z Reads: 155

```
Hi Guys,

Getting around the second time to try to build a custom e-board. Last time I got so frustrated finding parts that ended up getting an Yuneec E-Go, then a month after got a single motor boosted which I love. I still own both, but it's time to go back and build one with no hurry. This should be fun....

I have one of each motor, will only be using one of them:
6374 190KV
6355 190KV

I read [this awesome article](http://www.electric-skateboard.builders/t/what-is-battery-c-rating-is-it-important-for-electric-skateboards/36?source_topic_id=215) @onloop which help me understand more batteries prior to posting this, still I don't understand which battery i need to purchase for my motor, for the example 6355. I'd like to achieve decent speed (not more than 25mph) and distance other than torque. I know these motors are torqui. I'll be using a basic 1/8 scale ESC 120a (HobbyWing EZRUN-WP-SC8).

I plan to use a series connector which I think will allow me to have two thinner batteries below the deck instead of a huge thick one. Again, I could be completely wrong, I don't know much.

Looking to order batteries from Amazon, they have so many.

Thank you much for all your help.
```

---
## \#2 Posted by: anorak234 Posted at: 2016-07-22T13:40:18.353Z Reads: 143

```
So for your type of motors, I'd say anywhere from 8s to 12s will work. The ESC is your problem. Double check the specs: your ESC only takes up to 4 lipo cells
```

---
## \#3 Posted by: streamrash Posted at: 2016-07-22T13:46:38.722Z Reads: 138

```
@anorak234 thanks for that! I almost bought that ESC. Do you think 6S will do the job as well (maybe)? 2 x 3S batteries in series?
```

---
## \#4 Posted by: onloop Posted at: 2016-07-22T13:58:38.094Z Reads: 138

```
i would use vesc for esk8 these days. 

i recommend @chaka or Enertionboards for the best quality. both made in the US to high standards.

the best battery would be a custom made 18650 setup, minimum 10S3P configuration.


think about how you will charge & how you will switch on/off your system.
```

---
## \#5 Posted by: quanze Posted at: 2016-07-22T14:39:20.504Z Reads: 130

```
Or diyelectric. They got good stuff too
```

---
## \#6 Posted by: anorak234 Posted at: 2016-07-22T14:43:36.746Z Reads: 124

```
2 x 3s is exactly what I used with a 190Kv SK3. Top speed theoretically should be around 20mph but I've gotten it up to 25. It's got great torque.
```

---
## \#7 Posted by: streamrash Posted at: 2016-07-22T15:13:22.397Z Reads: 116

```
Awesome! Just ordered a decent ESC that will support up to 6S. I really don't wan't more than 25mph. Any particular 3S battery you prefer @anorak234?  mAh & cells?
```

---
## \#8 Posted by: anorak234 Posted at: 2016-07-22T15:17:24.140Z Reads: 112

```
Honestly go with a 6s2p lion if possible. I use 2 Zippy 3s 5000Mah lipo batteries but have had to get several more since initial buying because they failed so easily. I've spent 150 bucks now on 25$ batteries. I know @link5505 and @barajabali make 6s2p as I am currently looking into buying batteries from either of them
```

---
## \#9 Posted by: Lizardking0069 Posted at: 2016-07-22T15:20:12.222Z Reads: 111

```
I would recommend  @torqueboards for any first build.
If you are in the US they are very fast on delivery and have very good  customer service. Their stuff is pretty reliable.
```

---
## \#10 Posted by: streamrash Posted at: 2016-08-11T18:26:07.281Z Reads: 96

```
**Update on the Build**

I ended up putting 2 x Turnigy 5000mAh 3S 20C Lipo Packs series on a 150amp HobbyWing EZRUN running 6S. Motor 6374 190KV.

Problems:

* _Speed_ - It's maximum speed is currently around 16mph. I think I have is that the 190kv needs more like 8S-10S to function properly and to go faster. Maybe adding a better discharge rating (C) battery packs will help?

* _No Regenerative Brake_ - The ESC has three settings for running mode. (1) Fwd / Brake. (2) Fwd/ Reverse with Brake. (3) Fwd and Reverse. I've tried all of them and the braking is not great. The motor also makes a weird sound when hitting brake/reverse.

Maybe **VESC** is the solution to most of these issues.

Gear ratio I currently have is:

**Motor:** 15 tooth
**Wheel:** 36 tooth
**Belt:** 9mm Pitch Width

@anorak234 did you do something different to attain 20mph+? 

<img src="/uploads/db1493/original/2X/c/c5113602a8e2f41060eacf5c56d11117bf3be279.png" width="435" height="499">

<img src="/uploads/db1493/original/2X/6/6e017c69551d13ffcf7edb62e2ed82a928b210f6.jpg" width="375" height="500">
```

---
## \#11 Posted by: anorak234 Posted at: 2016-08-11T18:55:45.217Z Reads: 80

```
Idk exactly what I did, I'm usually on flat ground. 16/36 ratio, 2 X 20C 3s lipos in series. Got the SK3 192kv motor, 90mm wheels. Biggest difference in mine from most is weight. I weigh 140lbs, my board is around 20. That esk8 calculator thing also wasn't accurate for me, I'm assuming that it uses a fixed value for 'weighted' top speed
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-11T19:01:44.647Z Reads: 81

```
The calculator measures distance values based on the input variables. If you do the math manually it checks out. If you're getting higher speeds than what the calculator says, then one or more of the fields is inaccurate, or you're gaining speed form another source such as a downhill. Perhaps you have a higher KV motor than what's printed on it, or perhaps it's a different pulley. It could be a number of things.
```

---
## \#13 Posted by: streamrash Posted at: 2016-08-11T19:25:06.573Z Reads: 77

```
Yeah, I'm 200 pounds, kinda heavy. You do have larger wheels than my setup. I a set of Orangatang Kegel 80mm 80a.
```

---
## \#14 Posted by: streamrash Posted at: 2016-08-11T19:31:10.548Z Reads: 78

```
@Jinra @anorak234 check this out. that calculator is really incredibly accurate, wow, totally impressed. 

<img src="/uploads/db1493/original/2X/4/4cb9a000d3f0554c4adc3db4681cb23e567ebd52.jpg" width="685" height="500">
```

---
## \#15 Posted by: Jinra Posted at: 2016-08-11T19:33:08.033Z Reads: 72

```
Yep! If all specs are accurate on the parts themselves and you overcome resistance such as hills, wind, rough roads, weight, etc to reach peak effiency you should be getting close the top speed on the calculator.
```

---
## \#16 Posted by: Jinra Posted at: 2016-08-11T19:33:53.191Z Reads: 70

```
I noticed you put 15T for motor pulley, but you said 17T on your earlier post.
```

---
## \#17 Posted by: streamrash Posted at: 2016-08-11T19:36:00.559Z Reads: 66

```
Ops. I fixed the previous post thanks. It's 15T
```

---
## \#18 Posted by: streamrash Posted at: 2016-08-11T19:39:27.716Z Reads: 68

```
@Jinra i ordered two motor pulleys to try out. One 20T and a 24T. Theoretically If I increment the tooth on motor, it should increase speed. The calculator says that by adding 5 more tooth it will increase 5-6 mph. No idea.
```

---
## \#19 Posted by: Jinra Posted at: 2016-08-11T19:40:53.841Z Reads: 68

```
Running with a reduction that low on 6s will lead to an early death in your ESC and/or motor. You generally don't want to go under 2:1 ratio. 2.5:1 and higher is better for 6s
```

---
## \#20 Posted by: streamrash Posted at: 2016-08-11T19:41:47.436Z Reads: 66

```
Thanks, I won't do it then.
```

---
## \#21 Posted by: Jinra Posted at: 2016-08-11T19:46:38.531Z Reads: 64

```
If you want more speed, I suggest you get a higher KV motor or upgrade your ESC to a VESC and run 10s
```

---
## \#22 Posted by: NewbieBoardBuilder Posted at: 2016-12-19T05:56:57.023Z Reads: 37

```
What app did you use for that top photo?
```

---
