# NOOB AF PLEASE HELP IM DUM. DIY build! 10s4p 18650 with 3500mah cells+VECS+Bluetooth BMS etc

### Replies: 7 Views: 1226

## \#1 Posted by: david2772 Posted at: 2017-06-21T18:20:40.151Z Reads: 209

```
HELU PEEPS! sooo im trying to build a DIY Battery and a DIY eskate (obviously) and i have the following parts in mind. i have a bamboo long board (its pretty long) and is medium in flexibility. BUDGET LIMITED AF. so these were picked "carefully" to give "absolute performance". 


 MOST ARE ALIEXPRESS SHYT BUT WITH FAST SHIPPING  (like 2 weeks to canada)

motor:
http://bit.ly/2sqNxuK

this thing: (used for a charger? idk)
http://bit.ly/2sBvuAl

trucks:
http://bit.ly/2sWcL5a

remote: ( does this work with the vesc? )
http://bit.ly/2rW1cX9

VESC: (will get a coupon from seller too)
http://bit.ly/2sr2IUO

batteries: (good reviews...seems legit 3500mah)
http://bit.ly/2rVLGe3

charger: (no idea what cable is needed for bms to connect to this BS)
http://bit.ly/2rVGFlG

BMS: (with bluetooth so i can check on batteries and  blah blah)
http://bit.ly/2sUzIpE

wheels: (4 of them)
http://bit.ly/2sBrvDT

wheel pulley: (does this fit the wheels above? it says 17mm like wtf man)
http://bit.ly/2rVEgHG

mount: (option A)
http://bit.ly/2sUs4vB

mount: (option B)
http://bit.ly/2rVWFE1

confusion 1)
 is with the amps and volts (noob level -99).. basically i want to use the BMS with bluetooth because it shows how much miles and battery status left on your phone (which is like A++) and i dont know if it can handle 40cells (how tf do you calculate). also the configuration of the battery.. how many configurations are possible for my case (if any)?

confusion2)
is with the on/off switch (link one from ebay i beg u). how do you also wire that switch to work with the parts listed above? 

confusion3)
is with the freaking motor mount. which one do i use (if any of the options above work)

confusion4)
is with the wheel pulley. i found enertion pulleys that are 12mm but these suckers on ebay say they are 17mm? ebay ones are half the price of that of enertion so i was wondering if they fit a 83mm wheel.

confusion5)
what how where do you get a cable for the charger above that connects to the BMS? any alternatives? 

confusion6)
is with the remote. does the one listed above work with the VESC? if it doesn't, can you give a link to one that works (ebay preffered)? 

so what i want from this build is high milage and medium to high ish speed (30-40km/h? no? ok)

ALL ANSWERS AND SUGGESTIONS ARE VERY GREATLY APPRECIATED!!!
```

---
## \#2 Posted by: aigenic Posted at: 2017-06-21T18:59:31.126Z Reads: 179

```
Mounts: one of them is made for maytech trucks with welded ring on the truck so it cant be used on normal truck, only as a set....the second one can be used, but it is not good motor mount, it will be better if you get calibers and motor mount from somone on this forum, there are some cheap for like 22$...

Pulley: Should be ok, but i think it is HTD3, not HTD5 that is commonly used and better

BMS: it is ok, but rated only up to 30A, you should use it just for charging or buy a BMS with higher amp rating

Battery: 10S4P packs are commonly used, but the cells you mentioned not...use samsung 25R, LG HG2...more [here](http://www.electric-skateboard.builders/t/choosing-18650-cells/6240/4)
You will also have to connect them in series/parallel...you will have to use spot welder unless you want to damage the cells...some builders also use vapes, but they are quite expensive...

Remote: Good, often used but not reliable, get a Mini remote instead :slight_smile:

Trucks: just get calibers, they are better, reliable and they have (almost) square profile... 

Motor: Ok, you might exceed ERPM limit od the VESC, but it shouldnt be much, so basicly ok :) 

VESC: Maytech VESC is not good choice...if you are from the USA, get AXEL or DIY vesc, they are cheap and better :) if you are from Europe you should also consider different VESC, Maytech are not good...

conf 1: it can handle even more cells if you connect them correctly, but it cant handle more than 30A
conf 2: Make your own antispark switch from xt90 connectors or buy Vedder anti spark switch (alienpowersystem.com)
conf 4: They are HTD3, not as good as enertion pulleys but they should work...your belts wont be able to transfer as much torque as HTD5 belt...
conf 5: IDK
conf 6: It works, but get the MINI :slight_smile:

usefull links:
http://calc.esk8.it/
http://esk8.today/2016/12/28/how-far-can-i-ride/#rc
```

---
## \#3 Posted by: MockCocos Posted at: 2017-06-21T19:27:17.129Z Reads: 161

