# New User/Builder need some advice on what I need to build my first eboard!

### Replies: 14 Views: 676

## \#1 Posted by: FoxxyPants Posted at: 2017-02-21T01:42:23.173Z Reads: 88

```
Like the title says I'm REALLY new to this forum and the whole idea of electric skateboards, so bear with me. I've been struggling with trying to figure out which ESC to use, since (from my perspective) there seems to be alot of variables that matter in some instances, and don't mean much in other. I'll be mainly using the board for small travels to school or the store (1-2 miles at best) but still want the option to go a distance, or cruise for a bit. Here's the list together of what I think is needed to properly build a sick nasty board:

Battery: https://hobbyking.com/en_us/multistar-high-capacity-4s-10000mah-multi-rotor-lipo-pack.html

SEC: diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/

Motor:https://uedata.amazon.com/Turnigy-Aerodrive-3548-840kv-Brushless-Outrunner/dp/B01876Q6SI/ref=pd_day0_21_3?_encoding=UTF8&psc=1&refRID=WM1ZHHE22JAZ19MYZRAP


Wheels:https://www.amazon.com/Longboard-Flywheels-Wheels-Bearings-Spacers/dp/B01N8XLEKU/ref=sr_1_4?ie=UTF8&qid=1487349817&sr=8-4&keywords=abec+flywheels

Bearings: https://www.amazon.com/Bones-Reds-Precision-Skate-Bearings/dp/B01GBJC0CY/ref=sr_1_4?ie=UTF8&qid=1487437451&sr=8-4&keywords=skateboard%2Bbearings&th=1&psc=1

Trucks: https://www.daddiesboardshop.com/caliber-ii-longboard-trucks-two-tone-blue-50-degree

Controller:
https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html

Drivetrain: http://www.ebay.com/itm/Electric-Skateboard-Motor-Mount-63mm-DIY-Aluminum-Caliber-Truck-Compatible-Kit-/152399972223?hash=item237bbf077f:g:WHkAAOSwNnRYk1dF


Pulley(s): http://www.enertionboards.com/electric-skateboard-parts/12mm-wide-drive-pulley-kit/


Board: https://www.amazon.com/SCSK8-Bamboo-kicktail-Longboard-Skateboard/dp/B004URTVBI/ref=sr_1_2?s=outdoor-recreation&ie=UTF8&qid=1487350611&sr=1-2&keywords=bamboo+longboard+deck

Thanks in advance for the input and dealing with my ignorance
```

---
## \#2 Posted by: willpark16 Posted at: 2017-02-21T01:48:46.627Z Reads: 75

```
Yea that Motor is a no no, I recommend reading A bit more
```

---
## \#3 Posted by: FoxxyPants Posted at: 2017-02-21T01:50:32.208Z Reads: 75

```
Can you explain why?
```

---
## \#4 Posted by: JLabs Posted at: 2017-02-21T01:51:32.637Z Reads: 73

```
840 kv is a bit to high and the motor isint very big. Your top speed is going to be about 50mph and you will have zero starting torque. Your going to want a single drive 6354 190kv motor. I'll just drop this here: https://electric-skateboard.market/product/190kv-sealed-motor/
```

---
## \#5 Posted by: willpark16 Posted at: 2017-02-21T01:54:03.690Z Reads: 74

```
Not to mention it won't work with the vesc
```

---
## \#6 Posted by: FoxxyPants Posted at: 2017-02-21T02:24:51.237Z Reads: 70

```
I was just curious why this ESC is so cheap compared to the ones double the price, and if it should be even considered for stuff like this: http://www.banggood.com/FVT-CBWI120A-ESC-Brushless-Speed-Controller-For-110-and-18Series-RC-Cars-Skateboard-ESC-p-985970.html
```

---
## \#7 Posted by: psychotiller Posted at: 2017-02-21T03:10:22.854Z Reads: 68

```
After you burn out a few of these or have your board lock up or take off on you you'll see the value in paying for a good speed controller with board worthy failsafes.
```

---
## \#8 Posted by: FoxxyPants Posted at: 2017-02-22T02:39:31.216Z Reads: 38

