# Complete battery noob needs help

### Replies: 6 Views: 1193

## \#1 Posted by: rainbowbolt Posted at: 2016-07-12T17:55:20.357Z Reads: 106

```
Hey guys, I'm sorry for imposing on you like this, I should probably have stuck with a pre-prepared battery.

But here I am with all the parts on the dinner table and I don't know what exactly to do with them.

So far I have:

1x iCharger and power supply
1x hobbyking charging board with 4mm and balance
4x 3s Zippy 5000 mAh LiPo with 4mm bullet connectors
3x Series adapter for said bullet connectors (with this I can get them together for 12s, right?)
2x VESC from hellray.de (connected through the CANBUS)
1x TB mini remote
2x TB sensored 230kv motors

Attaching the motors to the vesc is easy enough, however, I have no clue how to attach everything together from the battery end. Help would be greatly appreciated.
```

---
## \#2 Posted by: rpn314 Posted at: 2016-07-12T18:16:31.677Z Reads: 102

```
Couple of question so I can figure out how to best help.

1. What charger and charging board do you have exactly?
2. Were you planning on putting the 4 zippys together end-to-end (in series) to get a 12s pack for when you're riding?
3. Were you planning on charging the packs as 1 big 12s pack, two 6s packs, or four 3s packs?
```

---
## \#3 Posted by: crameur Posted at: 2016-07-12T18:24:09.250Z Reads: 103

```
Hope this will help you, use XT90 and a XT90 antispark to the ESC
http://www.electric-skateboard.builders/t/solved-how-to-put-4-batteries-in-series/5825
```

---
## \#4 Posted by: sl33py Posted at: 2016-07-12T18:45:19.650Z Reads: 99

```
@rpn314 has some good questions.

A couple things to note - you _cannot_ run those motors (230kv) @ 12s on your VESCs.  VESC only supports 12s with motors <200kv.  You will kill your VESCs if you try.

You can run your 3s packs in series x 3 for 9s - that should work really well for you.  I ride regularly on 8s without issue and i'm a big guy.  Especially w/ dual motors = lots of power!

iCharger chargers are my favorite.  I have the 306b if you have any specific questions on them let me know.  I'm sure i can help with 206/208/308 as well depending on model you got.  What power supply did you get to power your iCharger?  I have a couple - from a 600w variable output, to dual dell server 750w in series for 24v.

what motor mounts, wheels, and gearing do you have?  How much do you weigh, and what kind of riding are you planning (flats, hills, etc.)?

recommend a loop key or anti-spark loop key as the simplest way to connect your batteries and disconnect them when not riding:
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

If it's helpful i can show you pics of a few boards i built - so you can see how i wired and placed everything?

First board test setup (painters tape for the win!):
[img]https://lh3.googleusercontent.com/-DU7V3W_5PLU/Va3n4cktyqI/AAAAAAAAspw/r1hULPvT0_s44CwTggbNTM2rSw752YlJwCCo/s1600/2015-07-19%2B12.32.22.jpg[/img]
(Battery (single 6/8s 8Ah iirc) --> Watt Meter (unneeded, just for info) --> VESC (w/ GT2b Rx next to Watt Meter) --> DIYes 5065 200kv.  Paris 195 trucks (eventually used on other board in dual rear setup), ADS original motor mount, 12/36 gearing (motor/wheel) 9mm belt.  Got quite a bit of skipping on 12t front gear - i use 13/14 now as a result as lowest.

Same trucks (Paris 195's) - setup dual rear w/ ~5mm spacers to fit 5065 motors:
[img]https://lh3.googleusercontent.com/-hPh_8gkCZ6k/Va3n3h4FguI/AAAAAAAAmrY/d-QbUeSSd3E5nqXnMHDO9j6bz3vXG8DOACCo/s912/20150720_215209.jpg[/img]

And complete board on a ride:
[img]https://lh3.googleusercontent.com/-PboOqp6ebgQ/VcQU6T0f90I/AAAAAAAAlQc/FfCwmyJTnYcFd5vkzhjh4s6wnvVWIUXAACCo/s912/20150722_202933-1.jpg[/img]
(GBomb, custom Subsonic deck, 97mm flywheels - awesome board until stolen out of car!)  

GF's setup now:
[img]https://lh3.googleusercontent.com/-kPs33sPKzlw/Vb_dcirbVwI/AAAAAAAAlIA/NzRnTo6FBtoPlqxjEW9CZpgyPJLeqvd_gCCo/s912/20150802_210037.jpg[/img]
Dual 3/4s - Wiiceiver/Kama Rx/Tx - VESC - 200kv 6355 motor (generic) - Enertion mount and 14/36.  83mm flywheel clones w/ Caliber II 50's.

That's pretty much the progression of my boards from taped up testing to a relatively "finished" board my GF rides.  

I have a Marbel i ride most of the time (since GF's on hers), and am still building a few other setups.  Another single motor guest board, a single motor setup to send home w/ a buddy in SoCal who will be visiting EOM, and my dual motor GBomb replacing the stolen one (bigger, better, faster, stronger).
```

