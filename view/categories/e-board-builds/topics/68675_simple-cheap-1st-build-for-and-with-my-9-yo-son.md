# Simple, cheap, 1st build for and with my 9 yo son

### Replies: 56 Views: 1318

## \#1 Posted by: owlen Posted at: 2018-09-20T20:19:57.640Z Reads: 282

```
Hi all, 

As I wrote in my [intro](https://www.electric-skateboard.builders/t/new-member-introduce-yourself-here-tell-us-your-plan/216/1394?u=owlen) I would like to build something basic for (and with) my son. 
I have a technical background, I can solder reasonably well, and know my way around a drill. Here are the requirements, some questions, and my initial thoughts. 

### Requirements
* **Slow**: Cause I hate writing "safe". 10mph (or 16kph as they are called in Israel) would be great. Better would be if it could reach twice as much and I could limit it with the ESC.
* **Cheap**: I'm sending him to work in the mines, but he's very weak so he can't make much $ for now. I have to admit that I already realised that it would cost more than I hoped it would, but I'm still hoping to keep it cheap.
* **Limited torque**: the kid is 35kg, and with a restrictive diet he shouldn't grow much. His pickaxe is just another 1Kg. There are no big hills to climb, and limited initial acceleration is a plus.
* **Limited range**: Better for ensuring he comes back home once in a while to charge, and not cohorting with those scary looking skateboard dudes. 

### My thoughts so far
* **Single hub**: Cheaper than dual. Simpler assembly than a pulley/mount system. 
* **Single battery pack**: Small, lightweight, limited current.
* **Low Energy**: Compared to a "standard" build, we aim for 
  * 60-70% lower weight
  * 50% less distance
  * 50-70% lower upper speed
  which my "bottom of an envelope" calculations shows much lower energy consumption.
* **procurement:** Besides a battery which I can try and get locally, I prefer stuff that can be ordered from Europe or [China], or from the US for reasonable shipping prices.

### Specific questions
1. Is there a cheaper way to go instead of a vesc? I understand the importance of it, but considering the small battery and limited speed/torque, is there a cheap alternative?
2. Should I consider a really fast skateboard so he can work an extra shift in the bakery? 
3. I assume a single hub can be enough. I also assume it's installed on the back truck. Is that crazy?

### How about these?
1. [ PULSE 4500mAh 5S 18.5V 45C - LiPo Battery](https://www.pulsebattery.com/plu45-45005-pulse-lipo-4500mah-18-5v-45c-ultra-power-series.html)
2. [MTO9055-HBM-60-HA hub motor](http://www.maytech.cn/en/mto91hbm-nh/8803.html)
3. some el cheapo esc, preferably that comes with a remote?

I'll appreciate any thoughts, pointers and such. Thanks a lot in advance!
```

---
## \#2 Posted by: Acido Posted at: 2018-09-20T20:36:11.842Z Reads: 246

```
hoping this kid stuff is a joke...
```

---
## \#3 Posted by: faithfulpuppy Posted at: 2018-09-20T20:43:05.034Z Reads: 247

```
no, he's one hundo percent serious. My dad works at israel and told me it's true.
```

---
## \#4 Posted by: Sebike Posted at: 2018-09-20T20:54:22.387Z Reads: 241

```
All my three kids work in mines. They leave at 3.45 AM. No time for breakfast. Without them we'd be broke. I usually spend my days lying on the sofa making sure I won't be too tired to welcome them back home when they get back at midnight.
```

---
## \#5 Posted by: owlen Posted at: 2018-09-20T20:55:30.187Z Reads: 235

```
[quote="Acido, post:2, topic:68675, full:true"]
hoping this kid stuff is a joke…
[/quote]

I'm serious! My son did ask me to do a project with him, and that's what we're planning. I'm already teaching him about torque, electricity, physical design... It's a great process. And when he grows up he can even become a mining engineer! 

PS: Just for full disclosure, there no (and never were any) mines in Israel.
PSS: We do have bakeries. Someone got to make those Challah bread...
```

