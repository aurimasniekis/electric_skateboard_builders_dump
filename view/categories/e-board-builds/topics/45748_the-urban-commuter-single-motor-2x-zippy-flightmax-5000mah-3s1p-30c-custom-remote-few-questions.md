# The Urban Commuter &#124; Single motor &#124; 2x Zippy Flightmax 5000mAh 3s1p 30c &#124; Custom remote &#124; Few questions

### Replies: 15 Views: 1078

## \#1 Posted by: bge22 Posted at: 2018-02-06T19:22:37.245Z Reads: 187

```
Hello everybody and thank you for the impressive amount of information posted all around this forum.

I am final year CS student and I'm lurking around for the last 2 or 3 weeks reading as much as I can and I understood that my initial idea "this is gonna be an easy plug 'n' play" was so, SO wrong...

I will try to be as short as possible, therefore I won't go through all the options I took into consideration before and will go straight at the current chosen path (and hopefully the one that I will follow).

*** DISCLAIMER***
I've read dozens of topics and I know the general recommendations, but given my absolute zero experience I'd like to have some input from the experienced builders that know their way around and have real experience with this (or similar) parts. Thank you!
***

I have a 22" Cruiser that I want to transform into a more pleasant commuter to use on my way to the university, job and around the city, sometimes in conjunction with the public transport.

I have around 65kg so let's say with my laptop and some stuff in my backpack I reach 70kg (or 155lbs) and the city is quite flat (I can think of only 2-3 hills or slopes around) so I guess I will be fine with a single motor.
I would love the duals, but I'd like to keep the budget as low as possible on this first build in order to get just get going on this topic and invest more money on my future builds when my requirements will be more specific.
 

Parts list (to be updated):

* HK Keda 6364 motor 190kV
https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html

* FVT 120A ESC
https://www.aliexpress.com/item/FVT-2-6S-LiPo-Battery-120A-Waterproof-Brushless-Car-ESC-For-1-8-1-10-RC/32791751551.html

* 2x Zippy Flightmax 5000mAh 3s1p 30c
https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-30c.html

* LiPo batteries protectors
https://www.aliexpress.com/item/15-6-4-5cm-Silver-High-Quality-Glass-Fiber-RC-LiPo-Battery-Safety-Bag-Safe-Guard/32791790597.html

* Aliexpress rubber wheels (not the greatest pavement in my city and I'd like a bit of dampening)
https://www.aliexpress.com/item/Outdoor-75A-Professional-Wearproof-Durable-PU-Rubber-Wheel-for-Longboard-Mountainboard-70x45mm-Snowboarding-Accessories/32849774601.html

* Aliexpress pulley kit
https://www.aliexpress.com/item/Mayitr-Electric-Skateboard-Motor-Pulley-Mount-Accessories-Belt-Kit-for-72mm-70mm-Wheels-Stainless-Steel-Skate/32817684750.html

* Custom remote with Arduino and 433MHz Radio

* Custom battery monitor with display and low voltage alarm (still Arduino)

* Custom fiberglass case


Now the questions I have:

1. On this specific configuration I would have a max. speed of around 16km/h (or 10mph).
I'd like a bit more speed, therefore I was thinking of changing the motor pulley to a 28 teeth so the max. speed would increase to 28km/h (or 17mph).
Will this result in not having enough torque?

2. Should I go with a higher kV motor? Would a 5065 with 270kV be better for this? Maybe an Alien Power 42mm with 300kV?
I know I should go higher on battery voltage, but that would result in having to buy another ESC that will be quite expensive.

3. I was thinking of a chain drive that would give me a 14:27 ratio, but the diameter of the wheel sprocket is 58mm and the wheel has 70mm. I am thinking this will result in problems (not enough ground clearance), am I right?

Thank you in advance!
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2018-02-06T20:13:11.131Z Reads: 166

```
Hey man, great to see a complete list, but there are a few things you might have to reconsider. I can understand that you want to build this on a budget, however it isn't always advisable to go for the cheapest in the esk8 hobby since that often means buying twice.

