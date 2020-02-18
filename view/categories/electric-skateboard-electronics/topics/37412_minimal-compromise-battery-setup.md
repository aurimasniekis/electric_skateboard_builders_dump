# Minimal Compromise Battery Setup?

### Replies: 26 Views: 1678

## \#1 Posted by: Youssless Posted at: 2017-11-05T13:01:49.615Z Reads: 223

```
Howdie,

Wanted to bounce some ideas around and see what direction I should go.

I love my board and looking to upgrade it to a dual drive with killer range... Except I have an addiction to punching the throttle on the empty roads I encounter here in London (they exist!).

I know the pros and cons of Lipos vs Liions but I'm after a solution that minimises these compromises they have.

There have been topics about huge capacity Lipos (such as 22Ah Gens Ace Tattus or Overlander 22Ah batteries) and these would really work great for range and reducing voltage sag. However, having an 8Ah 9s setup myself I've noticed that (after about 200 miles) my acceleration has dropped and so has my top speed (35mph to about 28mph now) and I'm assuming that's due to the reduced C rating my batteries have had over their usage? Not sure if its my VESC settings but that's besides the scope of this post. 

So I'm toying with the idea of Liions but even a big pack (12S8P) would still suffer from a lot of voltage sag with how I ride.

Should I just stick to high capacity 25C Lipos? Are there alternatives? The kicker is I want to keep everything under the deck (40" stiffy).

Thanks for your input. 

Youssef
```

---
## \#2 Posted by: Hummie Posted at: 2017-11-05T18:59:22.487Z Reads: 187

```
Surprising drop in 100 miles. I think range would suffer but not discharge ability

Li-iron cells maybe.  The red headway cells
```

---
## \#3 Posted by: Idle Posted at: 2017-11-05T19:26:02.378Z Reads: 173

```
What cells are you using?  

think you should test your cells and charger to find out what happened to them before pulling out your wallet.
```

---
## \#4 Posted by: thisguyhere Posted at: 2017-11-05T21:25:57.883Z Reads: 166

```
at 8p even saggy liion cells like the hg2 and 25r would no longer be an issue, since you'll have 160amp! available, which I doubt any setup will even be able to approach before melting the vesc down to molten metal
```

---
## \#5 Posted by: BigBoyToys Posted at: 2017-11-05T21:28:14.298Z Reads: 159

```
Agreed, a dual vesc wont sag a 12S8P pack. It will be awesome. Build it please.
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-11-05T21:31:16.743Z Reads: 157

```
what deck do u plan to use to fit a 10lb battery pack? 

or are you picturing a trampa board with the battery on the top center?
```

---
## \#7 Posted by: Youssless Posted at: 2017-11-05T21:50:10.784Z Reads: 153

```
@Hummie I did see a drop in range but I assumed it to be because I ride faster now. I also tweaked VESC settings to have higher motor and battery amps (80 each) and max Watts (1900) and I'm unsure if I pushed em too far.

@Idle they're 3x turnigy 3S 8Ah 30C batteries. They're all low resistance but I haven't checked how much capacity the charger gets them too as AFAIK that's not accurate.

@thisguyhere I was hoping to use 30Qs, they're rated to 15A each right? So 12S8P would give me 120A? Seems a bit low? I have a £50 9-ply maple deck that's quite stiff and w-concave. How much do you think I can fit underneath? I want to go BIG since liions are cheaper than massive capacity lipos...for science of course. I've a 70cm wheel base to play with (- space for 2 VESCs and a BMS). 

@BigBoyToys thanks, you answered a bunch of my questions previously and I know you push things. If you and @thisguyhere reckon its fine then I'll make the investment. How big do you think I can go?  I've a 70cm wheelbase to fit everything and I don't mind reverse mounting my morots...will get Carvons one day.
```

---
## \#8 Posted by: thisguyhere Posted at: 2017-11-05T21:57:43.416Z Reads: 138

```
[quote="Youssless, post:7, topic:37412"]
I was hoping to use 30Qs, they're rated to 15A each right?
[/quote]

30q are safe at 20a

https://www.e-cigarette-forum.com/forum/threads/samsung-inr18650-30q-15a-3000mah-bench-test-results.681259/

[quote="Youssless, post:7, topic:37412"]
So 12S8P would give me 120A? Seems a bit low?
[/quote]

