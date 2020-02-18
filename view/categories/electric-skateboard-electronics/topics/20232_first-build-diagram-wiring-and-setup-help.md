# First Build Diagram, Wiring and Setup Help

### Replies: 22 Views: 1881

## \#1 Posted by: fmb Posted at: 2017-04-04T03:22:44.814Z Reads: 259

```
Hello! I am a high school student and this is my very first E-Board Build! I don't have experience building with electronics I was hoping to get some feedback and clarification about my build before I buy all the parts. I've done some research but I want to make sure that my setup is correct and that I have everything I need. Thanks in advance!

I am planning on making at Dual Rear Motor Setup. 

I have attached pictures 2 possible setups I am looking at and have linked all the parts I am planning on using below. If you have any better suggestion for parts please let me know. 

<img src="/uploads/db1493/original/3X/0/0/0089b2b1c128dd2b0cf57b530d074bf83ac32bca.JPG" width="375" height="500">

2 Motors - 6355 190KV diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/
2 VESC's - diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
1 CAN-BUS - diy-electric-skateboard-kits-parts/vesc-canbus-connector/
1 Male to Male Servo Connector - diy-electric-skateboard-kits-parts/male-male-servo-connector/
1 Dual XT90 Parallel Connector diy-electric-skateboard-kits-parts/dual-vesc-xt90-parallel-connector/
2 Batteries in Parallel - 4500mAh 10S 35C https://hobbyking.com/en_us/zippy-compact-4500mah-10s-35c-lipo-pack.html
OR
4 Batteries in Series and Parallel - 5000mAh 5S 25C https://hobbyking.com/en_us/zippy-compact-5000mah-5s-25c-lipo-pack.html
1 Charger - Depends on the battery selection. See question 2 below
1 Remote - https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html
1 Pair of Trucks - Unknown. See question 6 below
1 Set of Wheels - Undecided. Thinking http://www.ebay.com/itm/281661805302?var=580665315832
I am planning on using a 36t/15t set up with a 9mm belt from Enertion.

1. Do both my diagrams look correct?
2. Which setup would you recommend? It is my understanding that most LiPo chargers go up to 6S, so if I go with the 10S batteries I will need a more expensive charger. The thing is I don't know if it'll save me weight and space on the board to use the 10S batteries?
3. I have no experience with this, so I wanted to confirm that I am suppose to use a Dual XT90 Parallel Connector to connect the 2 VESC's to the batteries?
3. I was wondering how would I connect the 5.5mm bullet connectors on the batteries to the XT90 VESC connector? I was wondering is there was a plug for that? Also, since I am wiring the batteries in parallel as well, is there a plug that splits so I can connect them properly (If that made sense)?  I have a soldering iron but I am unfamiliar with it and don't want to mess around with that on my first build. 
5. I know this a totally noob question, but do I need a connector to connect the batteries together? Do the bullet connectors connect to themselves or will I need a connector to do that?
6. Since I am doing a dual rear motor setup I am worried about making sure that both motors will fit. I was wondering if you had any recommendations for trucks that would be able to fit my motors? I was thinking about these trucks as I have seen them fit on someone else's dual rear motor set up but I don't even know what size to go with that would for the motor. https://calibertruckco.com/collection/ Any recommendations would be really helpful. Also, I have access to a 3D printer at my school so I am going to be using the motor mount found here http://www.thingiverse.com/thing:1753981

Sorry for all the questions. I am just hoping to reduce the number of inevitable mistakes that I make on my first build. Thanks again in advance for all the help!

I'm also sorry if this has already been talked about in another thread. I was hoping to get some look directly at the setup that I am going to use.
```

---
## \#2 Posted by: willpark16 Posted at: 2017-04-04T03:36:28.985Z Reads: 191

```

I don't recommend lipos to teenagers, and yes I am aware they can be made safe but spending the extra cash on a safer li ion that doesn't need as much care is better

10s charger is about 110 you can get an iMac b6v2 tho and charge to 5s in parallel
So many questions so I just recommend to read more

Ur v2 drawing looks roughly right but hard to tell with the batteries, I'd recommend going single and spending the extra cash on ur battery and quality esc
```

---
## \#3 Posted by: fmb Posted at: 2017-04-04T13:18:39.696Z Reads: 171

```
Thanks for the help! I'll look into the li ion batteries. They're just more expensive than I was hoping

110 is too much for me so I think it'll go with the 5S in series and parallel

I've been trying to read more, but some of the questions I have are kinda specific. For example, would I use a Dual XT90 Parallel connector to connect the 2 VESC's to the batteries? Also, I have questions that are probably pretty obvious to an average person, like, do the 5mm bullet connectors connect to themselves or do I need a plug for that? and what plug would you use to connect the XT90 to the 5mm bullet connectors?
```

