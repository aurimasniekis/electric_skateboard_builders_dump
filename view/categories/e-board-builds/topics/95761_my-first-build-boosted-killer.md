# My first build {Boosted Killer}

### Replies: 26 Views: 1532

## \#1 Posted by: Fre.dw Posted at: 2019-06-03T14:15:27.335Z Reads: 260

```
On this thread I'm gonna be keeping you up to date with my first build.In this build I'm always going to be looking for the best prices. The goal for this project is for the obvious things such as good speed, range and torque whilst also being aesthetically pleasing. I'm also always looking for your input and help so feel free to comment any thoughts. The design will be closely related to a boosted board e.g the internal cables and the natural wood deck.
```

---
## \#2 Posted by: captclearleft Posted at: 2019-06-03T14:49:57.695Z Reads: 241

```
Looking like some pretty good parts.  

I have used a similar style ESC/receiver in the past with pretty good results on a 6s setup.  
I think you are maxed at 8s with that unit.  (4.2x8 = 33.6) So that should be fine.

I have bought my share of Zippy Lipo's...  30-60c should work and be ok.  I have puffed all the Zippy's that I have got that were 12-24c, and the 25-50c.  So 30-60c should be good. 
On that battery - Look at the Specifications section and size.  An 8ah battery is going to be a big battery.  Here is [my setup](https://www.youtube.com/watch?v=-TEXCSU40yE) where I run [these batteries](https://hobbyking.com/en_us/turnigy-heavy-duty-5000mah-4s-60c-lipo-pack-w-xt-90.html).  I put them under the board in 3d printed enclosure...  If that helps.

I am not sure you need a BMS with Lipo's - Unless you are using it to charge the battery while the batteries are in the board.  Then you would need a BMS.  I am not a BMS Expert and I don't use them, but perhaps someone else can comment on that...

Looks good - Keep posting the pics !
```

---
## \#3 Posted by: Fre.dw Posted at: 2019-06-03T16:20:41.307Z Reads: 208

```
@captclearleft Wow amazing build!
Yes the bms is so i can charge the lipo's internally.
The esc is rated for 36v and 2 5s lipo's in series is 37v so an over volt of 1v is ok with me.
Also what esc are you using in that build.
```

---
## \#4 Posted by: Vykku Posted at: 2019-06-03T16:53:47.959Z Reads: 205

```
You should be able to get the ESC and trucks / wheels / motors from @dickyho for cheaper.

Edit: Here are some links: 
https://www.ebay.com/itm/DIY-dual-1500W-electric-longboard-drive-kit-90MM-wheel-7-trucks-5055-180-270KV/302590418888?hash=item4673cb5fc8:g:g8sAAOSw3wVaTov8

https://www.ebay.com/itm/Dual-motors-longboard-skateboard-controller-with-remote-ESC-Substitute/302812941839?hash=item46810ece0f:m:mEjYlp9id5UtRAwhPmlchiw&amp;var=601709105317

You can get 10% off Ebay prices if you buy from him directly.
```

---
## \#5 Posted by: captclearleft Posted at: 2019-06-03T16:57:27.682Z Reads: 187

```
@Fre.dw , Thanks!

Just to clarify... Fully charged Lithium cells are 4.2v.  Fully discharged Lipo is 3.2, fully discharged Lion is 3v (rare for someone to go to 3v, super risky).  That being said.  Two 5s Lipo's in Series is a 10s1p - That is 4.2x10 = 42 volts.  I personally would not worry about the batteries.  I would worry about that ESC.

So If you give the ESC more current than it can handle (HEAT), and the motors want that current... The ESC will try to give that current (There is no protection (Thus the manufacture recommended voltage range)), causing an array of BAD!  When your ESC fails, its a roll of the dice with regard to what happens with your wheels(motors).  Sometimes they stop, sometimes they go full speed, sometimes fire in the box... 

That being said.  I use the older [VESC 4.12](https:///collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller).  These work great, and have been super reliable.  

![build6x2|375x500](upload://vd4BLUTfLuyj1AGem0iGjnDQjD9.jpeg)
```

---
## \#6 Posted by: Fre.dw Posted at: 2019-06-03T17:02:19.652Z Reads: 169

```
thank you for the help but i live in the uk so delivery costs would make it even more expensive
```

---
## \#7 Posted by: Fre.dw Posted at: 2019-06-03T17:08:53.788Z Reads: 163