```
Could you guys recommend any videos that can explain these things more in depth? Because I wanna more about this stuff, rather than just building it and not knowing a thing about it.
```

---
## \#9 Posted by: jaykup Posted at: 2017-02-22T02:58:19.275Z Reads: 42

```
All that info is sort of scattered throughout these forums.  Search around a bit and you should find most of the answers.  

Your build looks good except the batteries, esc and motor.

**Battery** - you will probably want to run 8-10s with around 100-200 watt hours (10-20km range) (8s x 3.7v x 5000mah / 1000 = 148 watt hrs.  Rule of thumb - around 10 watt hrs per kilometer, that's a rough range of 14km.

**ESC** - basic ESCs work fine for RC cars and stuff but don't provide a lot of control or customization for electric skateboards.  The VESC is an open source ESC designed by Benjamin Vedder and is really the standard for skateboard use.  The VESC has tons of settings that can completely change the feel of the board, throttle, braking, acceleration, etc.

**Motor** - Browse the build threads for a while - you will see a lot of 50mm and 63mm motors at 150-200kv.  Those tend to work the best on a skateboard overall.  The VESC has some limitations when it comes to motors much over 200kv (simplified - head over to vedder.se for more reading).
```

---
## \#10 Posted by: Tampaesk8er Posted at: 2017-02-22T03:30:36.242Z Reads: 44

```
I bought the motor mount you listed from ebay, it doesnt work good with caliber II trucks, need special shims that retailer doesnt provide.. I had to buy a second motor mount from psycotiller.com and he provides shims, it finally worked perfectly with my caliber Ii trucks.
```

---
## \#11 Posted by: korryh Posted at: 2017-02-22T05:45:58.926Z Reads: 40

```
Agree - you need different batteries, esc and motor

I started with that same deck, wheels and trucks with the following electronics.

Battery - started with LiFePO4 3S1P 4,4A(4 of them) from hobbyking.  They are more stable than the Lipos, they wont explode but you still need to watch them.  They are about half the price of a 18650  spacecell type battery if it comes down to cost.  Then I upgraded to Spacecell and can now go to work and back 16 miles on one charge. There are people on the forum that will make you one for the same price as the spacecell in the US.

ESC - started with hobbyking 150a (caught on fire), DIY Electric Skateboards 6s esc(stopped working half way to work), and hobbywing(still works but very loud).  I finally got a VESC and will never go back.

Motor- I started with a hobbyking NTM prop 50 270kv and used that for about a year.  I didnt go real fast, I just wanted to cruise around and ride to work.  Then I upgraded to 2 of Ollin 50xx motors and damn they are fast and powerful.  You could probably get away with 1 of those motors or a 63xx motor I just liked the low profile of the 50xx motors.

Mounts - I ended up making my motor mounts for the Caliber 2 trucks and started selling them for 50xx, Ollin 50xx and 63xx motors

Pulleys - Every once in a while you can find a group buy or a good deal on a kit with the motor, wheel pulleys and harware to attach to the wheel.  I bought mine at DIY Electric skateboards, they were a good price and I am all about instant gratification when I want something.  They are also aluminum, I am old and not a big fan of the platic gears(even though they are glass filled and would probably be fine).

So to sum up - VESC (for sure), There are good motor options on the forum, you have a good , better, best option for batteries.
```

---
## \#12 Posted by: FoxxyPants Posted at: 2017-02-24T01:49:48.758Z Reads: 24

```
Would two of these work? https://hobbyking.com/en_us/turnigy-5000mah-3s-25c-lipo-pack.html
Again, I'm a bit uneducated on what the performance of 8s is compared to 6s, so sorry if these are really obvious or dumb questions.
```

---
## \#13 Posted by: JLabs Posted at: 2017-02-24T02:04:56.579Z Reads: 25

```
The higher the voltage 8s is higher than 8s the more 'power' and top speed you will have.
```

---
## \#14 Posted by: FoxxyPants Posted at: 2017-02-24T03:09:21.774Z Reads: 22

```
Oh so since the battery I chose is only a 4s I wouldn't be getting that much power or speed out of it?
```

---