no, 120a is way overkill. even chaka and lhb big ass packs are not even approaching those values. if u manage a 8p pack u may be going after the biggest pack record. 

in terms of fitment, you'll have to figure that out on your own
```

---
## \#9 Posted by: Youssless Posted at: 2017-11-05T22:03:19.703Z Reads: 129

```
Could have sworn I've read posts from last year that said someone already had a 12S8P.

Eitherway, I'm reassured and think I'll be going down the liion route for this upgrade. Thanks a bunch!

Edit: yeah I think @Ackmaniac has a 12S8P pack made of 30Qs. If so, how do you fit your batteries?
```

---
## \#10 Posted by: NickTheDude Posted at: 2017-11-05T23:32:59.952Z Reads: 117

```
How much range are you looking for? You could use lower capacity/higher discharge 18650s so you wouldn't need so many cells in parallel. A 12S8P of 30Qs would give you 160A discharge and 1065Wh which is like a 100km of range... I doubt you need that much.

These are good for 25A: https://liionwholesale.com/collections/batteries/products/lg-hd4-18650-battery-genuine-25a-2100mah-flat-top-wholesale-discount?variant=28023634769

And these for 30A: https://liionwholesale.com/collections/batteries/products/lg-hb6-18650-battery-genuine-tested-30a-continuous-1500mah-flat-top-wholesale-discount?variant=13978272644

To get roughly the same discharge as the 8P 30Q pack you'd only need a 5P of the HB6 and you'd still have around 30km of range.
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-11-06T00:17:18.064Z Reads: 111

```
Mine look like a doubled 12S4P. The cells are in sleds. The reason i went for such a big battery is because first i wanted to use harvested old laptop cells. And for that i had to use many of them in parallel because of the low current they can provide. But after a while i needed real power so i replaced them with the 30Q. 

And it's just awesome. You don't need to care anymore about your battery. Just simply go as far as you want because your legs will give up earlier. And it is still a very usable board. It weight's around 2,5 kg more than a 12S4P but that's it. It's configured as my speed board (long wheelbase, 60 km/h max)  for the road to do long distance stable and fast.

Some pictures of the old version of the battery can be seen here. The new one simply has the 30Q cells.
http://www.electric-skateboard.builders/t/10s4p-18650-build-using-vape-sleds/2092/56?u=ackmaniac
```

---
## \#12 Posted by: Hummie Posted at: 2017-11-06T01:35:21.541Z Reads: 99

```
But u have li-ion cells , and only 9s, and after 100 miles, and increasing the motor and battery Amps, you have a reduced top speed and acceleration I think u said.  
Id Get the vesc recording to see what Amps ur doing  and do more in series
```

---
## \#13 Posted by: GrecoMan Posted at: 2017-11-06T01:36:38.070Z Reads: 95

```
pshhh my 10s6p weighs 9lbs, 8p will weigh closer to 13lbs
```

---
## \#14 Posted by: PXSS Posted at: 2017-11-06T12:31:41.752Z Reads: 81

```
Each cell weighs 0.1lbs. +.5lbs of wires and stuff. 
My 10S4P weighs less than 5lbs. My 8S13P weighs 11 pounds
```

---
## \#15 Posted by: Acido Posted at: 2017-11-06T13:21:50.453Z Reads: 76

```
Longhaired boy did 12s9p i think
```

---
## \#16 Posted by: Youssless Posted at: 2017-11-06T14:11:47.659Z Reads: 75

```
I've been thinking and I'm trying to go over 1200 miles worth of excel spreadsheets and come to the conclusion that I've probably noticed a dip in speed for a large number of factors, namely:

1) higher wind speeds since I first started riding in the summer.
2) top speeds were achieved on still days that were very flat. 
3) A more gradual throttle curve at higher speeds means that I don't get the speed kick from 20+mph like I used to. 

So I'm going to spend some time performing tests to quantify things and control or eliminate as many variables as possible and see what I can conclude from that.
```

---
## \#17 Posted by: Youssless Posted at: 2017-11-06T14:13:10.335Z Reads: 73

```
Noice! I need to see this and take inspiration. Did some rough calculations and reckon a double layered 12s4p would fit under my board. Will see if I can tier a 12s5p and 12s4p together.
```

