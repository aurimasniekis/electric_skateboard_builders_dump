# Is this a good start?

### Replies: 10 Views: 775

## \#1 Posted by: chrille Posted at: 2018-04-29T19:31:46.360Z Reads: 171

```
Hi everybody that maybe will help me.

I'm going to build a electric penny board.

This is the parts:
motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html

esc: https://hobbyking.com/en_us/hobbyking-x-car-80a-brushless-esc-sensored-sensorless.html

balancer/charger: https://hobbyking.com/en_us/turnigy-accucel-6-80w-10a-balancer-charger-lihv-capable.html

battery: https://hobbyking.com/en_us/zippy-flightmax-5000mah-2s1p-40c.html

drive: https://www.ebay.com/itm/371784008917

reciver/transmiter: https://www.ebay.com/itm/272827433005

Dose all this fit together and have i forgotten something? 
Is there any better alternative for the same price? 
Mount, wheels and penny I already have.

Maybe:
esc: https://www.banggood.com/120A-ESC-Sensored-Brushless-Speed-Controller-For-18-110-CarTruck-Crawler-TB-p-1252065.html?p=1C26078191019201612Q&cur_warehouse=CN

motor: https://www.ebay.com/itm/N5065-320KV-1820W-Outrunner-Brushless-Motor-For-Electric-Skate-Board-DIY-Kit-New/371808123716?epid=2098194759&hash=item56917dbb44:g:yx0AAOSwo4pYR84X

There is alot of different KV alternative of these one with the same price. or is it the same but china labeling everything as they want?

motor2: https://www.ebay.com/itm/N5065-5065-270KV-Brushless-Sensored-Motor-2-6KG-3-8S-For-Electric-Skate-Scooter/222453276249?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D2%26asc%3D44040%26meid%3D174f1c1551a04636a855c12ff370cd30%26pid%3D100623%26rk%3D2%26rkt%3D6%26mehot%3Dpp%26sd%3D371808123716%26itm%3D222453276249&_trksid=p2047675.c100623.m-1


I'm happy whit 10km range and minimum 20km/h. 
Also I'm from sweden so everything that isn't from EU cost alot in TAX and other fees. 
I know there is alot of this kind of questions but still... Be kind and help me :slight_smile:
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2018-04-29T19:35:04.444Z Reads: 144

```
Get a vesc, I went through a bunch of different speed controllers.. some of the cheap ones will get you hurt.. ask me how I know
```

---
## \#3 Posted by: b264 Posted at: 2018-04-29T19:35:12.836Z Reads: 138

```
Those ESC will not work.  You need a skateboard ESC or they will be jerky and throw you off-balance.  Also, a 2S battery isn't going to work with a 320kv or a 213kv motor.

Overall, based on the parts here, you're trying to spend the absolute least amount of money possible, and if that's your goal, you should buy a Meepo board.
```

---
## \#4 Posted by: pennyboard Posted at: 2018-04-29T19:46:38.383Z Reads: 120

```
I second what @b264 said. If you’re not willing to spend at minimum $400, you’ll end up with a board that’s gonna break and cost more to repair in the long run.
```

---
## \#5 Posted by: chrille Posted at: 2018-04-29T19:56:03.895Z Reads: 106

```
So the other ESC will not work ether? som other jused that one on a penny on youtube, but mabey he died. Do you know any VESC that is good enough?

But if i change the battery to a 3s? is the 213kv motor best? 

I just need to take me to point A to B and fit in a locker. I will just be able to use it like 3 mouth then it will be to cold in sweden agan. then i have alot of time to fix a real board if i want to.
```

---
## \#6 Posted by: b264 Posted at: 2018-04-29T20:25:32.576Z Reads: 94

```
cheap/fast/good

You get to pick 2.  So, you want cheap and fast?

No board that cheap will get you a 10km range but there [are](https://www.amazon.co.uk/Benchwheel-Single-motor-Sino-wave-Controlled-Longboard/dp/B01M8GF2R6/ref=sr_1_33?s=sports&ie=UTF8&qid=1525033327&sr=1-33&keywords=electric+skateboard) a [bunch](https://www.amazon.co.uk/Original-Skateboard-Electrical-Skateboard-Longboard/dp/B07199W9PP/ref=sr_1_25?s=sports&ie=UTF8&qid=1525033180&sr=1-25&keywords=electric+skateboard) that are fast&cheap in that price range.  They might top-out around 10km under ideal circumstances.  In real-world use, probably 8km
```

---
## \#7 Posted by: chrille Posted at: 2018-04-29T20:58:13.351Z Reads: 85

```
but they don't shipp to sweden. 

what i have seen and researched my build will cost like them but be beather. all the reviews of those bords suck, they are slow, week and don't last so long and others sheep builds have ben beather.

5A battery should have no problem with 10 km according to youtube and thise site? 8km is enoug anyway.

if i change to 3s battery, a real but cheap vesc. the motor is the same as other "serious builds" biggest difference is less batteries but one more should fit.

or is it beater whit a shep VESC than a expensive ESC? (chep VESC is still more expensive then high A graded ESC (i think)) can't you program ESC? 

how can this be so bad? what exactly should be different? VESC for 200 dollar? dual motor? bigger board? what type of battery?
```

---
## \#8 Posted by: uigiroux Posted at: 2018-04-29T22:02:40.782Z Reads: 76

```
As far as I know you really shouldn't use a battery below 6s, and really you can get a 6s lipo battery for pretty cheap (~$50) from HK.  That's really not much more expensive.  You can get a VESC for like $100 no problem.  Overall if you sink maybe another $100 for the price of the upgraded parts you'll be much better off.
```

---
## \#9 Posted by: FredrikHems Posted at: 2018-04-29T22:22:17.406Z Reads: 70

```
@uigiroux is right. 6s or ~24v is the lowest you should go on voltage. Range or more precise Watt-hours doesnt just depends on Ah, but voltage is just as important. 
For reference: 
A 6s 5Ah battery will get you about 10 km, with a total of 110Wh.

A 12s 2.5Ah battery will also get you about 10km, with a total of 110Wh too.
I will suggest you to read abit more about different battery setups, until you get a better understanding, and can then choose what setup you want.
```

---
## \#10 Posted by: uigiroux Posted at: 2018-04-29T22:24:21.720Z Reads: 68

```
Also, you could check out the for sale section here and probably find a cheaper used vesc and maybe even a battery.
```

---