---
## \#6 Posted by: Acido Posted at: 2018-09-20T20:59:46.960Z Reads: 214

```
do you at least supply them with new pickaxes every once and then?
```

---
## \#7 Posted by: Sebike Posted at: 2018-09-20T21:02:00.813Z Reads: 213

```
No.

It's their job, their business.
Just bring home the money.
```

---
## \#8 Posted by: yelnats8j Posted at: 2018-09-20T21:06:33.579Z Reads: 215

```
Do you make them walk or use Eboards?
```

---
## \#9 Posted by: Sebike Posted at: 2018-09-20T21:08:21.832Z Reads: 213

```
Tbh I don't know how they get there. What, do you think I'm awake at 4 AM?
```

---
## \#10 Posted by: b264 Posted at: 2018-09-20T21:29:47.983Z Reads: 211

```
[quote="owlen, post:1, topic:68675"]
Is there a cheaper way to go instead of a vesc?
[/quote]

Of course.  But you get to choose: cheap or good.

VESC is the only one that has good enough software where you can tweak the maximum allowed speed and power and braking individually.
```

---
## \#11 Posted by: mmaner Posted at: 2018-09-20T22:01:35.763Z Reads: 205

```
That was a funny read 😀

As far as the build, I would suggest going belt drive. Its a lot longer lasting and much better torque. I would also recommend a vesc, an RC ESC is gonna be nothing but trouble and the cheap Chinese ESC's aren't terrible but they offer no programming options. With a vesc you can limit duty cycle and amps to control top speed and torque.
```

---
## \#12 Posted by: b264 Posted at: 2018-09-20T22:16:02.959Z Reads: 199

```
Yes, I highly recommend belt drive also.  Hub motors are the worst.
```

---
## \#13 Posted by: dareno Posted at: 2018-09-20T23:05:38.401Z Reads: 194

```
These were my plans for my sons esk8.  Slow and steady.  Bought him a meepo.  That thing now runs 2 focboxes and a 10s 5p with the amps far too high because the little shit is a speed demon.  I'm now building him a mini mountain board so he can hit the off road trails..........when will this obsession stop.
Its actually a great bonding process and they learn so much during.  Hes the one who sets his own parameters now with some basic ground rules in not blowing the thing sky high.  Hubs are not all bad for small kids.  If your son is anything like mine then he won't be careful with it at all and with belts and satellite motors there is an awful lot of undercarriage to wreck. Definitely go with vesc over esc though.  Much more control for you as the parent. Good luck!
```

---
## \#14 Posted by: owlen Posted at: 2018-09-20T23:14:20.300Z Reads: 178

```
@b264, @mmaner, thanks for the input! I thought hubs are "the future". Maybe it's simply not the future yet...
A belt drive will be much more fun to build (plus the added "gear ratio" tutorial for my son), but wouldn't it also be more expensive?

* Can you give a rough guidlines for a <40Kg rider, <20 kph top speed and just reasonable torque?
* A single 6355 170kv on a Gear ratio of 2.4:1 with a 6S1P battery should be fine? Would love your input on this.
* [Here is a calc I used](http://calc.esk8.today/config/?type=3.7&scells=6&pcells=1&cc=2.25&da=65&mda=65&kv=170&poles=14&eff=90&wheel=80&mp=15&wp=36&wpm=18). The default is 18 W-hr. I have no idea what to put there, but I assume it shold be lower with a much lower load. Any thoughts on this?

@dareno, that's a valid point - not only there is a better chance of something breaking, he'll probably let his friends ride it and the chance of misuse grows even more... Did the meepo had just one hub originally? What do you think of the original plan I've put?
```

---
## \#15 Posted by: trancejunkiexxl Posted at: 2018-09-20T23:17:08.536Z Reads: 164

```
I have some parts that I would not miss and you can have. I think we can do better than cheap. Only issue is shipping I guess
```

