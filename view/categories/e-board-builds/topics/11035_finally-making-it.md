# Finally making it!

### Replies: 12 Views: 1312

## \#1 Posted by: dmhmaestro Posted at: 2016-10-12T22:09:35.593Z Reads: 216

```
Hello all! 

I am going to be brief.. After long time i finally have money for my E board. Ive read alot about making it but i am noob in electronics so would like to have this thread open for my build. I will base all components of banana board build on instructables web.. Which most of u know i guess. Next week im buying this board and will order battery motor and few things im certain i will need.

My first question is should i really buy 190 kv or 245 kv? Because in banana board tutorial the kmh is 35 and mileage 15 km which sounds really gr8. I hope someone will find time to tutor me in my build because its really exciting!

[http://www.njuskalo.hr/image-w920x690/skateboard/longboard-globe-slika-64442025.jpg](http://www.njuskalo.hr/image-w920x690/skateboard/longboard-globe-slika-64442025.jpg)
```

---
## \#2 Posted by: sl33py Posted at: 2016-10-12T22:49:01.283Z Reads: 190

```
Welcome and looks like a fun build.

a couple suggestions - i would personally start with the ESC and voltage (# Series) of the battery you are going to use?  I'd usually recommend starting with two 3s batteries in series for 6s.  This gives you a lot of flexibility as most ESC's are capable of 6s voltage.  And if you get a VESC or similar you can add a 3rd 3s battery for 9s later, or a 4th for 12s if your kv of your motor is low enough to avoid 60k ERPM (where the DRV chip can/likely will have issues).

SO - ESC you want to use?
Where are you riding - hills or flats?
What kind of riding?  Cruising, commuting, racing?
How heavy are you?
What's your realistic budget?

Speed (your goal is 35kmh?) is just a factor of wheel size, motor kv, # Series/voltage of battery, and gearing (motor/wheel).

So an example setup to hit your target speed:
83mm wheels - 190kv - 8s - 15/36 (one of the most common - the kit enertion sells uses this too) = 35kmh

But at 8s you will need an expensive RC ESC, or VESC, or similar.

Same setup just swap in 245kv motor, and 6s battery = 35kmh again.

I'd grab one of the calculators and play with the settings to see what gets you where you want to go speed wise.  If hills or acceleration are your goal - i might even gear down further with a smaller motor gear (no smaller than 13t - especially on 9mm wide belts or it will skip), or go larger on the wheel gear 36->40t, or larger if you want to print some from thingiverse.

range - there are some rough ways to estimate your range.  Best is to use Watt Hours (Wh).  Take your battery pack voltage (6s @3.7v nominal = 22.2v) x Amp Hours (convert from mAh) = Wh.  So an example is some of the zippy or similar 3s (2 in series) 5000mAh (5Ah) 20c packs.  So 22.2v (6s) x 5Ah = 111Wh.

You should expect (with moderate riding and weight) to get about 1km per 10Wh.  So 111Wh = 11km.  If you want more, you need a higher Ah pack, or more voltage (more batteries in series for 9s as example).  a 9s pack (3.7v x 9) = 33.3v x 5Ah = 166Wh = 16km!

A lot to take in - give us some of the above detail and we'll help you figure it out!

HTH - GL!
```

---
## \#3 Posted by: dmhmaestro Posted at: 2016-10-12T23:08:13.328Z Reads: 162

```
Well sir thank u alot for extensive reply!

So for now the only thing i got sure are wheels... they are 80mm.

The other info..

budget around 350$
I have 80 Kg
I would like to go uphill because the town i live in now is pretty hilly... lol. 
I really like to go fast so the faster the better but within budget.
For mileage i could be happy with 10km. Although the tutorial i want to follow states 15 km range with its components. 
One thing. I would like to find good tutorial so i can follow it step by step. I mean i am sculptor and handy but with electrics not so much!

Banana board specs are

35 kmh top speed - 15 km range

83mm wheels - 190 kv brushless - 2x 5000mAh 20c 3 cell (11.1v) Lithium Battery

I also found this kinda cheap esc 

http://www.ebay.com/itm/GoolRC-150A-2-6S-LiPo-Battery-Sensored-Brushless-ESC-for-1-8-RC-Car-Latest-J9N0-/111907377671?hash=item1a0e331207:g:dAkAAOSwUuFWwtSx

What are ur thoughts?
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-10-13T04:17:50.022Z Reads: 117

```
A dual is best for hills...a single will end up just burning up. 

The ESC is fine ... I've used them but there is hardly any support for them.
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-10-13T04:18:40.979Z Reads: 123

```
Use this to figure out gearing 

http://calc.esk8.it
```

---
## \#6 Posted by: TarzanHBK Posted at: 2016-10-13T07:40:36.077Z Reads: 114

```
you will have serious problems with your budget and your specs!
if you want to go so low on budget go with a 6s 245kv system. 
But you have to do lots of things by yourself and i don´t think you´ll stay in your budget limit for your desired speed/range/torque.
I´d say at least double your budget for these things :smiley:
```

---
## \#7 Posted by: dmhmaestro Posted at: 2016-10-13T09:56:47.605Z Reads: 92

```
everywhere i look people say 350 is ok budget and vlad pomogaev is also always on that budget...

my budget is really 350 and cant go much bigger than that. So u recommend i go 245?

I dont have to go uphill it would be big plus but i dont have money for dual setup right now.
```

---
## \#8 Posted by: Mark Posted at: 2016-10-13T10:04:18.593Z Reads: 94

```
Are you located in Europe? If so, tax will kill your budget bigtime.

http://www.electric-skateboard.builders/t/europe-motor-controller-pulley-wheel-group-buy/10295/155

For cheap parts in Europe!
```

---
## \#9 Posted by: TarzanHBK Posted at: 2016-10-13T12:18:57.740Z Reads: 81

```
yah its possible if you do everything yourself like pulleys and motormount.
Everywhere else, descend builds start at 600 EUR i´d say.

Talk to @ajaynagra about your parts.
```

---
## \#10 Posted by: Tuomalar Posted at: 2016-10-13T13:28:27.008Z Reads: 83

```
Built my first board with 350e and it has been pretty reliable. It was true diy.
```

---
## \#11 Posted by: dmhmaestro Posted at: 2016-10-13T20:05:29.070Z Reads: 73

```
I plan on doing my mount and maybe printing gears... I am from europe but tax is not that big 25% so if i order 200 it will be 50 euros its not so big deal i guess.

Does anyone have 3d blueprints for 245 kv 80mm wheels?
```

---
## \#12 Posted by: TarzanHBK Posted at: 2016-10-14T06:43:04.891Z Reads: 54

```
245kv 80mm wheels??

245kv-motor
80mm wheels (orangatang kegels?)

what you want is depending on your motorshaft a 8mm pulley (don´t print this one - use aluminium or steel)

and for these wheels depending which one you use a wheel pulley.
http://www.thingiverse.com/thing:752893
```

---
