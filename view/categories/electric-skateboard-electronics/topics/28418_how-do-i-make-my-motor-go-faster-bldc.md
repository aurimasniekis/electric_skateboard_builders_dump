# How do I make my motor go faster (BLDC)

### Replies: 36 Views: 2237

## \#1 Posted by: nikolas Posted at: 2017-07-24T00:47:39.408Z Reads: 275

```
Hi, I have a [6355 190KV Motor] (diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/), two 5000 mah 3s1p 20c Lipo Batteries and a [Vesc 4.12](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/). I found that my motor has been going slower than usual. 

Here are my BLDC Tool Screenshots:<img src="/uploads/db1493/original/3X/8/0/80f48f2dec2135a6569a356d3dd566b1c1a97657.PNG" width="690" height="406"><img src="/uploads/db1493/original/3X/a/f/afdcb4d032288531375d0d81ca1ed300918b69bb.PNG" width="690" height="408"><img src="/uploads/db1493/original/3X/f/3/f373a2a46ed0c5a85e3533cac4c10a3183f41541.PNG" width="690" height="406"><img src="/uploads/db1493/original/3X/1/4/14352b2be977351a85214f9237c7a0d567def35d.PNG" width="690" height="409">

Thank you in advance!! 

@Blasto @darkkevind
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-24T00:51:59.113Z Reads: 250

```
190kv is a bit low for 6s. I'd upgrade to 10-12s or throw another 3s lipo in there for 9s. You can change gearing for more speed, but right now your setup isn't the most efficient. 

Also, run and apply motor detection, it's at default right now.
```

---
## \#3 Posted by: nikolas Posted at: 2017-07-24T01:12:26.450Z Reads: 248

```
Thanks for the quick response! So what batteries should I get... Including mah, cellls and c. Also, should I change anything in my settings besides motor detection? Thanks again!
```

---
## \#4 Posted by: jammin Posted at: 2017-07-24T01:16:06.433Z Reads: 244

```
Buy the same 5000 mAh 3s 20c lipo, preferably from the same manufacturer. Run all of them in series to get a total of 9s1p (5000mAh).
```

---
## \#5 Posted by: nikolas Posted at: 2017-07-24T01:27:49.113Z Reads: 232

```
Unfortunately, I do not have enough room in my box.
```

---
## \#6 Posted by: jammin Posted at: 2017-07-24T01:31:00.098Z Reads: 219

```
Welp, not much you can do then, unless you wanna make / find another enclosure.

But @Jinra is right; 190kv is not optimal for 6s. When running through a speed calc, are your speeds close, or is it something else?
http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html
```

---
## \#7 Posted by: darkkevind Posted at: 2017-07-24T13:46:38.635Z Reads: 195

```
What is the max AMP rating of your motor?
```

---
## \#8 Posted by: jmasta Posted at: 2017-07-24T13:53:40.709Z Reads: 186

```
Here are all your options for increasing speed:

* Get a larger motor pulley, or
* Buy bigger wheels, or
* Make/find a smaller wheel pulley, or
* Buy a higher KV motor (up ~330kV), or
* Increase system voltage, or
* Add jet packs
```

---
## \#9 Posted by: Challlsss Posted at: 2017-07-24T13:55:45.369Z Reads: 183

```
<img src="/uploads/db1493/original/3X/e/5/e564903ac9ec320459d92e94d1ad6930382ab47a.gif" width="400" height="225">
```

---
## \#10 Posted by: MrHappy Posted at: 2017-07-24T14:07:57.036Z Reads: 179

```
I could see collin furze making a rocket powered longboard.
```

---
## \#11 Posted by: adseguy Posted at: 2017-07-24T15:55:45.225Z Reads: 165

```
I know someone with a new 6355 260kV motor that is looking for a 190kV that you have.  If you are interested in a swap, let me know.  That will fix your problem instantly
```

---
## \#12 Posted by: TJBoards Posted at: 2017-07-24T16:21:26.068Z Reads: 162

```
You say you want to go faster. How fast are you going on your current setup? I am running 2x3s 5000mAh 30s batteries on a 6355 190kv motor. 16Tx36T on Orangatang Kegel wheels. Yesterday I went 9 miles on a charge, averaged 13.7 mph and maxed at 18.5 mph. Elevation gain was 111 ft.
```

---
## \#13 Posted by: nikolas Posted at: 2017-07-25T23:24:57.775Z Reads: 142

```
Sorry for the late response. My max AMP rating is 80 AMPS
```

---
## \#14 Posted by: nikolas Posted at: 2017-07-25T23:26:28.339Z Reads: 139

```
When I started, I could easily be going 20 - 25 mph, now I am only going 10 - 15 mph.
```

---
## \#15 Posted by: nikolas Posted at: 2017-07-25T23:27:38.052Z Reads: 132

```
If I am correct, lower kv rating is higher torque so I would like to maintain my torque and increase my speed.
```

---
## \#16 Posted by: nikolas Posted at: 2017-07-26T00:06:40.631Z Reads: 127

```
If I were to buy another 5000 mah 3s 20c lipo battery, is there anyway that I can connect it without using a HXT 4mm Series Connector with 12awg Wire?
```

---
## \#17 Posted by: oldguy Posted at: 2017-07-26T00:19:29.487Z Reads: 130

```
I'm no electrical D.C. Motor expert, but I'd caution you about the lower kv / higher torque assumption. There are extensive threads about it already. I have a 260kv and more torque than I need. Adding the extra 3s to go to 9s is a solid suggestion. Get creative and make the room if you can.