---
## \#16 Posted by: owlen Posted at: 2018-09-20T23:21:54.202Z Reads: 160

```
[quote="trancejunkiexxl, post:15, topic:68675, full:true"]
I have some parts that I would not miss and you can have. I think we can do better than cheap. Only issue is shipping I guess
[/quote]
Wow, that's awesome! Gonna figure out how to PM you for details.
```

---
## \#17 Posted by: dareno Posted at: 2018-09-20T23:27:19.440Z Reads: 166

```
No they are a twin hub design  and very cheap for what you get.  A single hub design is fine for a 9 yo.  Put it this way when the meepo was stock it pulled him up hills as fast as my dual 6374 10s board got me up them.  I had the little git on the flat though.  Great plan for a starter set up for him.  Again though if hes anything like my boy then he will be riding that thing like a pro in no time and making his dad look slow so might be an idea to over engineer it to start with and use limits rather than have to build a complete new set up when he gets bored and he will.
```

---
## \#18 Posted by: dareno Posted at: 2018-09-20T23:30:05.918Z Reads: 161

```
Oh and full safety gear is a must for him.  Trust me mothers get really funny about kids with missing skin.  Who knew?
```

---
## \#19 Posted by: trancejunkiexxl Posted at: 2018-09-20T23:32:12.938Z Reads: 159

```
whats the price on this single hub @dareno ?
```

---
## \#20 Posted by: dareno Posted at: 2018-09-20T23:33:58.058Z Reads: 160

```
What single hub?  The meepo has a diyeboard twin
```

---
## \#21 Posted by: owlen Posted at: 2018-09-20T23:35:31.477Z Reads: 147

```
Yeah, the safety gear will be there. No worries. I've already joined the www.diy-padding.builders forum... I'm also not worried about him getting faster than me - my mother doesn't allow me to ride any skateboard anyway :anguished:
```

---
## \#22 Posted by: trancejunkiexxl Posted at: 2018-09-20T23:35:35.060Z Reads: 136

```
i c that now, i imagine he weighs like 45kg? single hub could be good option but not very serviceable. what do u think :slightly_smiling_face:
```

---
## \#23 Posted by: dareno Posted at: 2018-09-20T23:39:43.755Z Reads: 140

```
[quote="owlen, post:21, topic:68675"]
my mother doesn’t allow me to ride any skateboard anyway
[/quote]

I was bombing a local hill the other day and hitting around the 50kmh mark and when I got home I had the tapping of the feet...I had the crossing of the arms......I had the distinct impression the wife was upset.  She was behind me in her car apparently and didn't realise just how fast they can go.   I had to do the explaining......
```

---
## \#24 Posted by: trancejunkiexxl Posted at: 2018-09-20T23:43:15.279Z Reads: 127

```
Careful, Lol my woman stole my loop key 🤣
```

---
## \#25 Posted by: owlen Posted at: 2018-09-20T23:43:43.737Z Reads: 129

```
He is more like 35kgm and I'm not a big guy, so I guess it would take him a while to reach 45 kg...

[quote="dareno, post:23, topic:68675"]
She was behind me in her car apparently and didn’t realise just how fast they can go. I had to do the explaining…
[/quote]
:rofl:
```

---
## \#26 Posted by: b264 Posted at: 2018-09-20T23:45:20.486Z Reads: 132

```
[quote="dareno, post:23, topic:68675"]
behind me in her car apparently and didn’t realise just how fast they can go
[/quote]

That feeling when a car is behind you at a red traffic signal, irritated you're in front of them and trying to go around you (since you're in the middle of the lane) then the light turns green and you just disappear, accelerating faster than their car can.  *That* feeling
```

---
## \#27 Posted by: trancejunkiexxl Posted at: 2018-09-20T23:45:57.533Z Reads: 124

```
ya cruising intersections when lights change green and u crush it :crazy_face:
```

---
## \#28 Posted by: dareno Posted at: 2018-09-20T23:47:20.150Z Reads: 123

