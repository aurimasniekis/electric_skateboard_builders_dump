# Anti spark switch (fried)?

### Replies: 29 Views: 568

## \#1 Posted by: Superflim Posted at: 2018-11-29T20:14:14.575Z Reads: 166

```
Hi esk8ters,

I connected this switch to my battery and it shorted. Didn’t read the instructions very well because afterwards when I checked what I did wrong, I came to the conclusion that I had to connect the physical push button to the anti spark. Now I think it’s toast but I’m not sure. Here’s a picture
 ![image|375x500](upload://h6QuQReacVS5UX20lk1fn2ujlFu.jpeg)
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-11-29T20:24:08.850Z Reads: 156

```
Does it start smoking when you plug it in now?
```

---
## \#3 Posted by: Superflim Posted at: 2018-11-29T20:31:30.507Z Reads: 155

```
I would have to check. Don’t have my tools out right now
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-11-29T20:34:36.025Z Reads: 156

```
Those switches tend to be really finicky. It is very common for them to fail and quit stopping power.
```

---
## \#5 Posted by: dareno Posted at: 2018-11-29T20:43:02.066Z Reads: 151

```
Sure it wasn't just a connection spark?  The switch shouldn't matter whether its plugged in or not.  You just won't be able to turn it on obviously.  Put it all together and try again.  Just be ready to unplug it quick if it is faulty because they can combust.  As @Trdolan03 says those antisparks are a pain in the arse tbh.  If its gone look at the flier 300a version.  
https://www.ebay.com.au/itm/300A-Power-Switch-16S-Flier-for-HV-ESCs-/263111954651

Bane of my life antispark switches.  This one looks promising though.
```

---
## \#6 Posted by: Superflim Posted at: 2018-11-29T20:47:15.597Z Reads: 137

```
Definitely, not a connection spark. 
It was a pretty big spark and the cables burned out between the bms discharge<—>anti spark
```

---
## \#7 Posted by: dareno Posted at: 2018-11-29T20:51:28.647Z Reads: 132

```
Don't connect it up again then.  :grimacing:  Its a gonna.  They are so unreliable those bloody switches but the one I linked is the one the mighty lhb uses so should be a good option.
```

---
## \#8 Posted by: Trdolan03 Posted at: 2018-11-29T20:59:26.633Z Reads: 128

```
If you do want to purchase the one he linked go through alienpowersystems.com They have a great support system and will repair it if it goes bad. Shipping is also much quicker.
```

---
## \#9 Posted by: Acido Posted at: 2018-11-29T21:19:58.532Z Reads: 119

```
My failed, but didnt stop the power delivery instead it became one huge ressistor that cooked itself for an hour of full throttle lol
```

---
## \#10 Posted by: TreeFactory Posted at: 2018-11-29T21:32:10.648Z Reads: 111

```
I picked up an [100 amp](https://buildkitboards.com/products/100a-anti-spark-switch)  switch. I'm going to be running dual TB 170kv motors. I'm worried after seeing this that it will just fail out and torch my focboxes. Is this worry warranted?
```

---
## \#11 Posted by: dareno Posted at: 2018-11-29T21:48:07.098Z Reads: 106

```
![image|432x500](upload://8RW4rmK6rwvBjw0ducVqhJNcmKx.jpeg) 
![image|666x500](upload://72Ut4W9SOA2S1nv2khWj0VCOXnH.jpeg) 

I personally don't think 100amps is enough.  Neither of these are the bkb version but still.  Scary stuff.
I bought 3 switches so far from 3 different vendors and they all were the same luna unit with different stickers.  None of mine have combusted but still.  Keep it away from the battery to be safe.
```

---
## \#12 Posted by: TreeFactory Posted at: 2018-11-29T21:51:54.327Z Reads: 100

```
well that scares me. Maybe I should opt for a simple anti spark plug
```

---
## \#13 Posted by: dareno Posted at: 2018-11-29T21:58:44.613Z Reads: 100

```
Not all doom and gloom.  All mine have failed but not in a dangerous manner.  2 had fets that stuck open and 1 just died.  No pyrotechnics.  Keep it away from the battery and you should be fine.  Never a bad thing to have an antispark loopkey on your build though.
```

---
## \#14 Posted by: TreeFactory Posted at: 2018-11-29T22:01:56.169Z Reads: 99

```
would having a fuse before the switch help with not blowing it out?
```

---
## \#15 Posted by: dareno Posted at: 2018-11-29T22:32:26.656Z Reads: 91