More importantly, if your board used to run at twice the speed, and you haven't changed anything in your setup, then you have problem to investigate. Just adding more power is akin to turning up the radio when your car starts to make a knocking sound.
```

---
## \#18 Posted by: Alanhunt123 Posted at: 2017-07-26T00:28:56.823Z Reads: 124

```
I'd take a good look at your batteries. You say that you had performance and are now losing it. Perhaps your cells might be getting a little tired, and sag their voltage under current now. Are you experiencing a drop in range?

I used some cheap lipos for my first build from hobbyking. I was also using a vesc, a 4.12 from Enertion. The batteries were great when I first bought them, the board had a lot of punch. After a good amount of cycles, the performance dropped significantly, both acceleration and range. Built a new pack and had my performance back. 

Best of luck!
```

---
## \#19 Posted by: darkkevind Posted at: 2017-07-26T06:37:09.771Z Reads: 115

```
I'd up your motor max to 75A
```

---
## \#20 Posted by: TarzanHBK Posted at: 2017-07-26T08:17:47.101Z Reads: 110

```
People often run their lipos too low.
Charge them to 4.2V per cell and discharge them to 3.5V. 
If you run them lower over time, you´ll damage them.

I also had bad experience with low C rating lipos. 6S with 20C 5000mah sucks pretty hard on hills and sag a lot.
```

---
## \#21 Posted by: Tuomalar Posted at: 2017-07-26T08:54:55.247Z Reads: 104

```
[quote="nikolas, post:14, topic:28418"]
I am only going 10 - 15 mph
[/quote]


Yep, your battery is probably ''broken''. I don't se any other reason why this would happen.

And i don't get how you managed to get that 20-25mph. What is your gearing? You can't get that speed even with 100mm wheels.
```

---
## \#22 Posted by: TJBoards Posted at: 2017-07-26T12:14:53.111Z Reads: 105

```
[quote="Tuomalar, post:21, topic:28418, full:true"]
[quote="nikolas, post:14, topic:28418"]
I am only going 10 - 15 mph
[/quote]


Yep, your battery is probably ''broken''. I don't se any other reason why this would happen.

And i don't get how you managed to get that 20-25mph. What is your gearing? You can't get that speed even with 100mm wheels.
[/quote]

I don't understand either how you were able to get 20-25 out of a 2x3s 190kv motor. The max I've been able to get out of that configuration is 17.5 and I think I was going downhill. 

<img src="/uploads/db1493/original/3X/8/2/823dd50a573f1418edc5947d9dbc0485d3d87119.PNG" width="281" height="499"><img src="/uploads/db1493/original/3X/d/4/d452f72e0bc50831a60aa185e3a2cf7e0308dbd4.PNG" width="281" height="499">
```

---
## \#23 Posted by: nikolas Posted at: 2017-07-28T05:40:06.123Z Reads: 89

```
@TJBoards

I think that there were many factors that added up.

1. My board is new

2. I am riding on new roads