```
I think now I'd like to use a vesc's aswell but its so much more expensive when you take into acount the spark switch and indicator but im sure its probably money saving in the future. Are these Vesc's the same as [this](https://www.amazon.co.uk/Tree-Life-Electronic-Electric-Skateboard/dp/B07QPZLQD1/ref=sr_1_1?keywords=vesc&qid=1559581485&s=gateway&sr=8-1) one. Its just the 50A seems to me, probably wrong though.
Also you're completely right with the batteries but I could use them with vesc's can'y I?
```

---
## \#8 Posted by: Vykku Posted at: 2019-06-03T17:31:57.239Z Reads: 151

```
I live in UK as well and have bought from him before. He can combine shipping, and also can pre-pay the tax so you won't have issues with customs afterwards. It does come out cheaper than the banggood ones, and postage is pretty quick.
```

---
## \#9 Posted by: KaramQ Posted at: 2019-06-03T17:33:15.391Z Reads: 141

```
Please don’t use those motors and trucks, I had a friend eat it at a group ride, the truck snapped and caused another guy to eat it
```

---
## \#10 Posted by: Vykku Posted at: 2019-06-03T17:34:28.150Z Reads: 138

```
If you do plan to get a cheap VESC, these seem the best choice, at least in UK: https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html?___store=en_us

They have a 1 year warranty and have good reviews on this forum, which is worth the extra £15-20 over the Aliexpress / Ebay special ones.
```

---
## \#11 Posted by: Tinp123 Posted at: 2019-06-03T17:37:41.175Z Reads: 139

```
Go with flipsky 4.12 vesc. Around 60$ on ebay, you can't beat that.

Don't even think about those old chinese esc, you will be disappointed and you won't kill any boosted board.
```

---
## \#12 Posted by: Fre.dw Posted at: 2019-06-03T18:24:59.197Z Reads: 134

```
@Vykku @Tinp123
Vesc it is. I'll get the flipsky just becuse its slightly cheaper.
This means I'll probably be running a single drive system but aloow room for upgrade in the future. can anyone recomend some different parts that will last? apart from battery im pretty firm on what i want. 
Any ideas on mechanical parts aswell is apreciated including trucks and wheels.
```

---
## \#13 Posted by: captclearleft Posted at: 2019-06-03T19:02:05.145Z Reads: 131

```
I agree.  VESC is the most common and proven way.  VESC is open source, so there are many manufacturers of the product.  As far as the antispark switch.  It's not completely necessary in my opinion -  I used just an XT90 loop for the longest time. You can see it on the back of my electronics box in the image I posted...  (Its just an XT90 male and female plug wired in between the hot wire from your batteries to the esc - To prevent spark when plugging in batteries)...  I then bought a couple of these from this guy.  Super good quality, a little big, but works great:
https://www.electric-skateboard.builders/t/vedder-anti-spark-switches-for-sale-from-18/31847
```

---
## \#14 Posted by: Flasher Posted at: 2019-06-03T19:49:23.855Z Reads: 115

```
I bought that exact esc. I have it in my old koowheel along with the original batteries and hub motors. It works well but I would never recommend it. Think of going the vesc or fsesc way for a killer. It's a pain to learn but once it's done you'll be in heaven. Too many limiting parameters in that esc compared to a vesc.
```

---
## \#15 Posted by: mutantbass Posted at: 2019-06-03T20:28:47.685Z Reads: 108

```
for a budget vesc, the flipsky 4.12 cannot be beat. its 45 euros ffs and i have done 1000km on my dual 6374s. 10s foc. 22 battery amps each 80 motor amps.
```

---
## \#16 Posted by: Fre.dw Posted at: 2019-06-03T21:34:02.388Z Reads: 101

```
Can anyone recomend a fairly cheap deck around £50. looking for just a plain twin tail around 40" long. Top mount aswell.
```

---
## \#17 Posted by: vasting27 Posted at: 2019-06-04T01:48:08.551Z Reads: 95

```
idk if you'll be "killing"  in boosteds
```

---
## \#18 Posted by: Guz Posted at: 2019-06-04T01:58:59.462Z Reads: 95

```
Yeah not sure if lipo’s and Chinese esc is the way to go if you wanted something similar to Boosted level.  Save more now and buy better gear, you will be throwing all that Chinese shit in the bin before three months, like I did.
```

