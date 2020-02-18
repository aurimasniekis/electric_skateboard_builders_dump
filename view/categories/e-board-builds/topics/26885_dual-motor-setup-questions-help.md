# Dual Motor SetUp Questions Help

### Replies: 6 Views: 1137

## \#1 Posted by: Exiledd_Top Posted at: 2017-07-06T02:51:44.275Z Reads: 116

```
Yes hello I have a few questions i would like to ask and i would like to present my build.
Where i  Live it is mostly hill's and hill's, i wanted to buy a boosted board or evolve carbon gt but they are not worth it, just for the fact that they would tackle hills bad, so i decided to do my research and research and watch 8+ hours and read forums of building on what to do and what not to do.
First i would like to present my build or the parts that i ordered 
(1)63mm 5300W Dual Motor Electrical Skateboard Kit -
diy-electric-skateboard-kits-parts/63mm-5300w-dual-motor-electrical-skateboard-kit/
(1) TorqueBoards 218mm Trucks(2 trucks)-
diy-electric-skateboard-kits-parts/torqueboards-218mm-trucks/
(2) Single Bolt On Motor Mount W/ Drive Wheel Kit(for 63mm motors)-
diy-electric-skateboard-kits-parts/single-bolt-on-motor-mount-with-drive-wheel-kit/?attribute_motor-mount-size=63mm+Motors&attribute_drive-wheel-gearing=16T%2F36T+12mm+ABEC+Drive+Wheel+Kit
(2)Turnigy 5000mAh 5S 30C Lipo Pack-
https://hobbyking.com/en_us/turnigy-5000mah-5s-30c-lipo-pack.html?___store=en_us
(1)Enertion Nano-X 2.4Ghz Controller-
http://www.enertionboards.com/electric-skateboard-parts/nano-x-enertion-2-4ghz-controller/
(1)90mm EPOWER Flywheels BLACK-
diy-electric-skateboard-kits-parts/90mm-longboard-epower-flywheels/
My Board is A Long board and this is the exact one 
Bamboo Loaded Flex 2- https://www.daddiesboardshop.com/loaded-fattail-bamboo-longboard-skateboard-complete?gclid=Cj0KEQjwnPLKBRC-j7nt1b7OlZwBEiQAv8lMLGNxYHiDwHfCbgca9LDQtYrEhxNWW8WZcBRq1Q2oAYYaAq2U8P8HAQ

My main concern is i wanted a 10s set up for the fact that i tried to learn how to solder a BMS but people dont specify what type of metal they burn (i am like basic knowledge of soldering) and the solder each cell part i get just what to do type of watt solder to use and what to do  with the - and + of the terminals in the BMS some say use the + for something and leave the - alone but they still solder it and just leave it there which is why am confused and second i want to use a Loop key but want to do the minimalist soldering as possible i i was looking at hobby king and wonderd can i use https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html?___store=en_us
as a loop key and just buy https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html?___store=en_us and use just the male part ? If you look at my build and something doesn't add  up please feel free to say something any help would appropriate it  thank you 
i also still haven't figured what enclosure i will need i want to keep the middle cleared because i did the mistake of buying a bamboo board and then doing my research so any help of what enclosure would help as well
```

---
## \#2 Posted by: wafflejock Posted at: 2017-07-06T03:15:16.358Z Reads: 93

```
Your idea with the series connectors and using the Male connector as the loop key (anti-spark is a good idea) will work fine.  

Can see the calculator to put in your values and get a pretty good idea of the weighted top speed of the board, if it goes much faster than you can run you should get familiar with how to fall from a high speed (starting off slow).  Know lots of skaters are not fans of braille but they have a decent video walking through it here if you aren't an avid skater already https://www.youtube.com/watch?v=Hundbrub8iQ

I started skating later in life but have been on and off skating for over 10 years so wasn't terrible getting going but some people are jumping right into eskateboarding which if it's the case for you then you should definitely heed this advice (also regardless make sure you have at the very least a helmet).

Regarding the enclosure if you have access to a 3D printer there are a few designs on thingiverse including my own (that is for 2 5S 5Ah in series but I'm working on a v0.2 er 0.3 but no one is keeping track).  If no 3D printer lots of people have either done molds using vaccum forming and/or using epoxy and fiber to make the enclosures or you can go the easy route for now and find some suitably sized tupperware or similar containers readily available at the store.

Make sure you have some extra 8-12 AWG wire as well for connecting things, also instead of the Y connector cable could just buy a box of XT-90 connectors and one antispark one just to have spares around in case you need to replace one ever or move things around without needing to pull out old connectors.
```

---
## \#3 Posted by: Exiledd_Top Posted at: 2017-07-07T03:05:27.035Z Reads: 71

```
i have a question as well i forgot to ask you Since i am getting a 5s 5000mah with 5,5mm bullet connector and i am getting 2 cant i just pair them both like connect the negative with the positive and there connected together or no? also what charger do you recommenced i was planning on using  https://hobbyking.com/en_us/imax-b6ac-v2-professional-balance-charger-discharger.html?___store=en_us but its a 4mm bullet connector and my batteries are 5.5mm bullet connector do i just get a adapter ? and would it be safe? if not what charger would you recommend thank you for your time
```