---
## \#4 Posted by: willpark16 Posted at: 2017-04-04T13:58:10.012Z Reads: 156

```
How much can u spend on batteries?
```

---
## \#5 Posted by: fmb Posted at: 2017-04-04T15:29:58.633Z Reads: 150

```
I really would not like to spend more than $150-$180

I also want to get good range (10 miles) as well as speed and torque since my area is full of hills
```

---
## \#6 Posted by: mmaner Posted at: 2017-04-04T15:35:46.556Z Reads: 150

```
If you have some freedom in your enclosure height @JLabs has a 10s3p/4p li-ion pack that I think will fit your budget.  Send him a message.  If you want lipos, look at hobbyking.com for the [5000mAh 2S 30C Lipo Pack](https://hobbyking.com/en_us/turnigy-5000mah-2s-30c-lipo-pack.html) and get 5 of them, wire them in series for a 10s pack and wire in a 10s BMS ([here](http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html) or [here](http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html)).  Cheaper than you think, comes out to $144.30 plus shipping.
```

---
## \#7 Posted by: willpark16 Posted at: 2017-04-04T15:37:45.609Z Reads: 144

```
lipos then 6s 8000 mah sould work just fine you will need 245kv tho for speed
or 10s 500mah lipo and 190kv
can u tell me ur whole budget?
```

---
## \#8 Posted by: lox897 Posted at: 2017-04-04T18:08:56.046Z Reads: 143

```
Do both my diagrams look correct?
Your VESCs need to be wired in parallel, your diagram shows they both go to the same side but both negative leads should go to the same terminal, and both positive should go to the same terminal. Wire your batteries in parallel first, not series. I can draw a diagram later if you'd like.

Which setup would you recommend? It is my understanding that most LiPo chargers go up to 6S, so if I go with the 10S batteries I will need a more expensive charger. The thing is I don't know if it'll save me weight and space on the board?
For a starting board, I'd go with 2x 5S batteries, although they are a bit thicker you will get more speed and range for the future. My first build had 6s and the range and speed wasn't great, although that was probably because of a KV decision.

I have no experience with this, so I wanted to confirm that I am suppose to use a Dual XT90 Parallel Connector to connect the 2 VESC's to the batteries?
Are you sure the VESCs have XT90? I haven't checked the page in a while but thought that most VESC had XT60. Yes you wire the two VESCS in parallel.

I was wondering how would I connect the 5.5mm bullet connectors on the batteries to the XT90 VESC connector? You will need a soldering iron or some adapters. If someone on the forum lives near you they might be able to help you with some soldering, otherwise have a go yourself and watch a few videos. Make sure your iron is adjustable temperature.

 I was wondering is there was a plug for that? 
You can use adapters

Also, since I am wiring the batteries in parallel as well, is there a plug that splits so I can connect them properly (If that made sense)?
Bullet connectors can connect together

Since I am doing a dual rear motor setup I am worried about making sure that both motors will fit. I was wondering if you had any recommendations for trucks that would be able to fit my motors? I was thinking about these trucks as I have seen them fit on someone else's dual rear motor set up but I don't even know what size to go with that would for the motor. https://calibertruckco.com/collection/ Any recommendations would be really helpful. 

If you have 2x 6355 motors, and Caliber 2 s you will be fine.

Also, I have access to a 3D printer at my school so I am going to be using the motor mount found here http://www.thingiverse.com/thing:1753981

I hope you have some strong filament 😂




Now onto your part choice:
I'd make a few changes so you can enjoy the build more. Firstly, you should get motors from electric-skateboard.market , may save some money there. Get the mini remote also from electric-skateboard.market , it's $30 right now and is much smaller than the GT2B (unless you plan to mod it).

Hope that helps!
```

---
## \#9 Posted by: fmb Posted at: 2017-04-04T20:53:05.126Z Reads: 118