I think the motor is a good choice, it should be enough to get you across a relatively flat cityscape and has both 63mm and 50mm mounting holes.
The ESC is probably fine if you don't catch one with quality control issues but it won't come close to the feel of a VESC.
The Lipos should be fine too for this ESC.
I haven't seen those wheels before and i'm not sure if anyone has experience with them. They could be nice but they also kind of look like a piece of candy on the picture and i'm not sure if the core will be strong enough to hold the pulley. Maybe stick to regular longboard wheels.
The Motor mount could be ok if you can make sure that your truck is thin enough to accomodate the mount, i made that mistake and had to file down my truck for ages.

I know the struggle of wanting to build as cheap as possible and i don't want to discourage you, but after all it's a vehicle and cheaping out doesn't give you the best value. Maybe save up a bit more and go for tested and reliable parts.

Oh and with the arduino remote - you might want to look into the nrf24l01 2.4ghz modules, i would assume they are more reliable than those 433mhz things. (i cant even get a reliable connections over 1m with the 433mhz ones).
```

---
## \#3 Posted by: Grozniy Posted at: 2018-02-06T20:53:04.262Z Reads: 146

```
[Take a look at this](https://www.electric-skateboard.builders/t/student-budget-e-board/45571/21?u=grozniy)
```

---
## \#4 Posted by: pat.speed Posted at: 2018-02-06T21:09:59.356Z Reads: 152

```
Hey mate welcome, that build list is fairly decent and will work great with a few small modifications. I personally run a board nearly exactly the same as this. The motor and batteries are both good, the fvt esc works well from what I've heard but I use the HobbyKing Xcar beast esc and it's great. 

I would recommend some slightly larger wheels (atleast 83mm). I also use that pulley kit which is ok once modified to fit the flywheel cores properly, I swapped out the 16t motor pulley for a 24t one so now I have a 2:1 ratio and it still has plenty of torque.

If you would like any more information just send me a pm

Here's my board ![IMG_1140|375x500](upload://2N5Y5AFgexRPF7TUGr9VilZwfVj.JPG)
```

---
## \#5 Posted by: Grozniy Posted at: 2018-02-06T21:24:31.358Z Reads: 137

```
How do you feel about your kit being 3M? Any belt skipping?
```

---
## \#6 Posted by: bge22 Posted at: 2018-02-06T21:43:45.635Z Reads: 139

```
Thanks guys for the fast replys.

@Der6FingerJo I'm aware that no ESC will come close to a VESC, but with the motor max. current at 90A and the price I am pretty sure I'll have to wait until my second build for it. Also if I'm going to buy the VESC I'll want the 6.x, not the 4.2 version, so I guess I'll be starting on a car ESC.
Regarding the wheels: yes, I agree they look kind of toy-ish so I'm still searching for other options.
Initially I decided to make my own motor mount, but when I found this kit I said "hey, I'm gonna try it and if it doesn't work, I'll make my own. If it works, I'm happy".
Theoretically a lower frequency means slower transfer rate, but longer range. Car keys are using this frequency so I'm going to give it a try (at < 1$ for the module it is so worth trying).

@Grozniy I read that specific thread yesterday and I actually took the kit into consideration, but I cannot find the gear ratio for it and I suppose it could be a 3:1 (as it seems to be a common ratio), which means the max. speed even using a 12s will still be quite low (aprox. 20km/h). Also I'd like to use my own board and spending money on parts that I won't use doesn't seem like a smart move for me.

@pat.speed I saw your build in the first days I began reading the forum and I was impressed with it, if I'm not mistaken it's actually the one that made me take into consideration using the penny board instead of a standard skateboard.
The HK Xcar is actually my other option. I saw there are some users on here swearing by it, while others recommending the FVT so that's why I'm on the fence... :sweat_smile:
My fear with larger wheels is the wheel bite and the stone to faceplant situation I sometimes have on the current wheels (70x54 78A).
```

---
## \#7 Posted by: Grozniy Posted at: 2018-02-06T22:08:15.606Z Reads: 121

```
The pulleys are 36:15T.
[Here](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":125,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":87}|) are specs for 10s setup, top speed 27km/h.
[Here](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":125,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":87}|) is 12s setup, 32km/h.
You will need a deck because it's not included.
You don't need to go faster than this on a penny board 🤣
You will have tons of torque.
It will be bolt on, no problems kit.
 VESC is smoother, more programmable and has better brakes than a ESC
