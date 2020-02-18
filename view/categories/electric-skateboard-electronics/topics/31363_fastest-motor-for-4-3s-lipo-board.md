# Fastest motor for 4 3s lipo board

### Replies: 22 Views: 1238

## \#1 Posted by: stormboard Posted at: 2017-08-24T02:23:15.571Z Reads: 118

```
what the fastest motor for a 4 3s lipo board build. and what fly whel pulley setup for abec 9 or 11 wheels on caliber 11s
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-08-24T02:29:00.268Z Reads: 121

```
I need some more info. 
Are you running your batteries in series?
Do you need a lot of torque? 
Fast is relative, what is fast to you?
```

---
## \#3 Posted by: wafflejock Posted at: 2017-08-24T02:29:48.244Z Reads: 119

```
Abec bearing ratings only go up to 9, the Abec 11 wheels are just named after a joke from spinal tap ("but ours go to 11").  Regarding motor speed the kv tells you the top speed without load, a 149kv motor does 149 rpm per volt applied, 190kv motor does 190 rpm per volt applied.  So you have a 12S battery then nominal voltage at 3.7V per cell you have 44.4V * lets say 190 = 8,436 rpm.  You also have to keep in mind with an older VESC (4.12 ones or FOCBox) you might run into the 60,000 erpm limit since there are multiple poles (14 I believe) in brushless DC motors and the coils fire in pairs so it moves the motor to 7 locations 8,436 * 7 = 59,052 erpm, so basically you go any higher on kv or voltage (which you will be when fully charged) and you could blow the DRV chip (it is supposed to work up to 100k I believe but in the 4.12 arrangement only works to 60k erpm before it blows).

---

The kv values are also based on no load speed, so given load you will need more or less actual power to turn the wheels.  The turning force on a wheel is called torque, torque at a given RPM is power (mechanical power).  The motor converts the electrical power (wattage) into mechanical power at about 80-90% efficiency (burns off the other 10-20% as heat from friction and resistance in the coils).

---

Also once you know your pulley parameters and wheel diameter and everything you can pretty easily and accurately calculate your top weighted speed http://calc.esk8.it/
```

---
## \#4 Posted by: stormboard Posted at: 2017-08-24T02:46:06.513Z Reads: 102

```
abec 9s so haha ya in series about 14 stone 25-30mph or do i need go dual. using vesc or focbox ya. wondering what pulley flywheel teeth setup do i need
```

---
## \#5 Posted by: wafflejock Posted at: 2017-08-24T02:54:41.955Z Reads: 94

```
Sorry can't really speak to that, I'm only about 115-120lbs or apparently 8.5 stones and my board tops out at 21mph, I have a 149kv motor with a 10S battery.

This is basically my setup except I have a 10S not 12S:

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":149,"system-efficiency":85,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":83}|

I get the 21mph it calculates for my build but I'm also a lighter dude.  The higher in kv you go typically the lower torque you get (assuming same wattage and all else), also if you have shorter magnets/rotor size then you are typically losing torque.  So the 6374 SK3 is what I have it's a beefy motor great for single motor setups but would have a tough time putting two of them onto one truck you'd either need to have them sticking out the sides or one up front one in back, but one is plenty for me personally.  If you're dealing with a hilly area I think dual will probably serve you better but have let plenty of dudes two or three times my size jump on my board and not have a problem in terms of it accelerating too little.

I would reconsider on the top speed unless you're already an adept down hill skateboarder, plenty of people on the forums here with injuries and hospital bills or days laying in bed eating pills trying to recover.  I think 149 with 12S is a pretty good combo if you really want that top end can go 192kv or whatever you can find around 190 but tend to be a little harder to come by it seems.

---

**Edit** apparently I could speak to that :)
```

---
## \#6 Posted by: ShutterShock Posted at: 2017-08-24T14:16:26.419Z Reads: 70

```
[quote="wafflejock, post:5, topic:31363"]
apparently 8.5 stones
[/quote]

lol same :joy:

On my setup, I am running 190kv on 12S.  Works great for me so far and I have managed to hit the "theoretical" top speed at 29.6mph with a 16:36 gear ratio.  It's scary fast and I would have been fine going with a lower kv like 149 like @wafflejock says.

For reference, I am about 140 lbs or... 10 stone :stuck_out_tongue:
```

---
## \#7 Posted by: stormboard Posted at: 2017-08-24T16:03:41.655Z Reads: 63

```
190kv it it is
```

---
## \#8 Posted by: ShutterShock Posted at: 2017-08-24T16:14:31.651Z Reads: 56

```
Fair warning, 29mph is really fast. Wear a helmet
```

---
## \#9 Posted by: stormboard Posted at: 2017-08-24T16:29:52.367Z Reads: 54

```
sound bud but a motorbike at a 150 is worse haha
```

---
## \#10 Posted by: ShutterShock Posted at: 2017-08-24T16:43:19.187Z Reads: 55

```
Lmao game beat.  :joy::joy:
```

---
## \#11 Posted by: Deckoz Posted at: 2017-08-24T17:05:28.578Z Reads: 48

```
I'm running 10s dual 190kv and weigh 127lbs or about 8.5 stones as well on a 16/36 on 83mm and have maxed out at 31 under power, and 43 down hill. About to switch to 40/16 and 90mm. Either way when I ride fast I wear all the gear

