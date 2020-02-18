# One or two motors on a Evolve GT clone?

### Replies: 15 Views: 1430

## \#1 Posted by: jga Posted at: 2017-01-12T20:19:38.725Z Reads: 163

```
I am considering building a board similar to the Evolve GT AT essentially for commuting. I do not have any big climbs on most of my routes. My wheels will probably be 7 or 8".
I don't need to go quicker than 30 km/h but I would like to have something like 20Km autonomy with the battery.
Do you think I could reach these objectives with a single 190Kv SK3 and a 10S 10A battery? Or do I need to go straight away to two motors?
Thanks
```

---
## \#2 Posted by: sl33py Posted at: 2017-01-12T20:45:51.453Z Reads: 159

```
big wheels and mileage is tough to calculate.  I know that w/ "regular" sk8 wheels we get typically 10wh=1km.  Depending on terrain (hills), weight of rider, and riding style (racing or hauling ass starting off) - all will decrease range.

So - no hills?  check.  Your weight?

Battery - if you want 20km range?  Can you clarify 10s 10Ah battery?  Any specific one - because the C rating of the battery or similar detail will help us figure out your performance and potential range (if someone w/ offroad wheels can chime in?).

HTH - GL!
```

---
## \#3 Posted by: jga Posted at: 2017-01-12T20:51:41.746Z Reads: 143

```
My weight: 80Kg ... ok, it's winter, maybe 82 :wink:
I was thinking of 2 x 5S Lipo, not bought yet so choice is open. My actual constraint is that I will need to take them on a plane so I need a split.
```

---
## \#4 Posted by: Okami Posted at: 2017-01-12T21:11:04.972Z Reads: 128

```
I think you need a battery which has around 400wh of capacity-energy. 

This is taking into consideration that the average consumtion per km could be around 20wh/km.
The lowest I've seen has been 15wh/km, I think @whitepony claimed this energy usage for one of his early Evolve boards (dont know which one was it) - but I think it could have the 7'' wheels.

A friend of mine in lithuania said he gets about 22wh/km with dual drive.. So I think you should stay around this number unless you plan to do off-road, where the consumtion may go way higher..

---

If you're not good with battery technology and words involved, 400wh battery would be around 11ah, if rounded. At least that's how it is theoretically calculated (3.6 x 10 = 36v nominal, 400wh / 36v = 11,11 ah) 

//400wh = 20wh x 20km.

Though, I have no tested fully the theoretical vs practical (real life) energy, but it seems you should be good with around 10-12ah pack at 10s. (better of course to get a bigger one, especially, if you intend to use bms or have higher consumtion etc)
```

---
## \#5 Posted by: jga Posted at: 2017-01-12T21:25:38.217Z Reads: 107

```
Ok, thanks, I will start on this basis.
I should be able to go for a second motor if it's not good enough after a while, but I wanted to start with something simple first to see how it goes.
If anyone has other inputs/experience to share, do not hesitate to jump in.
```

---
## \#6 Posted by: Okami Posted at: 2017-01-12T21:39:18.678Z Reads: 103

```
I could only advise to post your battery - distance related question in another topic, where the topic is more dedicated to the distance.. not a lot of ppl will know you ask about batteries and distance.. unless they open and read all what you wrote ;)
```

---
## \#7 Posted by: jga Posted at: 2017-01-12T22:02:18.570Z Reads: 99

```
Yes, I know, but my original question was actually on single motor or not. With the battery I know I can increase the Ah if I want to go longer, but if one motor only pushes me at 12km/h it''s not really worth it. I currently have a Yuneek E-Go which is not too bad but the limit on speed can be a bit frustrating.
```

---
## \#8 Posted by: Okami Posted at: 2017-01-13T08:49:00.372Z Reads: 105