```
They should realise by the way you are leaning forward at a 45 degree angle that something special is going to occur
```

---
## \#29 Posted by: Jake2k17 Posted at: 2018-09-21T00:48:10.239Z Reads: 125

```
honestly I would take the mines over high school
```

---
## \#30 Posted by: owlen Posted at: 2018-09-21T21:04:33.210Z Reads: 134

```
Two decisions so far:
1) We're thinking of taking the HUB instead the belt route. I'm sure more torque can be gained with a belt and there are probably other benifits, but considering it's much simpler to install, and going to be used by a 35kg kid, I think HUB makes sense.
2) We'll use a vesc. The only reason not to was price, but one of the commenters above was kind enough to offer to send us a great unused vesc for free(!!!!). If he wouldn't mind I'll let you know who was it of course. We're both thankful, surprised and thankful. 

Questions:
1) Found this cheap hub: [Maxfind 70mm/90mm Motor 500W](https://www.aliexpress.com/store/product/Maxfind-70mm-90mm-Electric-Skateboard-Motor-500W-Highspeed-Drive-Brushless-Hub-Motor-Self-balancing-Intelligent-Motor/1947786_32910347688.html?spm=2114.12010615.8148356.4.20c05288hPr2bk). There are many spces but no KV rating. Any simple way of calculating it from what's there? Anyone experienced with Maxfind hubs?
2) I'm realizing that mounting a hub can be trickier than mounting a regular belt mount, as I should find a matching square peg for the hub. Does that mean I'm better of ordering a hub plus truck from the same source?
3) Is there a minimal battery limit for a motor, and if there is - how is it calculated? Considering the prefered low top speed I would like to use a lower cell battery count, like a 3S for example. 

Again, thanks in advace!
```

---
## \#31 Posted by: b264 Posted at: 2018-09-21T21:22:46.451Z Reads: 129

```
[quote="owlen, post:30, topic:68675"]
I’m realizing that mounting a hub can be trickier than mounting a regular belt mount, as I should find a matching square peg for the hub. Does that mean I’m better of ordering a hub plus truck from the same source?
[/quote]

I can't recommend cheap hub motors.

But yes, it does mean that would be the much preferred way.  Don't spend too much money on the hub motor and hanger though because it'll get replaced anyway in due time.  It will get you moving sooner though.

The VESC software has a way for you to measure the motor kv, but I would ask the seller before purchasing.  60kv to 90kv is a good range for that, preferably lower.
```

---
## \#32 Posted by: electric Posted at: 2018-09-22T18:45:46.445Z Reads: 120

```
Cheap hub-motors are fine In budget dual setups and they work!
But in single is it worth it?


(Cheap) hub-motors are prone to get cuts from small rocks and glass,
(Cheap) hub-motors do less to prevent vibrations than regular urethane longboard wheels,
making for a less comfortable ride and a worse situation for your electronics.

Also cheap hub-motors have a thin layer of urethane that will wear-out quicker than regular longboard wheels costing you money in the long run.
```

---
## \#33 Posted by: sami Posted at: 2018-09-22T19:04:24.479Z Reads: 113

```
Happy to see more Israelis in here please ask away in PM if you want
```

---
## \#34 Posted by: owlen Posted at: 2018-09-22T19:10:25.658Z Reads: 114

```
Thanks! 

I contacted the [Maxfind](https://www.aliexpress.com/store/1947786?spm=2114.10010108.0.0.5996659aYrgg5k) store on Aliexpress, to ask about the kv. The first answer was _"What do you want it for?? these are for skateboards"_ :man_facepalming: When I said it's for skateboard, I was told: _"If you want to use this motor ，you need to buy the truck."_  So much for these guys.

#### Two updates:
1) I forced my son to stand on a weight, and he's just 30kg, and not 35! We just got a little bit more torque for free :smiley:
2) I'm bidding on a used 2x Maytech hubs offered on the "used items" board. 

#### Question:
Since we hoping to get a single VESC, can we hook and run just one of the two hubs while leaving the other unconnected? I know hubs suppose to be able to spin without power, but I'm not sure if they would have high resistance or something.
```