TSG Pass - full face
TSG DHP Knees
Hillbilly padded shorts with Tailbone
TSG Force 4 Elbows
Slide Gloves
Dakine backpack with spine protector.

150 on a motorbike could be worse...but you have no bike in the way to protect you when you go down. Its all body on a longboard. So I wouldn't shrug off 20, 30 or even 40mph like its nothing compared to a bike..you're more exposed, wear gear.
```

---
## \#12 Posted by: wafflejock Posted at: 2017-08-24T17:05:59.707Z Reads: 47

```
Yeah thing is the motor bike has suspension and tires, unless you go mtb build you're relying on urethane and whatever trucks you bought to not explode and your legs/ankles to not wobble out and whatever transmitter/receiver you have to function properly... basically lots of crap can and likely will go wrong so just be sure to protect the noggin you'll need it to rebuild.
```

---
## \#13 Posted by: stormboard Posted at: 2017-08-24T17:25:01.496Z Reads: 44

```
ill get a helmet anyway case hit a pothole ir something
```

---
## \#14 Posted by: stormboard Posted at: 2017-08-24T17:28:56.555Z Reads: 44

```
so what sites should my stuff from in a europe
```

---
## \#15 Posted by: wafflejock Posted at: 2017-08-24T17:32:37.819Z Reads: 43

```
I'm in the US but think hobbyking is a good place to shop for batteries and motors since they typically have best prices but depends on what you want really.  I got my pulley motor mount and trucks from  but you can definitely find better deals if you piece things together yourself (convenience vs money).  Think for skateboard components themselves you're best off trying to find some local shops so you can actually try things out otherwise I also bought some blank decks on Amazon just make sure you understand the space you need for the battery and ESC you go with and everything... basically good to search for "build threads" in the forum here and take a look at what components other people ended up with and maybe search for 190kv or 192kv builds in particular.
```

---
## \#16 Posted by: stormboard Posted at: 2017-08-24T17:57:05.627Z Reads: 36

```
what 3s lip battery would you choose from hobby kings ? puttin 4 ogmf them in series
```

---
## \#17 Posted by: wafflejock Posted at: 2017-08-24T18:01:14.644Z Reads: 40

```
Can use the product finder to narrow down your options based on how much juice you want to lug around and how much distance you want.  Roughly 10Wh = 1km, so say you go 5Ah * 12S * 3.7V = 222Wh (about 22.2km).  Keep in mind when you go in series you increase voltage but Ah is shared so 3S 5Ah 4 in series gets you the config above.

https://hobbyking.com/en_us/lipo.html?config=53&capacity=3855-10120&discharge=36-110&

Just make sure your discharge rate is above what you expect to ever draw to power the motor, say you have a 2200W motor and a 12S (44.4V) setup, then 2200W / 44.4V = 49.5A.  For C ratings it's the Ah * C rating = max discharge, so 5Ah 40C, is 5 * 40 = 200A max discharge which leaves a good amount of head room.  The higher the C rating the lower the internal resistance and heat build up in the battery and the less voltage sag when under load so always shoot for higher (price permitting).

---

Also I never actually hit that high a discharge rate myself as far as I know, peak I've seen is around 20A or so (maybe 25A) on accelerating with a 10S setup but could have been a faulty ammeter I can't say for sure, have seen other people pulling 40A but not sure what voltage that was at, still always good to be able to supply more power than the system needs.
```

---
## \#18 Posted by: ShutterShock Posted at: 2017-08-24T21:11:09.190Z Reads: 33

```
Personally, I ended up using the Zippy Compacts, because of size compared to the Flightmax, 4 3S 25C 5000mAh.  They ended up being the best price and performance split for my setup, and they've worked great so far. :slight_smile:

But like waffle said as well, you can always shoot higher, like 30C+ but it wasn't gonna be worth it for me
```

---
## \#19 Posted by: StormTrooperBert Posted at: 2017-09-19T04:46:11.178Z Reads: 30

```
Curious to know your wheel size? Running VESC? I'm running a single 190kv on 12s 16:36 on 90mm wheels. Took it for the first run on 12 last night and hit 36mph. Could've easily hit 40 but got speed wobbles 😂😂 oh! And I weigh 215lbs.
```

---
## \#20 Posted by: ShutterShock Posted at: 2017-09-19T06:37:35.523Z Reads: 30

```
I run 83mm wheels that I got with the kit from DIYElectric, they are a little hard but they do the job just fine.  I am also now running dual vescs, dual 190kv, 16:36 and I haven't dared to hit top speed.  I hit 30 and got speed wobbles even in a speed tuck, but I know it can go faster :joy:

Scary fast but sooo awesome.
```

---
## \#21 Posted by: stormboard Posted at: 2017-09-19T06:43:02.801Z Reads: 26

```
so how many zippy compacts did you buy in total?
```

---
## \#22 Posted by: ShutterShock Posted at: 2017-09-19T15:43:06.192Z Reads: 23

```
I bought 4 3S ones to make a 12S1P pack. I chose the compacts because they fit on my board better
```

---