```
Yeah if you have an inline fuse before it then yes.  Just make sure that the fuse is big enough to cope without being too big to be any use.  
Personally I don't use fuses on my driveline.  My current build has a gigantic bestech 100a bms wired for discharge and this takes care of that stuff.  It has a built in switch too.  Fuses can fail and I would rather damage the board components than me when hurtling down a hill and suddenly finding out I have no brakes.  Fuse from the battery will protect your vescs from frying and indeed the switch if you have one.  Cell level fusing on your battery will stop complete thermal runway on the battery itself.  You can take it as far as you want but while these things are dangerous,  if they are built with care and research there is no reason to be scared.  Use the switch because in my experience the switch is more likely to fail open than shut and this can save you.
```

---
## \#16 Posted by: Trdolan03 Posted at: 2018-11-29T22:36:56.501Z Reads: 86

```
[quote="dareno, post:15, topic:76530"]
Use the switch because in my experience the switch is more likely to fail open than shut and this can save you.
[/quote]

This 10 char
```

---
## \#17 Posted by: TreeFactory Posted at: 2018-11-29T22:45:04.077Z Reads: 86

```
i see what you're saying about the perks of having the switch fail over the fuse. I also have a besteck 80 bms for 12s lipos. I haven't completed my research of how im going to attach it just yet(i've got some posts and videos bookmarked for later). I like to error on the side of caution and have many fail safes in the electrical line rather than not. Something I've run into a bit on here is I'm building a mountain board and catch myself reading things that pertain to single motor longboards. Sense I'm learning this all from scratch I don't have full confidence that I've bought all compatible and efficient parts. My over all plan is to post the build in its entirety before connecting everything to see if people would be willing to review it. Thanks for heads up too.
```

---
## \#18 Posted by: dareno Posted at: 2018-11-29T22:50:01.650Z Reads: 88

```
Its always best to build to your environment.  I live in a very hilly area and am often hurtling down at 40mph.  On a downhill push board I would be ready to foot brake or slide but on my esk8 I rely on the brakes.  By the time you realise the brakes have failed it could be too late.  If you want help with a mountain board with lipos then summon andy87 when you want some advice.  Thats all he lives for lol
```

---
## \#19 Posted by: TreeFactory Posted at: 2018-11-29T22:55:18.540Z Reads: 86

```
I've had a few conversations with Andy87. He's been very helpful. I decided to go with the mountainboard due to the environment I'm in (Michigan. where the potholes eat you alive and the snow is plentiful). And oh boy 40mphs on a board. I think i'd crap my pants.
```

---
## \#20 Posted by: Trdolan03 Posted at: 2018-11-29T23:15:05.219Z Reads: 86

```
@TreeFactory I also have a mountainboard if you need help on your journey. :slight_smile:
```

---
## \#21 Posted by: TreeFactory Posted at: 2018-11-29T23:20:33.361Z Reads: 80

```
Awesome! Defiantly will keep you in mind. I'm 97% sure I will have some other questions down the road.
```

---
## \#22 Posted by: Trdolan03 Posted at: 2018-11-29T23:29:02.902Z Reads: 78

```
Most likely. I am working on my 5th board. Definitely always room for improvement. ;)
```

---
## \#23 Posted by: Fiori Posted at: 2018-11-29T23:32:32.409Z Reads: 83

```
Do it. You wont regret it. Anti-spark xt-90 Is less than $3, never fails, and can handle way more current than we will ever use. 
 
Plus, then your board has a KEY. I mean how cool is that?! I love knowing that regular people couldnt even figure out how to turn my board on :stuck_out_tongue: 

![sparky|500x500](upload://qTfCFEBbeJllD5O0LZ0iEyt5bVX.jpeg)
```

---
## \#24 Posted by: mmaner Posted at: 2018-11-29T23:39:14.592Z Reads: 75

```
This is a pretty good price on the Flier 300a...

https://www.alibaba.com/product-detail/Flier-16S-300A-power-switch-for_60768819667.html?spm=a2700.7724857.normalList.1.43c51df1raLrw9
```

---
## \#25 Posted by: TreeFactory Posted at: 2018-11-29T23:40:54.058Z Reads: 76

```
Agreed. It brings a personal touch to the board. Kind of like the scene from mad max fury road when she has to show how to get her truck started with a series of switches. At this point between the anti spark switch, anti spark key and bms there's gonna be all sorts of buttons in order to get it going.
```

---
## \#26 Posted by: macncheese Posted at: 2019-04-10T01:10:01.988Z Reads: 55

```
Know where to get that flier, only need 1 minimum order is 5. Ideas?
```

---
## \#27 Posted by: mmaner Posted at: 2019-04-10T02:20:20.813Z Reads: 51

```
Check with @longhairedboy, here used to use them.
```

---
## \#28 Posted by: longhairedboy Posted at: 2019-04-11T16:10:59.184Z Reads: 40

```
I order 5 at a time too, but not anymore. Using Unity and eliminating the discreet eswitch altogether.
```

---
## \#29 Posted by: AlanZhou Posted at: 2019-04-11T17:15:47.549Z Reads: 29

```
Https://www.eBay.com 😃
```

---
