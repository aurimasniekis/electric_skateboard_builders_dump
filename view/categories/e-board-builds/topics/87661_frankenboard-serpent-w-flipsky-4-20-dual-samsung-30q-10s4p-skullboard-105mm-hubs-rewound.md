# Frankenboard / Serpent-W / Flipsky 4.20 dual / Samsung 30Q 10S4P / Skullboard 105mm hubs rewound

### Replies: 4 Views: 400

## \#1 Posted by: MiniChopper4Me Posted at: 2019-03-19T19:07:10.443Z Reads: 134

```
![image|666x500](upload://6ppfaDUCtziFhWaqYw9zaTtOqt6.jpeg) ![image|666x500](upload://lFiUjOOy9E2vgZAQdu904um8GF9.jpeg) ![image|375x500](upload://7Tfo0CjcrDxxN1yrvd6BM4sj0Xi.jpeg) ![image|375x500](upload://qBimbL7cJsoJKokqdchFfH3oQHS.jpeg) ![image|666x500](upload://jNombxVRv8fAHZ8DDRz25rC8wDP.jpeg) So I finally completed my "first build", although I'll be the first one to admit its hardly a build so much as a rebuild.

I used the Serpent-W as the shell, but replaced all the guts.  It has a Flipsky 4.20 dual for the ESCs, Skullboard wheels and motors, a Samsung 30Q 10S4P battery, Hoyt St. puck for remote/receiver and just an Anti-Spark loop key for power.

I rewound the motors to 15 turns of 2 strands of 21AWG wire instead of 16 turns of 10 strands of ~28.5AWG.  As a result, I am able to deliver more power to them without anywhere near as much heat generation. Details of the rewinding can be found [here](https://www.electric-skateboard.builders/t/rewinding-90mm-hub-motor/80491/1)

I currently have the VESCs set at:
40A motor current
-40A brake current
40A battery max
-6A battery regen max

I'm also using Ackmaniac firmware, and am using it in current mode so that I can go from forward to backward without hitting a switch, since I'm used to and enjoy Boosted Board controls.

I burned through 2 separate anti-spark switches in the process of re-building this thing, and finally gave up and went the route of the loop key.

The charging port is everyone's favorite DC jack 5.5mm x 2.1mm with a rubber waterproof plug.  I have an 8A charger for it, so I also used a micro deans connector between the battery and charge port to ensure it doesn't melt (the battery I had came with a JST connector which would probably melt at that current over time)

I installed a voltage meter at the front bottom, which only works when the loop key is inserted.  I like that it lights up the undercarriage some.

I'm using a Hoyt St puck for the remote.  I love it!

This board is heavyAF at 25lbs.  It has *zero* flex!

Can anyone tell me how to better diagnose issues with the VESC? While everything seems to work great at the moment, I have had repeated issues that I'm pretty sure I can reproduce if I want to, and that is that if I go from full acceleration to full brake/reverse, I can make the VESC power down, until I turn it off and back on again.  I'm not sure how to get the faults from the VESC if they exist, or if I need to change my settings so that this doesn't happen, or if its just something I need to not do (stop going from full acceleration to full reverse/brake).

This is my first (re)build, so any suggestions would be welcome.  Thanks in advance!

I still plan to take it apart again and basically seal everything up with black silicone gasket maker to make it as watertight as possible.

(pictures forthcoming, I know this thread sucks otherwise)
```

---
## \#2 Posted by: Octave Posted at: 2019-03-19T19:34:03.769Z Reads: 95

```
Here's a topic that had really good information on the flipsky 4.20. Propably someone also has had the same vault and has put their solution there.
https://www.electric-skateboard.builders/t/flipsky-dual-fsesc4-20-info-review/71079/237
```

---
## \#3 Posted by: MiniChopper4Me Posted at: 2019-03-28T14:20:20.584Z Reads: 57

```
I see myself performing the resistor mod fairly soon in order to get rid of the cutouts.  We'll see how it turns out!
```

---
## \#4 Posted by: MiniChopper4Me Posted at: 2019-08-01T21:29:33.244Z Reads: 25

```
I did the resistor mod, and broke the Flipsky in the process.  Thank God for @JohnnyMeduse! Added a Metr Pro to the setup, along with full waterproofing using FlexSeal(tm)

I take this out pretty much daily, and its a great ride despite how stiff the deck is.  Time to give this board a real name!
```

---