---
## \#4 Posted by: wafflejock Posted at: 2017-07-07T03:22:58.467Z Reads: 69

```
Yup you could chain those in series with the bullet connectors.  Basically you just want a loop key with the anti-spark connector in there to be somewhere you can reach it from the top of the board so all else fails you have some chance to pull the loop key and cut the battery pack from the rest of the electronics ASAP.  The anti-spark is really just a plug with a resistor built into it so the first part of plugging it in the charge goes through a resistor in there that slows the current enough to avoid big sparks and lets the capacitors fill with some charge so by the time the rest of the plug is inserted past where the resistor is the capacitors have some charge and there isn't such a big inrush of current (which will toast/arc weld stuff).

So yes to chaining them, in series through the bullet connectors but still good to have a loop key in the circuit somewhere to break it and to be the last thing that connects to complete the circuit.

Regarding the charger I have a 80W one, they go for around the same price as the 50W one you linked, http://www.robotshop.com/en/b6ac-lipo-battery-charger-80w-us.html?gclid=Cj0KCQjwv_fKBRCGARIsAL6R6ehFu4hR7EJjAxase-zbATTdJqtpqZlQNts4s4WHBn56YsqiPFAfsMEaAksFEALw_wcB <-- that's not the exact one I got I forget where I ordered it from but it's essentially the same.  Basically you will need to charge each battery separately so you'll need to disconnect the series connection for charging each of them unless you get a charger that can deal with 10S balance leads in which case you could charge it as though it's just one big battery with 10 cells.  With the 80W charger I can set the charge rate to 3.6A before it starts to overheat, I keep a computer fan plugged into a USB adapter pointed at it and it stays cool enough (up to 5A should be easily in the safe zone for charging a 5Ah LiPo).  At 3.6A it usually takes about an hour or a few minutes more per battery to recharge from 70-80% depleted which is as far down as I take my batteries (3.6V per cell).  If you go with a 50W charger can expect max charge rate to be something more like 2A so will take closer to two hours or more per battery to charge.  Basically chargers that can handle higher W have fans/more heatsinks and beefier components to deal with the extra current but trade of in price vs time to charge.  You also don't want to charge above 1C unless the battery manufacturer says otherwise and always better to go slower in terms of overall battery life.

Oh also regarding different connector types, I usually just replace them on one of the components so they all match so go with all 5.5 or all 4mm if you're doing bullet connectors, I stick to XT-90s or soldering stuff to the boards for the most part though.  Also the chargers have a banana plug usually for the discharge wires and can get banana plug to almost anything.

---

If you go cutting connectors off of batteries make sure you understand what you're doing, work on only red or only black at a time never cut across both wires you will make a short with your tool as the high resistance piece in the middle and can end up welding the leads and your tools together and shorting your batteries in a very bad way.  Only ever expose one of the leads on the battery (red or black) and make sure the other is sufficiently wrapped in electrical tape or soldered down and covered with electrical tape or shrink tubing, biggest danger is short circuits causing big arcs/shorts.
```

---
## \#5 Posted by: Exiledd_Top Posted at: 2017-07-07T03:34:26.761Z Reads: 47

```
the reason i asked was because my whole set up is going to 5.5mm bullet connectors  besides the loop key, so i am confused if i get a adapter such as 5.5mm bullet connector to 4m bullet connector to charge each battery separately would i be okay or not ? and thx ill take that charger into consideration. i was thinking  of putting my vesc at 3.4v per cell thats what most people recommend for shut down, i dont plan to cut any wires at all   especially my battery wires! am a total noob for that !lol, is it different for 5s batteries ? thats the max you recommend them at?
```

---
## \#6 Posted by: wafflejock Posted at: 2017-07-07T03:43:59.995Z Reads: 49

```
Eh was just discussing this with someone in another thread they think that 3.5 is fine I don't go below 3.6 I started off doing like you around 3.3-3.4 for my cut offs but with voltage sag you can bring some of the cells below 3.0 if you set it that low and once the cell goes too low it never charges all the way back up with the rest of the pack (if your charger will even accept it).  There are videos on faking out the charger to pump some juice back into a cell that has been over discharged but it isn't really safe and even having done it the result is you have a cell that never gets fully charged and therefore a pack that is always out of balance... long story short if you go 3.6 you will be safe but you are keeping about 20-30% of the charge in the battery which means you're reducing your range by as much.  I still get about 12 miles on 2 fully charged 5Ah 5S in series on a 149kv 16/36T setup, I wish I had more range but I want 12 more miles not 3 more :) working on a swappable pack for that but the 3d print has been killing me.

Yeah the adapters on the discharge cables for the sake of charging too is all good you just don't want a lot of adapters on the board itself since ya know more points of failure.  With 10S the sparks I get without an antispark haven't been that severe, with 12S I was blowing up XT-90 plugs and replacing them after every few rides, any sort of easy access way to break the circuit is good to have though (controllers/receivers/escs can all do crazy things sometimes and everything is being vibrated on the ground pretty violently).
```

---