```
At 10s i think you should not worry about the speed at all. It is tricky with 6-8s where you cannot go with very high gear ratio (no 1:5 or more) or low kv motors (140kv would suck in speed probably, unless gearing is adjusted).

There is this calc: 
http://calc.esk8.it/

If you know your future parameters you can play with the numbers.

 Use google to find out much cm is 7 or 8inch tire. Efficiency leave at ~85% at least this number works ok for me, some (lighter ppl) can perhaps use even 90%.

---

<img src="/uploads/db1493/original/3X/f/b/fbcc66aa55304a457e30fd144f6363b095b1ba3f.png" width="690" height="358">

I think you will even get a few more km/h while the battery is fully charged. The thing with batteries is that once you start deplete them, the max speed also decreases a bit (since the voltage gets lower, too).

Anyways, as you can see, with 190kv motor you dont need to worry about the speed at all. If you had 140kv that would be more tricky. Plus, you need to put into consideration - where will you get your parts?

This will influence your choice and options on gearing ratios. It is hard to get very small motor pulleys for belt drives (15mm size).

One more consideration is - will you use lipos or make / buy Li-ion pack? Li-ions usually have - are set to charge to a bit lower voltage - more like 4.1v but they also have better longevity compared to lipos..

---
 Once more about the speed, I would tell, that it is better to go with at least 35-40kmh max speed, even if you are a beginner like I was. There will be times when you will have straight road and no obstacles and you will probably like the feeling of pushing the board till its max.. so yeah 30+kph is probably the minimum max speed for the start :)

--

Cannont comment much on choice about dual or single.. im running only single right now, there are times when 2 motors might give you ''a nicer feeling'' but generally one motor works pretty well and unless it is 50'' or something size (for single driven emtb), it should work quite ok! (usually ppl use 6374 / 6364)
```

---
## \#10 Posted by: jga Posted at: 2017-01-13T12:23:41.355Z Reads: 81

```
I think I will use what I ordered in December for the conversion of my other board, which is: 10S4P Li-ion with BMS, VESC, Vedder anti-spark. I will add to that an SK3 6374 190Kv and probably Hypa or Superstar wheels.

The last interrogation I have, and I don't know if the topic is addressed elsewhere, is whether I should use skateboard or mountain board. trucks
```

---
## \#11 Posted by: Okami Posted at: 2017-01-13T12:29:21.891Z Reads: 81

```
Well, you need to check the lenght of the axles.. skateboard/longboard axles might not be always long enough to acommodate the wheels. I dont know the proper sizes but you should check how long is mountainboard axle vs longboard one..

Or.. if you meant trucks itself - whenever springs or bushings.. I've only got experience with skateboard trucks, the steering is not that great (at least for my board) but at least it is not wobbly. 

On the other hand, spring trucks seem to be more easly adjustable, especially if you can move the spring location.. They also seem to be more ''turny''.

--

@jga Have you found your source for pulleys / mounts also?
```

---
## \#12 Posted by: jga Posted at: 2017-01-13T12:38:25.256Z Reads: 76

```
I have ordered the motor mount from Idea, more designed for MB.
I think the Trampa trucks should be large enough, whether skate or MB type. I know that when I am landboarding with my Scrub board it is not very stable, so I would tend to go for skate trucks. 
Would there be a difference on the height of the deck (ground clearance) between the two?
```

---
## \#13 Posted by: Okami Posted at: 2017-01-13T12:40:16.553Z Reads: 79

```
oh cool, did not know you've got scrub board already.. Which one do you have? I assume you have one with the spring trucks, is that right?

Yes, trampa should be good :) Im not sure about the clearance.. The only difference im seeing is that for skate trucks there are risers.. not so much for spring trucks it seems.. (unless you make your own). 

Though, i would not put a very big/high risers for skate trucks anyways.. they just make the board wobbly and not so stable..(even if turning improves..)
```

---
## \#14 Posted by: jga Posted at: 2017-01-13T12:51:13.036Z Reads: 72

```
It's a Scrub Regolith, but the motor is currently Flysurfer Speed 3 :sunglasses:
Yes it has spring trucks
```

---
## \#15 Posted by: Okami Posted at: 2017-01-13T13:19:27.580Z Reads: 75

```
@jga What deck will you choose for your board (the one you gonna make electric, similar to evolve AT) ?

Well, at least now I know that these scrub spring trucks are not that stable (so it seems)..

---
If talking about deck/board choice..


I ''eyed'' furnace creek board for a while, since it had spring trucks also.. though before seeing scrub furnace creek I already bought myself ''silver reef series II'' 

The downside - it is quite springy/flexy.. 

So actually not that great choice of a deck for emtb! Also considering that it has huge 9inch primo striker wheels.. which is actually no so great for commuting/riding in the city. 

Other than that I really like the deck shape/colour of my current board - silver reef, too bad it is quite long.. that is part of the reason why I am searching for options to make the deck size smaller without making compromises..
```

---
## \#16 Posted by: xBRAZILx Posted at: 2018-01-30T00:36:55.873Z Reads: 34

```
have you been running a single motor since day one that you build your esk8 or did you run with two motors in the past and nowadays you are running single?

if you ran with two motors and now are running with one: 
did your top speed change? 
did your motors run more cooler? 
did you have more range?
did you have more torque?

i am question you because i always see almost everybody saying that is build a esk8 with two motors.
i have a setup with just one, and i can reach 30kmh top speed (which is already dangerous).

thanks for the answer
```

---
