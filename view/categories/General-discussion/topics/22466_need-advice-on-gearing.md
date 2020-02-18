# Need advice on gearing

### Replies: 20 Views: 1260

## \#1 Posted by: jmart432 Posted at: 2017-05-05T14:13:34.715Z Reads: 134

```
Hey guys I'm new here and looking at building myself an electric longboard. I do have a bit of a history with RC cars so I get the basics with the electronics but I'm having a bit of trouble deciding on the gearing I need for the board. I understand that with the motors a lower kv rating means more torque and a higher one means more speed. I'm looking at the Turnigy Aerodrive SK3 245kv on two 3s lipos in series which I think should be pretty good for where I'm riding - no very steep hills, mainly flat but a few gradual or not too steep hills - but I'm not completely sure what ratio I should be looking at for the gearing.
I know the size of the wheels on the long board do play a part in the gearing but I don't have the board yet so I'm not sure how big the wheels are. I've been looking at these cheap motor mounting kits on ebay which I know won't be the best quality but they're cheap (http://www.ebay.com.au/itm/Pulleys-and-5065-Motor-Mount-Kit-DIY-Electric-Skateboard-Parts-For-72-70MM-Wheel-/322321348553?hash=item4b0bd977c9:g:aHgAAOSwImRYIanj). 
There are a few different kits you can get with different tooth pulleys for different ratios but I'm not sure which one would be best. So would someone be able to give me some ratios I should be trying to get with different size wheels (i.e what ratio for 60mm, 70mm, 80mm)?
Or even what max speed I should get with that battery and that motor on 6s and then I can use the speed calculator on this site to work out my ratio and wheel size?

Thanks heaps 
-Jacob
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-05T14:55:08.801Z Reads: 120

```
Somewhere around 16/36 should work for you, you could even go tighter if your motor and battery can handle it.

While wheel size somewhat affects torque, the far bigger factors are rider weight and riding environment
```

---
## \#3 Posted by: sl33py Posted at: 2017-05-05T15:12:32.958Z Reads: 117

```
Agree w/ @Jinra.  

I'd suggest the most common setup:

83mm Flywheels or Clones - then w/ your motor and battery - with my speed calc sheet i see:
83 - 245 - 6s - 15/36 (usually more common that 16/36) = 20mph build.  

If you do go 16/36 = 22mph (all approx)

How much do you weigh?  That's really the missing piece here.

Gradual hills - it's all about a good run at the hill and keeping RPM's up.

I typically gear as low as i can for more hill and torque performance.  Limiting speed too for running 8s-12s.

The biggest gap i see, is which ESC are you going to use?  I would usually figure this out first, then figure out batteries (# series / voltage) - then correct kv motor - finally gearing.  Running higher voltage will give you more power, but then you need to gear down further to avoid a "rocket" build.  I usually run 8-10s but also limit motor kv and gear down to keep speeds reasonable (like the 14/15 motor and 40t if wheel is big enough).

While i'm deluging you w/ random info - your deck choice also will sometimes dictate smaller wheels.  A symmetrical board like Vanguard can run big wheels 83/90/97's, but on a top mount standard deck you might need risers just to fit 83mm!  I'm not a huge fan of risers as it starts to get a bit high off the ground and i try to avoid and run as low as possible.

HTH - GL!
```

---
## \#4 Posted by: aigenic Posted at: 2017-05-05T15:13:15.644Z Reads: 96

```
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":245,"system-efficiency":90,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":83}|

Her you have a calculator for your speed...you can use it to estimate your max speed...if you are not too heavy (80kg+) I would go with a ~245kv motor with 6s battery...

