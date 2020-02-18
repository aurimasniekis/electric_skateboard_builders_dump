# Tight budget 1st build &#124; 6374 190kv &#124; &ldquo;sleeping lion 120A&rdquo; &#124; 8S LIPO &#124; SPARKLE

### Replies: 6 Views: 1250

## \#1 Posted by: jbalint1122 Posted at: 2017-11-01T15:31:44.428Z Reads: 180

```
Alright. This will be kind of a long story anyway, so why not start with the beginnings. :wink:

I think many of us got to know e-skateboards from Casey Neistat. When I first saw him riding it, back in 2015, I immediately looked it up and knew I would buy it until I saw the price. After that, I tried to get it out of my head, because it was WAY out of my price range.
After maybe a year or so, I started seeing other e-boards on the market like Evolve or Stary. Some kickstarter boards were even getting close to being reasonably priced (for me at least). :sweat: 

From November 2016, I was always on the hunt for the perfect board, but sadly I asked for too much.

It was January 2017, when I accidently found this forum. From that point, I started to believe that what I wanted, might be even possible!

This was my wish list for an electric skateboard:
-	Have the range of at least 6-8 km
-	Be fast!
-	Be well priced. (I had like [€400 / $480 / £370] back then).
-	Be good looking
-	Be able to fit it in my locker at school
-	Be able to go over rough terrain. I live in Hungary, and roads here are catastrophic…

The first idea I had, was to build a dual drive mountainboard, and ride next to the cars on the road. I basically wanted a board like @squad had: (https://www.electric-skateboard.builders/t/diy-trampa-long-35-e-mtb-dual-vesc-six-sensored-emax-gt5345/2474) I even went as far as asking (more like begging) him for the templates that he used for his motor mount. Amazingly, he was kind enough, to give me the templates, even though, he must have put serious work in it. :slight_smile:

But even if I made the motor mount “myself” costs would still have been way too high…
No matter how bad I wanted it, there were (and are) just too many disadvantages of a mountainboard for my application:
- It would have been really heavy.
- $$$$$$$$
- If the struggle wasn’t bad enough already, I found out that using an electric vehicle on public roads is illegal in Hungary… :sob:

So my only option left, was to stay on the sidewalk. And for that, a monster like a Trampa, would be overkill. 
I had to make a compromise: I decided that I will make an e-board with mountainboard components, so I will have a “compact” board for commuting, and if I get some money in the future, I will build a mountainboard. This way, I could build two boards for one’s price (if the actual skeleton of a mountainboard doesn’t count). The only disadvantage of this concept was the fact, that every time I would want to switch boards, I would have to take them apart, and switch the components. I don’t know how much would I hate that, but at the time it seemed like such a good idea. :grinning:
--------------------
It was late February when I made my first purchase. After a long chat with @WARMAN , I bought:
- A Turnigy Sk3 6374-192KV motor
- Caliber II trucks
- An Enertion mount with belt and pulleys
-  A Gt2b transmitter with receiver 
From this point, there was no backing off.

This purchase was quickly followed by buying the ESC from @barajabali , and again, I was going to make an e-MTB so a regular VESC wasn’t going to be enough (I really couldn’t afford blowing up one). I bought an FVT 12S HV 120A “Sleeping lion” ESC, which @squad , and @idea were using for their e-MTBs. This looked much more “solid”, than a “VESC 4.something”.

Batteries were next. (Of course I had to go Lipos because of price…) I decided on 8S, because if it is made of two 4S packs, it is easily upgradable to 12S with an extra pack (Again, I was having that MTB in my mind).
These were the ones I went with: 
https://hobbyking.com/en_us/turnigy-graphene-5200mah-4s-15c-w-xt60.html?___store=en_us

Wheels were a hard question. I needed them to be big (rough roads), but I was starting to run out of money, so MBS all-terrain wheels were too much. I ended up with some 97mm flywheel clones:
https://goo.gl/PKL977 (this link was incredibly long)

After that I bought a small skateboard (only for the deck itself, it was pretty cheap…) that could fit in my locker:
It is [68,5 cm / 27 inches]
<img src="/uploads/db1493/original/3X/9/6/9649dd0414808481973314b74609e4f519460529.jpg" width="500" height="500">
 The small stuff:
I ordered wires, connectors and an anti-spark plug from the trusty bannggood and Loctite and an ABS sheet for vacuum forming was ordered from ebay.
When I got everything, I put things together as fast as I could. Vacuum forming could wait…:  
<img src="/uploads/db1493/original/3X/6/6/66834d75b0547773a3adef3244d903750319c89d.JPG" width="690" height="449">
<img src="/uploads/db1493/original/3X/4/d/4dd5f29d8f426ee6b3d85748335df73e4c4e3aff.jpg" width="666" height="500">
This was the time problems started to arise. It was instable. Firstly, I thought it just needs some getting used to, but after one or two charges I realized that this much power with this ESC on a small board like this is not controllable. Startups were the hardest. Every time, I had to concentrate to move the trigger as slowly as I possibly could. 
I had the idea, that maybe if I had a slightly bigger board, I would have more stability. So I measured my locker in school, and I was surprised how big it actually was. It was [90 cm / 35 inches].

I decided that I will get a deck that is close to that size. Only problem was, that I had only like [€33 / $40 / £30] left. After a long seek, I managed to find a used board for that money. It was about the right size, and I liked the look of it. :grin:
<img src="/uploads/db1493/original/3X/9/b/9bd65948d7ebb60fc564522cafe503dcdc199cd2.jpg" width="690" height="430">

----------

This is the time for a bit more detailed build thread:
(This was partly done before I got the longboard…)
## Step 1:
I made a lead that connected my batteries in series, and added a female XT90 connector on the positive wire as an antispark plug:
<img src="/uploads/db1493/original/3X/4/c/4c8b1a7ed621e65c6683375b0ff1458d1f338dd8.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/8/8/88aa357a9cad37e818a598cd307f67af446a7472.jpg" width="666" height="500">
## Step 2:

I soldered it up to the ESC, which was a pain in the butt, as I didn’t want to remove the heatsink. I ended up soldering only the ground wire on, and soldered the positive lead to the small wire that was coming out of the ESC (all solder joints came out nice, and IMO they can safely carry 120 Amps).:
<img src="/uploads/db1493/original/3X/2/7/27bb3833163159cad1f07c1f822b350b3a253646.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/d/4/d49b02176c66521939572b5f1ceb87d797079e0b.jpg" width="374" height="499">
## Step 3:

Enclosure time! Now this was a hard question… Vacuum forming was clearly my only option. It costs like nothing. Only problem I had, was the vacuum part. I don’t have a shop vac, I could have only useed my family’s vacuum cleaner. After some thinking, I realized that this machine probably won’t generate enough suction for my enclosure, and the last thing I wanted was to kill both the vacuum cleaner, and have an unusable enclosure…
So I came up with something different: “Vacuum forming without a vacuum”, so maybe just “forming”:

## Step 3.1:

I made the form. Nothing fancy.
<img src="/uploads/db1493/original/3X/e/9/e93a5279e704cb1114a5fd6a069ecb44f7d1146c.jpg" width="375" height="500">
## Step 3.2:

I made the frame form two sheets of wood, to hold the sheet of ABS together. Using this method, the inner part of the frame should be cut out in one piece. Where the cut is made, there will be the starting point of the ledge of the enclosure (where you can screw it onto the board)
<img src="/uploads/db1493/original/3X/3/e/3ea0b2c46255e4eaa4a5f54cbf86018628b14b44.jpg" width="374" height="499">
<img src="/uploads/db1493/original/3X/7/d/7d556083f97a1fe75324790afe150a646732290a.jpg" width="666" height="500">
## Step 3.3:

I mounted the form (made in step 3.1) onto the cutout of the frame.
<img src="/uploads/db1493/original/3X/2/f/2f8fa08a36413d679a94ef8d61c71c13dc6ea40d.jpg" width="375" height="500">
## Step 3.4:

I mounted the whole thing to a big piece of wood to prevent slipping. And also drew a few lines for better accuracy.

## Step 3.5:

I put the piece of ABS into the frame and screwed it together. I also let the screw get through the ABS.

## Step 3.6:

I put the frame with the ABS sheet, in the oven. (I know it isn’t the healthiest thing to do, so if you have other options, please use them. Also the temperature of the oven was about [150 degrees Celsius / 300 degrees Fahrenheit])

## Step 3.7:

I got it out when I saw the ABS melting, and pressed it onto the form. Kept it there for a minute or so, and the enclosure was made! :sunglasses:
<img src="/uploads/db1493/original/3X/8/c/8c00f921fff96e02890e5634fb55bc0b3277f5cc.jpg" width="666" height="500">
## Step 3.8:

I drilled out the holes for the motor wires, the ESC, the XT90 and the charging cables.
<img src="/uploads/db1493/original/3X/3/2/3223ea40d9bca624d16d73d4cf3a7108f794a6e5.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/d/9/d9b928f16fbf0e26e8ea58fa8c462d3d5003cf2f.jpg" width="374" height="499">
## Step 3.9:

I cut the enclosure to size.
<img src="/uploads/db1493/original/3X/0/2/02ebf4305ec6f1c976cb7a1a94b44d32035aa118.jpg" width="375" height="500">
## Step 4:

Putting it all together! Everything fitted nicely. One thing, I thought was kinda smart was that I used ties, to make the motor wires the perfect size.
<img src="/uploads/db1493/original/3X/0/f/0f5a3aca321d134749c9b0205daea51bd00668b3.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/2/4/24136e07456f7f96e5a62f429688a89e565c9a09.jpg" width="463" height="500"><img src="/uploads/db1493/original/3X/1/a/1af4aed4fe427e4d55eb2f77968a54d750cbda14.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/f/d/fdef7a3d9c7ba49001ae0272d90172ed04a1fcf4.jpg" width="374" height="499">
## Step 5:

Tape it up and take it out! I quickly fixed the enclosure to the board with some insulating tape, and took it out for a ride. It was great! This bigger board gave me a lot more control and balance. (As I hoped it would)

## Step 6:

Screws in! Nothing fancy, just some screws. One future upgrade I can think of, would be to replace these with black ones. Sadly, my local hardware store only had these.
<img src="/uploads/db1493/original/3X/3/5/3547e6463199f42f8b3a3237c275e8ba34f42a88.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/f/e/febf73617612262ca01581066019bb68e3b7a232.jpg" width="666" height="500">
## Step 7:

SPARKLE!!!
The main thing that irritated me, was that I needed both hands to carry my esk8. One for the board and one for the massive gt2b. So I found a friend with a 3d printer, and made @okp ‘s Sparkle mod. There is plenty of information about this so I won’t go into it.
<img src="/uploads/db1493/original/3X/2/b/2b6b39702d153c41e900e56b77d554d72dad67f8.jpg" width="374" height="499">
------------
The board was finally done. After 10 months of continuous research, more than 100 hours of reading on the forum, it is finally done. :heart_eyes:

Sorry for the low quality pictures, I have a crappy smartphone. I’ll try to get some better pics of the finished board in the following days…


----------

Thanks to these guys for answering my stupid questions, and helping me solve problems:

@okp - Thank you for the inspiration, the replies and the Sparkle mod! You sir, make some of the nicest boards! :wink:
@barajabali - Thanks for the ESC!
@WARMAN - Thank you for your massive patience and your honesty!
@kovjanos - Thanks for your time, and I’m sorry I didn’t buy your stuff…
@squad - Thank you for sending me the PDF of your mount. I’m thankful for it, even if I didn’t use it.
@esk8 - Thanks for the private chat in Hungarian!
@okami - Thanks for your time, knowledge and the long replies!
@sl33py - Such great advices! Thanks for your time!
@Namasaki  - Thanks for helping me solve my ESC problem!

I'd mention more but this is the max. :sweat:

This forum is full of constructive, helpful and kind people. I would be nowhere without the help I got!:grinning:
_____________________________________________________
Please share your opinion, ideas and thoughts down below. Also, if you’ve got any questions, feel free to ask me.
```

---
## \#2 Posted by: blastouz Posted at: 2017-11-01T15:58:16.900Z Reads: 118

```
Nice build, what are the specs (range, speed...) ?

Did you make a hole for balancing ports ?
```

---
## \#3 Posted by: jbalint1122 Posted at: 2017-11-01T16:11:03.764Z Reads: 111

```
Max speed is about 36km/h / 22m/h. Range is about 12km / 7.5 miles. Yup, there are holes for the balance connectors too.
```

---
## \#4 Posted by: WARMAN Posted at: 2017-11-01T16:32:50.978Z Reads: 110

```
Well done balint,patience and perseverance payed dividends! When I was reading through I thought there's no way he's riding round with that much power on that little board! Lol btw your English and spelling is very good!
```

---
## \#5 Posted by: jbalint1122 Posted at: 2017-11-01T17:03:28.170Z Reads: 106

```
Thanks! (I've been learning English since primary school) 
Maybe with a VESC, it would have been more stable, but with this ESC, that little board was like balancing on a toothbrush sized rocket. :joy:
```

---
## \#6 Posted by: okp Posted at: 2017-11-01T17:07:17.643Z Reads: 97

```
nice man ! enjoy the mod !!!!
```

---