3. I think my gearing set up is pretty good
```

---
## \#24 Posted by: Tuomalar Posted at: 2017-07-28T07:40:44.154Z Reads: 86

```
What is your gearing?  New board or good roads doesn't explain this.
```

---
## \#25 Posted by: nikolas Posted at: 2017-08-02T18:53:46.465Z Reads: 87

```
36 Teeth on my Wheel Pulley and 16 on my motor. I would also like to add that I am only 100lbs if that makes a difference.
```

---
## \#26 Posted by: nikolas Posted at: 2017-08-02T18:57:16.725Z Reads: 87

```
Hi, Sorry for the late response... My 190kv is very scratched up on the outside. Let me know if he/she is still interested.
```

---
## \#27 Posted by: TJBoards Posted at: 2017-08-08T12:48:58.998Z Reads: 85

```
[quote="nikolas, post:25, topic:28418, full:true"]
36 Teeth on my Wheel Pulley and 16 on my motor. I would also like to add that I am only 100lbs if that makes a difference.
[/quote]

My daughter is only 90 lbs. and her board has the same exact setup as mine now and she doesn't go any faster on her board than mine. We both have a top speed of 21.7 mph. 6s lipo battery, 16/36 gearing, 6355 260kv single motor.
```

---
## \#28 Posted by: longhairedboy Posted at: 2017-08-08T20:00:44.324Z Reads: 74

```
I saw this a couple of weeks ago and i've been racking my head trying to come up with a solution.. but then last night it came to me in a fit of delirium like so many brilliant ideas do. 

I'm pretty sure this will resolve your issue. I would only use this for short bursts, and at the end you might notice a startling end to the boost but this is extremely efficient. Almost no additional battery power is used and you'll dramatically increase your motor RPMs. 

<img src="/uploads/db1493/original/3X/c/5/c54aafeb053fb752c22ae34a0b25b0389694ea66.png" width="500" height="500">

You may need to adjust the belt length and of course the distance between pulleys, and you may need some additional room around the motor can, but i'm positive this is exactly what you're looking for.
```

---
## \#29 Posted by: Jinra Posted at: 2017-08-08T20:11:57.144Z Reads: 69

```
who needs brakes!
```

---
## \#30 Posted by: ChrisChaput Posted at: 2017-08-08T23:47:41.109Z Reads: 66

```
I'm tired of belts and pulleys and hub motors. See you at the Performance Days bitches!

<img src="/uploads/db1493/original/3X/e/b/ebf61e685c467d2c6185853aa23f1c88eb9e2dd7.jpg" width="690" height="385">
```

---
## \#31 Posted by: Jinra Posted at: 2017-08-08T23:48:39.295Z Reads: 65

```
It's all fun and games until someone loses their leg to a jet turbine.
```

---
## \#32 Posted by: longhairedboy Posted at: 2017-08-09T11:47:17.807Z Reads: 63

```
dude i can't wait to pit my moon traveller mod against your jet turbine mod. I'm pretty sure the moon travelers are going to smoke you.
```

---
## \#33 Posted by: Nstroh Posted at: 2018-05-26T04:14:25.761Z Reads: 44

```
Hi, I need help with my board, I have a dual n5055 270kv 3000w dual belt drive setup with 3 3s 5mah 20c lipo batteries in series and it’s 15t-35t and I just don’t get enough speed, my single hub motor skateboards goes faster, what can I do. 83mm wheels and a cheap ESC off eBay. If you have suggestions can you add a link please, thanks. Also how do I post question so in other places, I’m new.
```

---
## \#34 Posted by: Nstroh Posted at: 2018-05-26T04:56:05.496Z Reads: 45

```
Hi, I need help with my board, I have a dual n5055 270kv 3000w dual belt drive setup with 3 3s 5mah 20c lipo batteries in series and it’s 15t-35t and I just don’t get enough speed, my single hub motor skateboards goes faster, what can I do. 83mm wheels and a cheap ESC off eBay. If you have suggestions can you add a link please, thanks. Also how do I post question so in other places, I’m new.
![image|500x500](upload://rdeXKmbQavOsj5Hxy5oZpdkSEyP.jpeg)
```

---
## \#35 Posted by: TarzanHBK Posted at: 2018-06-11T10:29:52.706Z Reads: 38

```
might be that you got the wrong ESC. These are available for 6 and 10s i think and for Hubs or Beltdrive. Each is different.
You might have a HUB ESC for 10s, so you are below that with 9s and it might also be that yours is for Hubs only.
```

---
## \#36 Posted by: carwyn987 Posted at: 2018-06-25T02:09:55.338Z Reads: 28

```
lmao 5mah??!! i think you meant 5000mah or 5 amp hours
```

---