For example on 15/36 setup I have conquered 18% hill with 240kv motor and 6s battery (I weight 72kgs) so it will give you enough torque (I don't use this setup anymore, if you would be interested, I could sell the electronics to you for quite cheap price, pm if you are interested :) )
```

---
## \#5 Posted by: aigenic Posted at: 2017-05-05T15:24:49.625Z Reads: 93

```
Also I do not recommend to buy that pulley setup...it might be cheap but it will be just a pain in the ass...You would probably have to modify your trucks, IDK if it fits calibers, but it doesnt look like that...The wheel pulley wont fit to ABECs, maybe on orangatangs, you should ask about it...there is no second ring for the pulley?! The belt is quite short and it is HTD3, which means it cant transfer enough torque with just 10mm wide belt...
There are so many reasons not to buy this :/
```

---
## \#6 Posted by: jmart432 Posted at: 2017-05-07T01:37:27.554Z Reads: 76

```
Hey everyone. Thanks for all the replies. The esc I'm using is this one https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html and I weigh 90kg. 
I still haven't got the long board yet but my neighbour has this long board he'd sell me. Still not sure the brand or wheel size but I'll post them up when I get it.
As for that motor mount kit, I know it's cheap and not gonna be ideal but originally I was just going to get the pulleys and belt and make the mount so I'm sure I'll be able to get it to work. The long board I'm buying probably isn't going to be some popularly used one with specific kits for it so I'm happy to do a bit or a lot of modifying to get the motor mount to fit.

Thanks for all the feedback I'll keep you updated when I get the board
```

---
## \#7 Posted by: aigenic Posted at: 2017-05-07T06:48:58.217Z Reads: 67

```
Yeah, u might get it to work...the C distance of the Motor mount is quite small, so it might be problematic with bigger (63xx) motors, because it wont fit on reverse kingpin trucks...
```

---
## \#8 Posted by: jmart432 Posted at: 2017-05-07T10:25:34.513Z Reads: 59

```
Alright everyone, got the board today. The brand is Drifter and it has 65mm wheels. Had to look up what reverse kingpin trucks were but the board does have them, so would someone be able to describe what the c distance is? and what I have to modify or buy to get either that motor mount or some cheap one to work with my board?
Thanks
```

---
## \#9 Posted by: jmart432 Posted at: 2017-05-07T12:01:04.155Z Reads: 52

```
Hey guys, been playing around with the speed calculator and I'm thinking the 65mm wheels might be a bit or a problem. The 245kv motor on 6s with 3:1 gearing and 65mm wheels will max out at around 13.8 mph which seems like it would be too slow. So, without spending even more money to get bigger wheels, what are my options? I've had a look at some different pulleys to get say a 2:1 ratio but I can't find much. With, say, a 300kv motor, I'd max out at 16.9mph, but I imagine I would not have enough torque with that motor. The esc I'm looking at is only rated to 6s so it would be expensive to upgrade that and get two 4s lipos.
```

---
## \#10 Posted by: aigenic Posted at: 2017-05-07T13:00:16.701Z Reads: 47

```
Go with at least 80mm wheels so you have enough space for motor mount, motor, drive gear...it is the easiest solution...what wheels do you have? can you post them? You probably planned to drill holes in them and then connect them with the wheels pulley by screws, which would go through the wheel, am i right? 

Everyone on this forum use larger wheels with holes in core, so they can use pulley, which goes through the core...if you drill the holes in the polyurethane, you might damage it, your pulley probably wont be centered and taht will lead to high tension on belt, which will break more often
```

---
## \#11 Posted by: jmart432 Posted at: 2017-05-08T12:01:06.938Z Reads: 46

```
Thankyou for all the feedback everyone. Just because I want this to be a relatively cheap project, I've decided to just go with the setup I've described - with the 65mm wheels that came with the board. I know that it's not ideal but I want to put something together and I can get bigger wheels later on if I need them. 
So I'm going to run the 245kv sk3 motor on this esc https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html and mounted on this http://www.ebay.com.au/itm/DIY-Electric-Skateboard-Kit-Parts-Pulleys-Belt-and-Motor-Mount-For-80MM-Wheels-/322322475393?hash=item4b0beaa981:g:~UEAAOSwcLxYIu3Y.
I'm just not sure about a few things. Firstly, do I need a programming card? I assume the esc comes set up with some relatively normal car settings which probably aren't ideal but they'll work fine won't they?
Also, I've seen a lot of videos of people making their own boards and pretty much all of them use some sort a anti-spark device, but I hadn't seen much about them for rc cars - so do I need something like that (also, is there a certain plug that is anti-spark I could use for the batteries instead of having a separate anti-spark thing?) 
Last thing is I know that the mounting kit I linked was not recommended and neither were the 65mm wheels I'm going to use, but, before I get some bigger wheels, will I be fine riding with those wheels and that pulley? As in will the wheels be big enough to give enough ground clearance between the pulley/belt and the ground?

Thanks very much for all the help
-Jacob
```

---
## \#12 Posted by: Jebe Posted at: 2017-05-08T12:16:57.914Z Reads: 43

```
Read. Lots of information here -  I don't think you're ready to build.
Do you have a pulley for these 65mm wheels?
There are reasons why no one uses wheels this small.
A poor man buys twice.
```

---
## \#13 Posted by: jmart432 Posted at: 2017-05-10T06:54:41.497Z Reads: 42

```
Ok guys. Been doing a lot of reading here and I've decided if I'm going to do this I might as well do it properly. So, here is what I'm going to buy diy-electric-skateboard-kits-parts/torqueboards-single-motor-mechanical-kit/?attribute_motor-mount-size=63mm+Motors&attribute_wheel-color=83mm+Clear+Blue&attribute_motor-mount-pulley=16T+HTD5+12mm+Motor+Pulley
diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html
https://hobbyking.com/en_us/quanum-2-4ghz-3ch-pistol-grip-tx-rx-system.html 
2 x https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack.html
https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html
https://hobbyking.com/en_us/hxt4mm-battery-harness-14awg-for-2-packs-in-series.html
So, I have got 2 things I'm not too sure about. First is should I go with that 245kv motor or get a 192kv equivalent? With the 83mm wheels both of them will go quite fast but as long as the 245kv one will have enough torque for some small hills I will probably just go with that.
Also, the vesc says it comes configured for a 190kv motor and 10s battery pack. Should I mess around with the settings or just leave it as is (I'm using 6s)?
```

---
## \#14 Posted by: aigenic Posted at: 2017-05-10T07:00:26.928Z Reads: 40

```
You will deffinitely have to set up your VESC, but it is not difficult, you just connect it to batteries, motor, computer and set it up in BLDC :) 
guides: https://www.youtube.com/playlist?list=PLICpQdAXJazT-ICMIgJuc2pl-w0-j1j9A

The motors is OK, I wouldnt be surprised if you could climb even steeper hills :O I have one similar (but used a little) for sale, but you are probably from the USA, so you would not be interested :/

About the remote, you should change it, this one is not good, may ppl couldnt get it to work properly...by mini remote from aliexpress or GT2B, they are reliable...
```

---
## \#15 Posted by: jmart432 Posted at: 2017-05-10T07:19:19.576Z Reads: 37

```
Ok thanks. I'll switch that for the GT2B from hobbyking. So you think 245kv will be fine with the steeper gearing and bigger wheels? I'm from australia btw
```

---
## \#16 Posted by: aigenic Posted at: 2017-05-10T07:47:20.738Z Reads: 35

```
With the kit you mentioned it will be ok :) I have runned similar set up 235kv, 15/36 and I had a really a lot of torque, good climbing ability :)
```

---
## \#17 Posted by: jmart432 Posted at: 2017-05-10T08:31:42.341Z Reads: 34

```
Awesome thanks. Another thing, for the mount/trucks/wheels kit, it ask whether the motor is 63mm or 50mm, looking through the specs for the Turnigy Aerodrive SK3 - 6364-245kv, it says diameter of 59mm, length of 52mm. I'm guessing the mount needs to suit the diameter, so do I need the 50mm or 63mm mount?
```

---
## \#18 Posted by: aigenic Posted at: 2017-05-10T08:42:14.985Z Reads: 37

```
The SK3 has 32mm distance between motor holes, thats all I know....Ask DIY's support, they will certainly know :)
```

---
## \#19 Posted by: Jebe Posted at: 2017-05-10T09:12:24.035Z Reads: 36

```
where in Aus are you?
you would need the 63mm mount
```

---
## \#20 Posted by: jmart432 Posted at: 2017-05-10T12:45:29.055Z Reads: 33

```
Alright thanks, I'll get the 63mm one. I live in Cairns
```

---