---
## \#35 Posted by: dareno Posted at: 2018-09-22T21:44:44.460Z Reads: 107

```
[quote="owlen, post:34, topic:68675"]
Since we hoping to get a single VESC, can we hook and run just one of the two hubs while leaving the other unconnected? I know hubs suppose to be able to spin without power, but I’m not sure if they would have high resistance or something.
[/quote]
Wouldn't recommend doing that really.  No point when you can run a free wheel.  Just put it away till you decide to go dual.  Or as a back up.  
Maytech's are good hubs reliable and torquey but there are other good inexpensive options (was going to say cheap and good but @b264 will jump on my head) 
@rey8801 has done some good reviews on hubs and knows his stuff.
```

---
## \#36 Posted by: pat.speed Posted at: 2018-09-22T21:48:14.322Z Reads: 111

```
I wouldn’t recommend running the hub in connected. Instead either buy a spare 90mm flywheel and swap it with the pare hub motor or ask around if anyone has some left over ones
```

---
## \#37 Posted by: Eretron Posted at: 2018-09-22T22:10:06.731Z Reads: 118

```
Well if you decide to go belt route, I have a mildly used evolve 5065 150KV motor that is collecting dust, so if you find it useful I'll ship it to you free of charge, just pay for the shipping.

I am from Europe so it shouldn't be much...

It's not pretty, but its almost new, and fully functional.

![IMG_8262|666x500](upload://16yAC44p19YfL9FmEtE7vyBPYFg.jpeg)
```

---
## \#38 Posted by: rey8801 Posted at: 2018-09-22T23:04:53.284Z Reads: 112

```
@visnu777 is selling used replaceable 90mm hub motor for cheap. @owlen yuu could ask him. You don't need a vesc, you can also go for a cheap ESC capable for two hub motors. Or if you have a 4.12 VESC buy another from Flipsky for 60$ and you are done. Nice set up for cheap.
```

---
## \#39 Posted by: owlen Posted at: 2018-09-23T11:07:20.289Z Reads: 105

```
This forum rocks... Thank you all!
@Eretron - thanks a lot man! Already arranging for shipment of the above, but with all the goodwill going on around here I'm starting to think I'll end up building one for myself :upside_down_face:

@dareno @pat.speed - I understand. So I'll probably remove one and keep it as a backup, and replace it with a free wheel. Can I assume that the truck, after removing the hub, will fit any 90mm wheel? Should I care about the width and other params, or "90mm flywheel" is the standard I should look for?

Unless (tan tan tan):
@rey8801 Someone offered to send me an unused [TORQUE ESC BLDC ELECTRONIC SPEED CONTROLLER](collections/featured-items/products/torque-esc-bldc-electronic-speed-controller) - are you saying that it can hook up as a master to a different (cheaper) vesc (or the flipkey you mentioned) and it would work normally? If that's indeed the case than we might connect the 2 hub as well(!!)
```

---
## \#40 Posted by: pat.speed Posted at: 2018-09-23T11:24:38.551Z Reads: 97

```
Any 90mm wheel should fit as long as the hub truck has a solid axle, some of the hubs (ie meepo) have the axles attached to the hubs themselves
```

---
## \#41 Posted by: J0ker3366 Posted at: 2018-09-23T11:29:15.739Z Reads: 98

```
Can I just say that this was the funniest build thread till the kid stuff was taken out lol. Good show my friend.
```

---
## \#42 Posted by: rey8801 Posted at: 2018-09-23T13:38:30.749Z Reads: 98