Look at [This](https://www.electric-skateboard.builders/t/the-basic-build-hobbyking-esk8-kit-review/45288?u=grozniy)
```

---
## \#8 Posted by: pennyboard Posted at: 2018-02-06T22:34:55.795Z Reads: 112

```
I would recommend going with something bigger than a 22" cruiser. It's going to be really hard to find space to mount everything and be really awkward to carry cause of the way you'll have to cram everything on there.

Also, accelerating hard and going any speed over 15MPH is very unstable on such a small board. My first board was a 22" penny and I fell more on that in the month I spent riding it than I have in the year and a half I've spent riding larger boards.
```

---
## \#9 Posted by: Quezacotl Posted at: 2018-02-06T22:56:48.775Z Reads: 114

```
That motor mount is garbage. It feels good for a while, and then you experience that it goes constantly loose, even with great tightening and locktite. When you ultimately try to weld it in place, it's hollow and melts away. It is just weak. :smiley:
Another thing i saw that the smaller pulley is also weak. It takes only few times of belt slipping and the teeth grind away, increasing the slipping chance even more.

That ESC is interesting. Is there any smooth start on RC cars? I haven't really driven any serious RC, only children toys though.
```

---
## \#10 Posted by: pennyboard Posted at: 2018-02-07T00:28:44.427Z Reads: 109

```
@Quezacotl  Out of curiosity have you tried JB weld with the mount? That's the only thing I can think of that you haven't listed yet. 

@bge22  if you're insistent on going with a cheaper vesc alternative, why not give this esc a shot? It's cheaper and I've been pretty pleased with it on my cruiser board 
https://www.ebay.com/itm/single-motor-electric-longboard-skateboard-controller-ESC-Substitute/302546263597?hash=item4671299e2d:m:mGesvI1BOEcyvrLVbfKGQ8Q
```

---
## \#11 Posted by: Quezacotl Posted at: 2018-02-07T08:02:08.110Z Reads: 89

```
I have tried JB weld.
That mount is not just aluminium, it's maybe zinc-aluminium-something, which makes it resist the low-temperature welding. I'm not welding expert, but i heard this outcome means about that.
```

---
## \#12 Posted by: bge22 Posted at: 2018-02-07T10:59:51.117Z Reads: 83

```
@Grozniy Okay, my bad on the board and gear ratio. :sweat_smile:

@Quezacotl Would a HK Turnigy motor mount be better?
Regarding the ESC, I don't think that the start will come close to VESC's or will even be smooth at all, but I'm fine with push starting so no problem on that subject.

@pennyboard I looked at the eBay ESC, but it has absolutely 0 programming capability and even though none of FVT and Xcar are as customisable as the VESC, they give you a small degree of tuning. I also don't like the remote as I have some functionalities in my mind that I want to implement in my custom one.
In your build topic you seemed pretty impressed with the "100$ POS" which exceeded your expectations. Has it been so bad in the last few months that it made you completely change your mind?

P.S.: Is HK inflating the prices on a daily basis, or is there something that I'm missing? :hushed:
```

---
## \#13 Posted by: Quezacotl Posted at: 2018-02-07T11:23:28.487Z Reads: 68

```
I don't have experience on turnigy mounts.
```

---
## \#14 Posted by: pennyboard Posted at: 2018-02-07T16:17:08.551Z Reads: 60

```
Yeah that's true, there's no programming, so what's shipped to you is pretty much what you get. Although there are 3 speed modes, that's basically it, you get no customizability. 

No, nothing's happened that made me change my mind. Maybe the title confused you, but the name "100 POS"  was what it was named from the beginning, sort of as a joke, so that's not a new name that I applied out of frusstration or anything. 
I still use that build quite a bit, mainly getting back and forth to class.
```

---
## \#15 Posted by: PennE Posted at: 2018-02-08T21:34:37.334Z Reads: 52

```
In terms of hobbyking's pricing, always make sure to clear your cookies before ordering, then wait on the product page for about 5 minutes and it will pop up a "one-time only discount" of usually around 10%.
```

---
