# Tips on installing Torque boards dual hub motors?

### Replies: 14 Views: 1549

## \#1 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-03T15:05:33.269Z Reads: 182

```
So I've got the [dual hub motors 75KV](diy-electric-skateboard-kits-parts/electric-skateboard-hub-motor-dual/) coming in the mail any day now. I'm building a boosted clone with 10S4P. 

After reading [this thread](http://www.electric-skateboard.builders/t/psa-dont-buy-torqueboards-hubs/29000) I figured I should read up on how to install the motors properly. But it seems they don't come with instructions on how to install them. 

I've read a little and here's what I've gathered: 

* Use loctite on the screws that face inwards, to the center of the board. Wait 24h to let it cure.

* The screws that face outwards should already be locked in place with loctite. Can't hurt to double check though.

* Grind a flat spot on the truck so that the screw that holds the hub motor in place doesn't slide around. Use loctite on it as well.

Is there anything else I should know?
```

---
## \#2 Posted by: slerm Posted at: 2017-08-03T15:41:58.234Z Reads: 165

```
I'm probably the wrong person to ask since I wouldn't advise anyone use them since I did everything you mentioned, and still had screws back out, causing me to get pretty seriously injured. EVeryone pretends I loctited them wrong, but it doesn't take an engineer to know how to add locktite to a bolt and let it cure (mine sat for 3 days before I rode it, and it still backed out)

I also drilled a small pilot hole for the collar set screw to make absolutely sure it didn't slip. 

Hope you have better luck than I did. Trying to figure out what to do with them now
```

---
## \#3 Posted by: NickTheDude Posted at: 2017-08-03T15:51:14.643Z Reads: 157

```
Some of the grub screw holes for my set got stripped really easily so now I'm too afraid to use them with only 1 grub screw. Be very careful while installing them, what you mentioned is probably the best way to go.
```

---
## \#4 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-04T04:55:55.606Z Reads: 147

```
Yeah, I got a little scared when I read your thread.

So far you're the only one, that I've read about, who had a bad experience with them. But you had a catastrophical failure, I really hope something like that doesn't happen again.
 
I'll see if I drill a hole as well!

Cheers
```

---
## \#5 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-04T04:57:29.597Z Reads: 150

```
Thanks for the heads up! I can re-drill the hole and tap it with other threads if I accidentally strip it!
```

---
## \#6 Posted by: BigBoyToys Posted at: 2017-08-04T05:56:36.631Z Reads: 149

```
Before installing the hubs visually inspect them and spin them by hand looking for an issues  before you spend time installing something with an obvious problem.

U might notice that the hall sensor connector is smaller than the 2.0mm JST PH connector on the VESC. If you dont have the adaptor Dexter sells then you would want to cut and solder on the new connector prior to installing it. 

 Since we know that the screws on the backside do not come with loctite, remove those and apply loctite one at a time. They are quite loose to begin with. I put about an extra 1/2 turn on them from their original position in addition to adding loctite.

The hubs have two set screws onto the collar that slides over the ends of the hanger. I use a spring loaded punch ($5 at harbor frieght or ebay) to mark the two spots on the hanger where holes will need to be drilled. I tapped my holes with matching threads (m4x .7) but a slightly larger hole without threads should work fine as well. Drill one hole then install the hub and the set screw before marking the hanger for the 2nd hole to ensure your mark is as close to spot on as possible. Be sure to partially install the hollow axle nut while marking your hanger as well to make sure axle is centered in the motor. 

I use a little dielectric grease on the shrink wrapped section of the bundled phase wires where they exit the hub motor. This prevents the shrink wrap from binding on the hanger as you slide the hub onto the hanger which can short/tear/expose the sensor or phase wires.

Try to align the holes you drilled on the hanger with the set screw holes on the hub motor before sliding the motor on to the hanger to minimize any twisting you have to do for alignment once the hub is on. 

Once the motor is on the hanger and as close as possible to being aligned with the holes you drilled, hand thread on the hollow axle nut. Then install the set screws one at a time. 

If both screws align well enough, tighten the axle nut and check that there isnt any play and that the motor still spins freely.  If all is well, remove the set screws, apply loctite, then reinstall. Then remove the axle nut and apply loctite then reinstall. Its an aluminum nut so dont over tighten it.

Now repeat on the other side.

Hope these tips lead you to have as much fun with these as I am having.

Cheers!
```

---
## \#7 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-04T09:09:42.646Z Reads: 121

```
Great write up! I Will follow it to the dot, thank you!  :slight_smile:
```

---
## \#8 Posted by: NashNZ Posted at: 2017-08-07T14:43:42.537Z Reads: 108

```
Give us an update with how you get on, I'm thinking about picking up a set.
```

---
## \#9 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-07T15:03:48.822Z Reads: 103

```
Will do! I plan on making a video guide on how to put them on and a review as well.
```

---
## \#10 Posted by: NashNZ Posted at: 2017-08-07T15:13:56.602Z Reads: 101

```
Awesome! Cheers, bro. Looking forward to it.
```

---
## \#11 Posted by: BigBoyToys Posted at: 2017-08-07T19:31:02.035Z Reads: 85

```
I took my 4wd with these motors out for a test run last night. The board was breaking traction in the front during initial acceleration and it hit 39mph before I got the wobbles and let off. I think thats about the top speed on these in FOC on 12S though. Sensored FOC is feels like butter.
```

---
## \#12 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-07T19:57:37.170Z Reads: 84

```
Nice! I'm going to run a 10S4P on my dual setup. I'm a light guy(143lbs/65kg) so I hope that'll give me enough torque. 

From what I've gathered you and @torqueboards are the only ones running these in sensored FOC. Would you mind sharing your settings? 

I've only used BLDC on my first board but I'd love to run this new one on FOC since stealth is a priority.
```

---
## \#13 Posted by: BigBoyToys Posted at: 2017-08-07T20:40:48.432Z Reads: 81

```
I wouldnt recomend using my settings lol. They are on the edge to say the least, they'd knock your socks offf at 140lbs. Im literally double your weight. Set up is just as expected. Id say start with stock settings and use one of the foc tutorials on youtube. Then come back to the forum for tips on fine tuning to get improvements in the specific areas you desire.
```

---
## \#14 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-07T20:55:50.058Z Reads: 83

```
Haha you're probably right! Thanks for giving me someplace to start at least, I've been stuck reading post after post about it on this forum.

Cheers
```

---