---
## \#18 Posted by: Youssless Posted at: 2017-11-06T20:08:19.517Z Reads: 67

```
Quick question:

1) How long does it take to charge?
2) What's your charging setup?
3) What does the latter part of 'Max. continuous discharge: 15A(at 25°C), 60% at 250 cycle' mean? Is it talking about max discharge?
```

---
## \#19 Posted by: Hummie Posted at: 2017-11-06T21:06:13.054Z Reads: 69

```
With question three for @Ackmaniac it sounds like li-ion do degrade their c-rating a lot after 250 cycles.  Cells lose capacity and discharge ability w cycles .  another reason to go li-iron. The red headway cells have a high discharge ability and I've seen video of people overcharging and shooting w a bow and arrow or a hacksaw.  No problem no fire
```

---
## \#20 Posted by: Youssless Posted at: 2017-11-06T21:11:09.814Z Reads: 67

```
LiFePOs don't lose C rating as much? Other than safety what other benefits do they have? I ruled them out previously because they're less energy dense and expensive
```

---
## \#21 Posted by: Hummie Posted at: 2017-11-06T21:15:42.658Z Reads: 63

```
I'll check the discharge ability but I remember it was pretty high and they have way more life cycles.  Comparing the cost vs energy expendable over the cell's life iron wins. Heavier n bigger. But the screw tabbed headway red cells I want

Just 10 continuous and 20 peak amps
```

---
## \#22 Posted by: Youssless Posted at: 2017-11-06T21:19:26.803Z Reads: 66

```
Lol as long as I can get 24Ah 12s under my board I'm open. Definitely possible with Liion, you know of a good vendor for LiFePO4s in EU?
```

---
## \#23 Posted by: Hummie Posted at: 2017-11-06T21:20:50.280Z Reads: 66

```
http://evcomponents.com/lifepo4-cell/headway-38120hp-8ah-lifepo4-cell.html
But I've never had them and 20 peak it says.
```

---
## \#24 Posted by: Youssless Posted at: 2017-11-06T22:18:46.247Z Reads: 67

```
Man, I really should check em out! 8Ah and 10C per cell? A 12S3P pack would do wonderfully! If expense and mass are the only significant downsides to these things then I need to sign up! 

Also, on a separate note, did some top speed testing, I hit 30mph and could have gone quite a bit faster but had a car come onto the road so had to slow down and tail it (15m back :smile: ).

<img src="/uploads/db1493/original/3X/f/9/f9622608d9d46d1375e41f5aec6f4646d2a51330.jpg" width="281" height="500">
```

---
## \#25 Posted by: Ackmaniac Posted at: 2017-11-06T23:47:38.140Z Reads: 52

```
Ok let's analyse your ride a bit and bring some light to the the continuous amps we use.
<img src="/uploads/db1493/original/3X/4/2/42a5d784b005e4179de87c6270db259f398c9b7f.png" width="390" height="441">

On the left side marked in red it shows the average amps when when the battery is really used. So when you just coast (no throttle and no brake) it won't be counted. In this case you used 16A of your battery.

But the more realistic value is the one on the right. It shows the average amp use while you are moving. So also coasting is taken into account. And in this case you only draw 9.8A from your battery on average.
So instead of 60A continuous (guessed you have 20A Li-ion cells x 3P) you only used 1/6 of that (17%). 
So they won't get hot and they will perform much better than 60% capacity left after 250 cycles. And you won't discharge them completely which gives you more lifetime and mostly you won't charge it with a standard charger to exactly 4.2V a cell. In most cases it is a bit lower (like 4.16 a cell) which gives you also more lifetime.

And why don't we hear here in the forum that a li-ion battery pack exceeded it's max cycles. Most of the times the BMS failed or nickel strips came loose.
```

---
## \#26 Posted by: Youssless Posted at: 2017-11-07T10:06:11.002Z Reads: 41

```
Thanks for the insight. 

So even at 60% max cont. discharge (which I'd imagine is a cautious number) I'd still have enough amps on a 12S8P pack. Moreso if I stick to a 4.1V-3.6V range.

The downsides seem almost negligible in this case but I'm still tempted by LiFePO4s for extra life. I don't mind extra weight since I'm about 105kg with my gear on so hauling an extra 5kg won't be too taxing.
```

---