```
Actually the Flipsky is a newer version 4.12 compare to torque board. They proved to work quite well so of you already have the TB vesc fine otherwise but two Flipsky vesc for 100 euro or the dual 4.20 for 105 and you save in space since the size format is amazing. Check their website and take into account that usually you get 20% off of you like their Facebook page.
Anyhow if you already have the 4.12 from TB it's ok. Buy another 4.12 like Flipsky one and one is master rand the other slave. Both are stressed the same so doesn't metter of one is better or not  to be a master. In this way you can connect them and run dual. Plus with a cheap bluetooth module you can change the mode from your phone and for instance make the safe mode for your son with top speed 15 kmh, and 300watt max power so you know that he is not gonna hurt  himself. And then when you want to use it change in 1 sec from your phone to release all the power! Rock :grin:
```

---
## \#43 Posted by: goldrabe Posted at: 2018-09-23T14:03:43.753Z Reads: 94

```
Is there someone who can check and repair VESC's in Israel?
I have a Maytech VESC which I would let go, it just shows overvoltage faults. One of the capacitors is dented, so i am guessing they need to be replaced.
```

---
## \#44 Posted by: owlen Posted at: 2018-09-23T16:54:58.735Z Reads: 90

```
[quote="rey8801, post:42, topic:68675"]
Flipsky vesc for 100 euro or the dual 4.20 for 105
[/quote]

On [their site](https://flipsky.net/collections/electronic-products) I see a bit higher prices, but they do look nice!
I don't see a Bluetooth option on the [mini fsesc](https://flipsky.net/collections/electronic-products/products/mini-fsesc4-20-50a-base-on-vesc-widely-used-in-eskateboard-escooter-ebike) 0 is this a separate module I can connect to the vesc?

@J0ker3366, I didn't take the kid stuff out, there was just no update. But worry not - I'm about to feed him today or tomorrow the latest, so I'm sure there will be something to write about... :wink:

@goldrabe - I really don't know the local scene that well, but I've asked on a local facebook page.
```

---
## \#45 Posted by: rey8801 Posted at: 2018-09-23T18:02:33.810Z Reads: 93

```
FLipsky 4.12 https://www.electric-skateboard.builders/t/taobao-aliexpress-bangood-alibaba-all-the-chinese-deals-here-community-log/57716/98?u=rey8801
Flipsky 4.20 https://www.electric-skateboard.builders/t/taobao-aliexpress-bangood-alibaba-all-the-chinese-deals-here-community-log/57716/102?u=rey8801
Dual only on website. You can either ask a discount to them on Facebook after you like their page or take part of a group buy. Depends where you ar elocated there are EU and USA.
Bluetooth is separate, but not expensive at all. I have some for cheap plug and play https://www.electric-skateboard.builders/t/esk8-flea-market-eu-ww-small-cheap-parts-hm-10-bluetooth-android-oreo-compatible-volt-meter-3dprinting/57463?u=rey8801
Otherwise buy a HM-10 module and solder it by your self. Pay attention to the module for the compativility with Android Oreo in case you have it.
```

---
## \#46 Posted by: owlen Posted at: 2018-09-30T21:31:56.421Z Reads: 88

```
You guys are really awesome! Thanks to your help we now have 2 Hubs + truck, 1 vesc, and another truck that are on their way to Israel! it would take them few weeks to get here, and then just a few more days to pass security screening on the border to ensure they are not terrorists or worse - vegans. While we wait for them, it's time to think about a deck:

My son is 9 and about 30kg. He's used to a very small plastic board with a kick tail. We played with some mockup, and we believe 27 inches would be good for his size. We'll be using hubs, and probably a low capacity battery. Would love to hear your thoughts about it. 

Here is a cheap option I found on aliexpress. Does the size make sense? 7 layer of maplwould be enough for a 30kg (66 pounds) rider?
https://www.aliexpress.com/item/24-27-Inch-7-Layer-Maple-Blank-Skateboard-Deck-Skate-Board-Concave-Kick-Decks-Skate-Board/32920089262.html

Any good UK/EU source for a short blank deck?

I'm starting to like this project so much that I'm thinking that it would be best if the board would be too thin for me to ride. Otherwise, the boy might never get to use it...

In the photo below: Two very short decks made of bread, separated by meat. With pickles. 

![image|307x230](upload://57lZgYZ1Ab3p75OJuqEHYlqjgJY.jpeg)
```