```
Thank you so much for all of your help!! It really cleared a lot up for me!! I feel more confident now.

- _Your VESCs need to be wired in parallel, your diagram shows they both go to the same side but both negative leads should go to the same terminal, and both positive should go to the same terminal. Wire your batteries in parallel first, not series. I can draw a diagram later if you'd like._

If you could draw a diagram for wiring the batteries that would be great! Thanks so much for doing that!

- _For a starting board, I'd go with 2x 5S batteries, although they are a bit thicker you will get more speed and range for the future. My first build had 6s and the range and speed wasn't great, although that was probably because of a KV decision_.

I think I'll go with the 5S batteries then. I was wondering if you think getting 4x 5S batteries is overkill? (2 pairs in series connected in parallel)


Do you think for the XT90 to bullet connectors you could link some parts/adaptors? I was looking on HobbyKing but I can't seem to find them or I'm just not looking at the right ones. 

- _If you have 2x 6355 motors, and Caliber 2 s you will be fine._

I will probably go with the Caliber 2 but I was wondering as an alternative, do you think these will work as well? http://www.ebay.com/itm/Blank-Pro-180mm-Reverse-Kingpin-Longboard-Trucks-10-Axle-Black-/140892408040?hash=item20cdd788e8:g:vIUAAOSwnDZT9ikx


I think that the filament that we use is pretty strong. But I'm going to be using a 100% fill and I'll be printing a few just in case.

I will definitely look at the electric-skateboard.market. The prices seem better for me and that smaller remote looks seems like a better site for my hand.

Again, thank you for all of your help!! I really appreciate you taking your time to look at my build!!
```

---
## \#10 Posted by: fmb Posted at: 2017-04-04T22:26:27.278Z Reads: 101

```
I want to stay under 800
```

---
## \#11 Posted by: fmb Posted at: 2017-04-04T22:27:13.190Z Reads: 90

```
Thanks for the information! I'll look into that as well
```

---
## \#12 Posted by: lox897 Posted at: 2017-04-04T23:03:28.668Z Reads: 93

```
[quote="fmb, post:9, topic:20232"]
I think I'll go with the 5S batteries then. I was wondering if you think getting 4x 5S batteries is overkill? (2 pairs in series connected in parallel)

Do you think for the XT90 to bullet connectors you could link some parts/adaptors? I was looking on HobbyKing but I can't seem to find them or I'm just not looking at the right ones.
[/quote]

As long as you get 5s 5000mah at least, 4 of those is overkill. 10S is 37v nominal, 37v x 5ah = 185wh = 18.5km range. So if you went with 4 batteries you'd have 37km range.

Google XT90 to 5.5mm bullet connector or whatever your battery has connector wise. You may want to look on ebay as HK doesn't have lots of options for XT90.

NO, do NOT use those trucks, they don't have the right hanger for a mount
```

---
## \#13 Posted by: fmb Posted at: 2017-04-04T23:25:02.961Z Reads: 82

```
Thanks again for all the help!! I really appreciate you taking your time to clarify everything and look at my build!! It really helped!!
```

---
## \#14 Posted by: fmb Posted at: 2017-04-04T23:27:49.055Z Reads: 78

```
I just had one more question. Is an HXT 5.5mm bullet connector the same as just a 5.5mm bullet connector?
```

---
## \#15 Posted by: korryh Posted at: 2017-04-04T23:41:45.842Z Reads: 77

```
You may not want to use a 3D printed motor mount. I tried that at first and it failed on me coming down a hill and I had to jump off.  It was 100 percent fill abs but the plastic deformed and made the belt loose so it came off the pulley. 

Torque , enertion and I sell the mounts, they wouldn't be as free as your printed version but they won't leave you stranded or needing to test how fast you can run.
```

---
## \#16 Posted by: lox897 Posted at: 2017-04-04T23:49:23.486Z Reads: 64

```
No problem. Glad to help. I'm honestly not sure about the HXT question, I think it's just 5.5mm in a case yeah. I used them for a bit but they are quite bulky, then soldered on some XT60 and like it much more now.
```

---
## \#17 Posted by: fmb Posted at: 2017-04-05T00:08:09.113Z Reads: 66

```
Thanks for letting me know about the 3D printed mounts! I've been kind of worried about that.

It's probably not worth it to get the free mounts and have them break down. I'll look around to see if I can find some that aren't too out of my price range.
```

---
## \#18 Posted by: fmb Posted at: 2017-04-05T00:09:06.522Z Reads: 63

```
Thanks so much! I'll be doing extensive research on soldering
```

---
## \#19 Posted by: korryh Posted at: 2017-04-05T01:18:40.291Z Reads: 64

```
Since you may be buying motor mounts, check out @JLabs, he has nice motors and will help offset the mount cost.
```

---
## \#20 Posted by: korryh Posted at: 2017-04-05T01:26:57.826Z Reads: 74

```
Also @Titoxd10001 sells the wheel pulley kit and you can get 2 kits for about the price of 1 at most other vendors. I bought a couple and they are good quality and aluminum wheel gear and steel motor gear.
```

---
## \#21 Posted by: Customesk8 Posted at: 2018-12-08T04:35:47.306Z Reads: 15

```
can you get away without the bms here ?
```

---
## \#22 Posted by: mmaner Posted at: 2018-12-08T04:37:55.656Z Reads: 18

```
If you use a balance charger. But then you have to remove the batteries to charge or come up with a way to mount the balance leads. It would be better to just get a BMS in my opinion.
```

---