---
## \#19 Posted by: captclearleft Posted at: 2019-06-04T15:05:42.535Z Reads: 81

```
As for your deck.  So many options.  If you are new an doing a lot of custom work; maybe a longer board 42" (or somewhere around there.).  A longer board is more stable, has a little more flex, and more area to work with when mounting your components.  
[Here is my first build with a $39 Rimable board from Amazon.](https://www.amazon.com/gp/product/B06XS2NCMH/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)

![firstbuild|690x388](upload://3xXUhM1YiJ8NfbMcQsUnVJMj0Cz.jpeg) 


Below is my current build.

 [Here is the board that I used in the image I previously posted.I like this board so much - I bought another.  (#L240)](https://www.skateshred.com/40-75-x-9-75-drop-down-drop-through-deck.html)

This SkateShred board is a "W" shape.  So its not completely flat underneath. But its super comfy on the feet, and has some flex which is nice.

NOTE: I don't know where these all ship to/from.  And the Rimable is not available as of right now.  The Rimable board is pretty stiff, but I put tons of holes in it, and it still holds up pretty well. I prefer the SkateShed over the Rimable.  I built a couple boards out of the Rimable boards because they were bottom mount, had tons of room for big tires, and were super cheap....
```

---
## \#20 Posted by: Fre.dw Posted at: 2019-06-04T15:54:12.865Z Reads: 70

```
Yeah I know this now, new part list coming soon I'll be doing a single belt drive build that then will be upgraded in the future to dual drive.
```

---
## \#21 Posted by: Fre.dw Posted at: 2019-06-04T19:08:42.265Z Reads: 63

```
I've removed the old parts list because i think it was causing confusion I'm not using those parts anymore
```

---
## \#22 Posted by: SkateYS Posted at: 2019-06-05T00:22:26.732Z Reads: 67

```
Killing the boosted and the Evolve just means spending a lot of money from what I've observed so far! I got a sick single drive that beats the boosted and a dual drive that kills the Evolve.
![|690x335](upload://mwKkNhYIvRrzZ2GjFNkx65JkjVD.jpeg) ![Any%20boosted%20killer|690x335](upload://levRNJIaVYxPFPuj51iRPdG7MZC.jpeg) 
 I have a Doc with all parts, specs and links to every single part I have used! 😎 If anyone wants to really kill the game!
![|690x388](upload://zoBDJcI9L6uCn4gKmW4YhIbRpWf.jpeg) 
![~%2050%20MPH%20-%208%2C064%20WATT%2012mi%20Range%20beast%20%2C|272x500](upload://v56noD0L4k0q7kwjXQQ4QhVhjOV.jpeg)
```

---
## \#23 Posted by: Fre.dw Posted at: 2019-06-05T16:37:12.982Z Reads: 48

```
Send your parts list
```

---
## \#24 Posted by: SkateYS Posted at: 2019-06-05T20:45:16.329Z Reads: 45

```
Single Drive
https://drive.google.com/file/d/1WySU0mixLTqjz4jkEFX75J1GgdtbI-t2/view?usp=drivesdk


Dual Drive
https://drive.google.com/file/d/17MatxH2dB1TQLIRj4UMSvbgxqVqeMtOm/view?usp=drivesdk
```

---
## \#25 Posted by: infiniteoffset Posted at: 2019-06-08T13:32:38.517Z Reads: 38

```
[Flipsky FSESC 4.12](http://s.click.aliexpress.com/e/cqB8jf76) is $35 cheaper than Turnigy ESC and v4.12 should be reliable. Free shipping as well. Also I wouldn't trust hobbyking 1 year warranty, I used to buy there lot of stuff for RC models, warranty process can take even over 3 months (personal experience) and with electronics like ESC they will often tell you to buy another one, they will give you new one for free only if it was dead on arrival.
```

---
## \#26 Posted by: Fre.dw Posted at: 2019-06-11T22:01:12.551Z Reads: 26

```
Here's the new parts list opinions and help please.
Remember i live in the UK

![image|690x388](upload://hwY2CtyVD1WW4ufgUPkqxukz1Vc.png) 

![image|690x388](upload://xCRCIwtHxZkFby7IByO8qZjjAmI.png) 

![image|690x388](upload://ezQalxDxvt0MGtPCLFZ11HNPzZJ.png) 

![image|690x388](upload://nEoHcJMEQBHKpLsMRa7WeECzc6M.jpeg)
```

---