---
## \#47 Posted by: trancejunkiexxl Posted at: 2018-09-30T21:59:17.681Z Reads: 84

```
so are you still missing 2 wheels?
```

---
## \#48 Posted by: owlen Posted at: 2018-09-30T22:32:24.272Z Reads: 83

```
Ah, yeah, we actually need 4 wheels! All this advanced math is driving me nuts...
According to @pat.speed "any 90mm wheel should fit". So I thought any regular wheels would be relatively easy to come by. Now that I think about it, he was answering my question about using a single hub setup. So we might actually need 3, not 2. 1 for the Maytech truck and 2 for the awesome Caliber2 truck we got for free! (:sunglasses::gift:)
Another option is we might get another vesc and go the dual route as @dareno and @rey8801 suggested.
```

---
## \#49 Posted by: pat.speed Posted at: 2018-10-01T04:56:50.036Z Reads: 77

```
By “any wheel should fit” that is with the use of a spacer depending on if the truck with the hub motor has slightly larger axles than normal trucks, just a few washers or a wheel spacer will suffice
```

---
## \#50 Posted by: mountainboardlover69 Posted at: 2018-10-01T09:00:07.797Z Reads: 78

```
###  ILO Minimum Age Convention (No. 138)

ILO Minimum Age Convention No. 138 establishes 15 years as the minimum age for work, though in some cases 14 years is allowed for a specified period of time. The minimum age for work that is likely to jeopardize the health, safety or morals of young persons is 18, while light work that does not harm health or school work is allowed for children aged 13–15.

like the project is cool but com on man ....... 9 years old woking in mines..
i think a mepoo or other pre made boards are a better option or get a kit from diyeboard.com
```

---
## \#51 Posted by: moon Posted at: 2018-10-01T12:07:27.998Z Reads: 75

```
Don't get anything from diyeboards lol. They don't respect your privacy
```

---
## \#52 Posted by: MD84 Posted at: 2018-10-02T03:09:35.357Z Reads: 68

```
I worked in a mine starting at the age of 7. And just look how I turned out :face_with_symbols_over_mouth:
```

---
## \#53 Posted by: owlen Posted at: 2018-10-02T07:41:41.719Z Reads: 66

```
> I worked in a mine starting at the age of 7. And just look how I turned out :face_with_symbols_over_mouth:

@MD84 is right. And besides, the middle eastern labour laws are a bit different...

But maybe @mountainboardlover69 is right. My son does like soccer. Hmm, perhaps I should pull him out of the mine and send him to the soccer stitching shop together with his sister.
```

---
## \#54 Posted by: owlen Posted at: 2018-10-02T15:34:33.476Z Reads: 63

```
[quote="owlen, post:46, topic:68675"]
Here is a cheap option I found on aliexpress. Does the size make sense? 7 layer of maplwould be enough for a 30kg (66 pounds) rider?
[https://www.aliexpress.com/item/24-27-Inch-7-Layer-Maple-Blank-Skateboard-Deck-Skate-Board-Concave-Kick-Decks-Skate-Board/32920089262.html ](https://www.aliexpress.com/item/24-27-Inch-7-Layer-Maple-Blank-Skateboard-Deck-Skate-Board-Concave-Kick-Decks-Skate-Board/32920089262.html)

Any good UK/EU source for a short blank deck?
[/quote]

Can anyone comment on this?
```

---
## \#55 Posted by: pat.speed Posted at: 2018-10-02T21:13:06.210Z Reads: 61

```
Looks ok. It will definitely work fine for your son. I’d got for the 24” as it will be easier for him to use.
```

---
## \#56 Posted by: owlen Posted at: 2018-10-07T22:31:49.681Z Reads: 54

```
Thanks! Ordered.
```

---