---
## \#5 Posted by: rainbowbolt Posted at: 2016-07-12T19:44:55.565Z Reads: 77

```
@rpn314 
1. I have an iCharger 106b, the charging board is [this one](http://www.hobbyking.com/hobbyking/store/__31314__Hobbyking_Parallel_charging_Board_for_6_packs_2_6S_HXT4mm_.html), which I chose because the banana plug fits the iCharger and the battery plugs fit into it too.
2. I was planning to do so, but another commenter said this cannot be done with the VESC?
3. I was planning to balance charge them as 4 3s' with the chargeboard mentioned in point 1, .
Apologies if I come across rude, this format seems easiest for answering your questions.

@sl33py
Thanks for advice on the charger, I think I'll be fine but I will be sure to remember.

If I understand correctly you advise to run 3x3s for 9s1p, would it be better then to run 2x2x3s for 6s2p? This would provide more range and less top speed. My gearing setup is the kit from TB with 16x32.

The xt90 anti-spark is used instead of a power switch correct? What I don't understand is why you'd need a loop key, would connecting the batteries to the VESC through an xt90 anti-spark not be enough? Simply unplugging when you need the batteries disconnected?

Thanks a bunch for the pictures too, they really help simplifying things, diagrams just don't really work for me.

As a side note, I'm guessing there is no simple solution for charging on the go? the powerbank and iCharger are quite a burden to carry around all the time haha

Quick edit: I am an idiot, the article for the switch is definitely a great idea and I completely understand why one would do it.
```

---
## \#6 Posted by: sl33py Posted at: 2016-07-12T21:07:29.370Z Reads: 68

```
106b is a great charger and should work well for you.  What power supply are you using for it?  I wasn't suggesting to get a new or different one, just commenting which setups i have.

Balance board - how i prefer to charge.  Easy if you don't mind unplugging batteries to charge them.  BMS would be easier, but more $$$ and complexity.

I'm advising a max of 9s for your batteries.  12s will kill your VESC w/ your >200kv motor.  If you want more range (or to let a friend ride your board who is new), you can use 6s1p or 2p.  I'd usually prefer to carry spare batteries (1p) vs all of them under the board.  Lighter in your back than on your deck (when you aren't riding).

Glad the pics helped - from super newb setup to less-noobish latest setup!  I'm a visual person as well, so i take lots of pics.  Wait till i eventually do another build log of these other setups... slow speed or dialup connections be warned!

XT90 loop key - yep - simple and works well.

charging on the go?  hmm.  Compromises needed, but i got one of these for this exact reason:
http://www.hobbyking.com/hobbyking/store/__58285__IMAX_B6AC_V2_Professional_Balance_Charger_Discharger.html
About $40, plus another balance board = ability to charge 2/3/4 batteries at once.  Your big limitation is the max 6A charge rate.  

At full 6A - it will take roughly 1 hour (guessing 20% loss) per pack.  Even with parallel board - 3-4 hours for 9s or 6s2p setup. From an online calculator.  Where I would normally charge at 1C or .5C for longer pack life, and when needing a quick charge (get home and want to ride), or at work you could charge at 2 or 4 c (9A and 18A if your 106 and power supply can handle it) cutting your charge time down to just a few minutes per pack!  (edit - 106b max is 10A)

HTH!
```

---
