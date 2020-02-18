# Go Kart Frankenstein Build, Would like opinions

### Replies: 4 Views: 955

## \#1 Posted by: John_Doe Posted at: 2017-07-17T04:13:41.924Z Reads: 171

```
A little bit about myself, I come from a Robotics background, majoring in Programming and design (with a fair amount of build experience). I just recently lost my job (New management) and have been feeling down, so this project is a pick me up :slight_smile:. For reference I'm fairly small, five eight and weight around 150lb. 

Breakdown:
Chain driven electric longboard with an 11in go kart wheel as my rear wheel (yes a single) and normal longboard wheels (with shocks) as my front, 

The mounting frame for the wheel and the motor I will be custom making out of some aluminum stock I have lying around.

So here are the specs:

-1x 11.5 x 6.0-6 Dunlop slicks ($30 off eBay) 
-2x [190Kv 3150w 6374 DIY motor](diy-electric-skateboard-kits-parts/motor-6374-190kv-3150w/)
-2x [Multistar 6s 20Ah Lipo battery pack](https://hobbyking.com/en_us/multistar-high-capacity-6s-20000mah-multi-rotor-lipo-pack.html?___store=en_us)
-2x [HK Beast series 150A esc](https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-150a.html)
-The front trucks are currently cheepo trucks from my old longboard, gonna get an MB truck with inbuilt shocks. 
[Probably along the lines of this](https://www.mbs.com/parts/12042-mbs-pro-matrix-truck-black-1)
-If you guys are curious I am custom building the remote (one of my duties in my old job), having a friend of mine 3d print some prototypes rn. 

The gearing will be 1:5 (12t: 60t). The chain will be #35 (mainly because I already have the chain as well as the 12t sprockets for said chain :stuck_out_tongue:) 

*I should mention I am mounting the motors on either side of the wheel and chaining them individually to their own 60tooth sprocket on the wheel. This is for easy expandability later on if I want to add on 2 more motors for MOAR TORQUE!!!!

If you guys want I can post more details on how the wheel assembly is going together in the comments, but essentially imagine a go cart wheel assembly on the back of a longboard (When I was in high school I spent a summer servicing Go karts at my local Playdium) 

The only parts that are currently locked in are the wheels, sprockets, and chain as I already have those from previous projects/work assignments. 

So here is what I am looking for:
Are there any choices I made which I could get a better value else where? (Ex, I'm bounding between the DIY and the SK3 6374 motors, the difference being the DIY has a 3mm keyway, for which I have keys for)
 
What would you guys estimate my top speed, as well as my range to be? (I know use the calc.it for the top speed, but I want an experienced builder to give me an estimate, plus it can't do range(I have some rough numbers for range based on my experience, but that's from a completely different feild))

Will I have crappy acceleration because I am going to an 11in wheel rather than the standard longboard trucks or MB 8in wheels?(If so I am open to suggestions)

Should I go with 2 168Kv sk3's instead?

Also ESC vs VESC for my application, what are the suggestions?

Any battery suggestions? (will mine do, am I missing something here?)

Also, I'm all ears on suggestions for enclosures, I was known for shitty wire management and I can tell you, what I make generally works, I give it to the rest of my team to make it look pretty :stuck_out_tongue: 

I have a bunch of sketches to clear up some details if you guys want I can post them later on. Seriously, like 40 pages worth (Old habits die hard I guess). 

That's all, any help would be appreciated. (I will be ordering parts in early August and hopefully completing the build in early September)
```

---
## \#2 Posted by: Cobber Posted at: 2017-07-17T07:38:01.151Z Reads: 123

```
[quote="John_Doe, post:1, topic:27827"]
What would you guys estimate my top speed,
[/quote]

Try the calc [here](http://calc.esk8.it/) bro
Your batteries look heavy, but I get 44km/h and weighted 37km/h

Might need a lower Kv motor for such a big wheel w/5:1 gears...

What "X"C is the ratting on your batteries? I have 65C Amp ratting on the ones for my current build so I can thrash the hell out of my board without sag...

Not sure about your ESC, most here go for a VESC, it has lots of adjust-ability. That said I have two 160/200 Amp aeroplane ESC's for my current build... you know for science.

As for enclosures, I'm going utilitarian, and using something like [this](http://www.b-w-international.com/product/type-500/) for my batteries. Check out the for sale section, members who have stuff like covers for sale or group buys pop up there often.

Lastly, your ESC is only 6s, maybe thats all your after, but you will be pulling big Amp numbers at such low voltage. Might be easier to get higher power with a higher cell count (more volts). I'm going 12s, but 8 or 10s might be a better choice depending on your final ESC choice.

Some times you save money in the long run by buying better components, some times you over engineer. I like to err on the latter.

I see you haven't racked up much reading time yet, some of the more seasoned members will wait till you have put in a few more hours reading till they contribute. Or will suggest you use search before posting...

The whole thing sounds a bit good crazy ;) Not sure how your back wheel will work, look forward to seeing what you come up with.
```

---
## \#3 Posted by: John_Doe Posted at: 2017-07-17T12:00:03.831Z Reads: 86

```
Thanks for the advice, tbh I have more hours on here than my acc suggests (long time prowler I guess). 

Understand if I want to go for a VESC I would need much higher voltage (lower current draw). Any suggestions on where I can get good 10S - 12S batteries? (i could just link my current setup into a 12S). The batteries can definitely handle the current draw at 10C each can output around 200A. With some rough calculations I will be pulling max around 140A per motor, but that will be if im saturating it. 

I'm looking into lower KV motors, say somewhere in the 160s. But Im looking for keyed shafts, in the past I've had some bad experiences with grounded flat with a set screw and lock tight.Any suggestions? 

I agree with you on pushing for quality upfront for longevity. My budget is flexible and am willing to increase it to meet my goals.
```

---
## \#4 Posted by: John_Doe Posted at: 2017-07-17T12:00:45.024Z Reads: 85

```
To clarify, I made the account recently, have been "researching" (jealously looking at builds) for a while now.
```

---