```
Can't help you will all your questions, because my knowledge exceeds some of them.

Gear kit: As far as the gear ratio goes, they are wide af and might hit the side of the truck. That system to how the gear attaches to the wheels has been known to cause the inner side of the wheel above the core to grate like cheese. Which will ruin your wheels.

The wheels: Speaking of wheels, you can't really go wrong with Chinese wheels 

The trucks: Each truck on the website is a different color/different pattern so which color would you be going with?

The motor mount: May fit the truck depends on what color/pattern you get

Remote: Should be fine, because it comes with a receiver. I can't guarantee it though.

Vesc: Don't know much about that one, but try to get a quality one. 

Batteries: Sketchy man. I would never buy batteries from ebay or a Chinese distributor. Get them from NKON or Liion Wholesale.

Charger: The one that everyone gets lol. Should be fine, make sure you get the right plug.

BMS: Doesn't look like enough amperage for the cells, but depends on your batteries orientation.  

Motor: Looks fine, but again that 40a current. Depends on how you set up your batteries.

Charging port: I wouldn't go with one of those, too easy to short circuit. Get one of these (pretty sure it fits your charger but I would check) http://www.ebay.ca/itm/1PC-Waterproof-5-5-x2-1mm-DC-Socket-Power-Jack-Plug-Female-Mount-Connector-/181989199616?hash=item2a5f66cf00:g:mGIAAOSwJkJWlKMR 

Confusion 1

Depends on how you config the batteries, the more recommend type is to get 30 cells, because there is minimal voltage sag and put them in 10s3p which means 10 cells in series=voltage and 3 cells in parallel=mah and amperage. 

Confusion 2
Ask the forums, I use something pretty expensive but works well which is this diy-electric-skateboard-kits-parts/electric-skateboard-on-off-power-switch/

Confusion 3 

You can get most of the parts you are looking for from the link above, just more expensive as it comes from the united states.

Confusion 4

Those wheel pulles for the wheels is plastic which is....not good, I wouldn't plus they are wide af


Confusion 5 
This is how you setup everything <img src="/uploads/db1493/original/3X/7/e/7e0622aa91f97e8cb73d46234f6a4cf0f1a3a196.jpeg" width="689" height="363">

Confusion 6
Remote should. These work too

http://www.ebay.ca/itm/2-4GHz-Receiver-Binding-Plug-Radio-Remote-Controller-For-Electric-Skateboard-NEW-/232284516689?hash=item36153c7151:g:gfMAAOSwax5Y2PAs
```

---
## \#4 Posted by: sl33py Posted at: 2017-06-21T23:31:36.604Z Reads: 106

```
Welcome.

I would stick to some tried and true setups vs the mix of things linked.

83mm clones work great - Amazon or elsewhere is fine.

motor - that 6355 looks OK.  Watch out for 10mm shaft versions and avoid - nearly all gears you'll find easily are 8mm.  (the one you linked was 8mm just FYI).

Motor mount - don't skimp.  Get a good quality motor mount or you can fight with it incessantly.  @KorryH has great inexpensive and sturdy ones that are a lot less than others but just as quality.

Trucks - stick to Caliber II's or good caliber clones.  Need the shape of the hanger as it's not round so makes the mount more secure and won't rotate like on Paris and other round trucks.

Batteries - if on a budget - i'd stick with some good quality Lipos from HK.  I'd go for 5000mAh 30C or higher in series for the voltage you want (6/8/9/10/12s).  I personally like the 3 and 4s packs as they are really thin and then add more in series to get 9/10/12s.

Charger - iMax B6ACv2.  Get the legit one - good charger for the price.  

Remote - GT2b - cannot beat it for the price and save a few $.  Move it into a 3d printed case later (master cho, badwolf, flatline customs, okp, etc.).

VESC - i would instead get from Axle or DIYes - basically the same price or really close and will have bootloader working!  A bit more $ for VESC-X/FOCBOX, or Ollin board co variants might be money well spent if you save some $ elsewhere and can swing it.

Wheel pulley - look for some here, but i'd avoid 3d printed ones like linked for longevity and less likely to skip.  DIYes has some nice 36 and 40t aluminum ones (my preferred vs nylong or injected molded like Enertion (also need to cut/modify axle hanger to fit)).

on/off switch - get or make an anti-spark loop key.  Easy if you can solder, or see if you can find one.  Vedder's anti-spark is also good, but a bit more $.

12 or 15mm belts - use bbman belt length calculator w/ gears and axle to axle (CtC) distance measured to determine belt length needed.  if you stick with some well known motor mounts and gearing we can probably help you with those measurements and belt lengths likely to work.  I would pick between 12 and 15mm for a single motor setup depending on your weight and how much downhill hard braking you plan to do.  

Welcome and GL!
```

---
## \#5 Posted by: potatowarrior13 Posted at: 2017-06-22T05:13:31.489Z Reads: 92

```
Hey
Straight to the point... Looking at your post i'm not sure if an electric skateboard is the best first project for you, if you make mistakes they will be very costly. I suggest reading up on basic RC electronics and basics like series and parallel wiring, relationship between amps and volts, li-ion battery technology, 3-phase brushless motors, and how to program a VESC, how to solder (if you don't know) etc, before attempting something so expensive like this. Not trying to crush your dreams of building an e-sk8, but its actually quite complicated without previous experience with similar projects and you might end up making a mistake that could cost you a lot of money.

That said, good luck with your build, building an e-sk8 can be a practical and rewarding experience!
```

---
## \#6 Posted by: david2772 Posted at: 2017-06-26T00:21:26.354Z Reads: 76

```
HI ALL. THANKS FOR THE REPLYS!! 

a few other questions i have:

1) how can i use a sprocket chain for the wheels listed ? thinking on using this: ( http://bit.ly/2sRbSIF )
2) would i be able to use scooter wheels (or any bigger wheels for off road) on this 10s3p settup? and if i do, can the sprocket chain be used?
3) what are some slim 10s3p configurations for the batteries? i want to keep it as slim as possible with the 10s3p setup and get a good range (ordering 30 3000mah LG gh2 batteries).
4) is there any good battery indicators that you recommend? on budget!
5) is there a how-to detailed tutorial on making a power switch from anti spark xt90?

THANK YOU ALL!
```

---
## \#7 Posted by: oldguy Posted at: 2017-06-26T00:48:20.534Z Reads: 68

```
This has probably been covered already, but since it is thus far my favorite hyperlink of all time, your reference to "this thing" lol, (no really, out loud) is not what you want. That is strictly for audio. So unless you are integrating headphones into this build (*light bulb - ding*) you'll want a different adapter. I love the link though!
```

---
