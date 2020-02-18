# Esk8 alternator/ Onboard generator

### Replies: 42 Views: 799

## \#1 Posted by: Jaeson Posted at: 2018-12-18T15:25:00.621Z Reads: 213

```
Hey guys I was wondering what some of you think about the possibility of creating an alternator or generator to charge our batteries while riding. In doing some research I found this:

http://sullivanproducts.com/product/s660/

Let me know if you guys think this concept can somehow work. I feel like if we could even give our ride 30% more distance, it would be a worthwhile addition. What do you guys think?
```

---
## \#2 Posted by: Bor.inc Posted at: 2018-12-18T15:36:18.415Z Reads: 209

```
Well the vesc offers regenerative braking so if you break the motors are used as a generator and give some power back to the battery

I dont realy know how that product works but if it is just a turning generator it wouldnt give something extra because by the laws of physics you cant have a perpetuum mobile.
```

---
## \#3 Posted by: Jaeson Posted at: 2018-12-18T15:42:08.829Z Reads: 203

```
Yeah but regen gives back seemingly very little. I’m not thinking of reproducing the same amount of energy spent, just sending the battery some energy while it’s exhausting some. Wouldn’t this effectively give more distance? Although not infinite. 

Also, if you had two battery connections onboard, wouldn’t you be able to simply switch between a set of batteries “in use” and another set being charged. 

Btw, I am by no means an electrical engineer, and that may be very obvious, please go easy on me if I seem dumb. I’m attempting to learn via poor mans education. Lol.
```

---
## \#4 Posted by: Itsmedant Posted at: 2018-12-18T15:45:06.504Z Reads: 186

```
You are never going to truly get back the same amount of energy. You will loose a good amount through heat with something like this.

I think with the range newer batteries can give us, there's really not a huge point (unless science of course) to start putting these on our boards. Tech needs to catch up with that type of stuff before its truly efficient.
```

---
## \#5 Posted by: Jaeson Posted at: 2018-12-18T15:46:51.311Z Reads: 178

```
Yes! Science, relative to experiment, to create better tech is exactly my goal.
```

---
## \#6 Posted by: Itsmedant Posted at: 2018-12-18T15:47:59.998Z Reads: 165

```
Necessity is the mother of invention my friend.
```

---
## \#7 Posted by: Jaeson Posted at: 2018-12-18T15:48:21.637Z Reads: 160

```
I love that saying!
```

---
## \#8 Posted by: Itsmedant Posted at: 2018-12-18T15:49:33.367Z Reads: 156

```
Yea, that thing is gonna need to get way more powerful to be able to truly make a difference.
4.8v DC and 500ma? (I think thats what I read)

It may be enough to power some lights or something like that.
```

---
## \#9 Posted by: Jaeson Posted at: 2018-12-18T15:54:03.873Z Reads: 152

```
Yeah, but it also says you can have them make it capable of 13.xx volts, I was just thinking and researching and thought that generator might spark an idea for a concept that might benefit esk8. 

Alternatively I was thinking about a hollow front axel with a ring and pinion gear, the pinion shaft could come out behind the front truck and turn a belt driven super small alternator. 

I have no idea if this would even be efficient but I’m trying to put it out there to see if one of the electrical geniuses can create a forever battery for us.
```

---
## \#10 Posted by: Hummie Posted at: 2018-12-18T16:02:08.392Z Reads: 147

```
Converting chemical energy to electrical,  as is done in a battery, is very efficient.  Converting from mechanical energy to electrical or vise vesa with a motor, as this thing does, isn’t as efficient but more important this passively gotten energy you’d get using this would be a loss of course and not free and this device creates some drag.  You’d be more efficient just running electrical stuff straight from the battery.  In a case where you’d want to slow down, then the conversion this thing does would be a benefit but the regen brakes are likely more efficient 
If looking for a source of free energy whilst riding.  ..the heat of the motor could be converted to electrical energy or the flexing of the deck and there’s electronic gizmos that do that conversion and would be with no net loss. The heat from the motor is lost energy anyway so you’d be making a more efficient system

I forget the name of the device that creates electricity due to the different temp but they’re built already and just have to mount it on the motor somehow or the mount and wait till the motor gets hot then sit back and reap the rewards.
```

---
## \#11 Posted by: Jaeson Posted at: 2018-12-18T16:10:04.950Z Reads: 128

```
That is a very interesting idea! I want to talk more about this but have to head to work. Thank you for the advice and the food for thought! @Hummie
```

---
## \#12 Posted by: venom121212 Posted at: 2018-12-18T16:15:42.201Z Reads: 122

```
Unfortunately thermo transfer is wildly inefficient due to the natural insulation of air. What do you do for a living @hummie? This is twice now you have provided specific knowledge in a field not many know. Thermo electric generation or the seebeck effect is what you are referencing.
```

---
## \#13 Posted by: Hummie Posted at: 2018-12-18T16:18:29.886Z Reads: 123

```
O shit at three times I’m in trouble.  I’m a sub teacher

Wonder how much energy could be gotten back from a well placed one of these. But with as little air between the plates as possible. 

 Or a pezio (forget how u say or spell it) ..one of those bending quartz things, would do.  At least you could catch that energy while riding n not have to wait till after already hot.
```

---
## \#14 Posted by: Deodand Posted at: 2018-12-18T16:25:00.910Z Reads: 122

```
Yeah, the skateboard already does:

Chemical energy → mechanical energy
Mechanical energy → chemical energy

About as efficiently as you can. If you want to do something different to improve and add range you need to switch the source and/or the storage mechanism as hummie mentioned. For instance a flywheel that you spin up on braking and store mechanical energy as mechanical energy. There's some cars that do this. Something that injects water into hot motors and powers a turbine with the resulting steam similar to turbo charger. Ultimately the biggest place to recover lost energy is heat, but heat is one of the lowest quality energy sources so you won't see much gains trying to recapture it and the mechanisms will be pretty complex.
```

---
## \#15 Posted by: Hummie Posted at: 2018-12-18T16:37:06.160Z Reads: 116

```
This thing is just cool
https://www.moosejaw.com/product/brunton-hydrogen-reactor-portable-fuel-cell_10245384

But want an ethanol one 



https://www.digikey.com/product-detail/en/marlow-industries-inc/EHA-PA1AN1-R03/1681-1087-ND/7537072
```

---
## \#16 Posted by: venom121212 Posted at: 2018-12-18T16:50:07.562Z Reads: 112

```
I'm looking forward to taxi'ing on neighbors golf carts when my unity arrives. It'll be great to be going 25 mph around the park while charging my battery. @Deodand, do you/the unity have preference over discharge and charge BMS vs discharge only? Someone mentioned that a discharge only bms can't handle brake regen but I don't buy it. Can you set me straight?
```

---
## \#17 Posted by: Deodand Posted at: 2018-12-18T16:54:51.463Z Reads: 111

```
If you have the money and space in your build charge/discharge is ultimately safer (if it's a quality bms). Problem is the bmses aren't always designed with ekate in mind, so certain scenarios can cause the board to cut power on you which is a potential safety issue. 

The unity was designed with charge only bypassed bms in mind. I prefer the simplicity of such a setup, but you just have to be careful to check your cell balance from time to time and make sure your charger is doing it's job. This is true in either case but a discharge bms should cut power on you if the pack is out of balance badly where's charge only won't.
```

---
## \#18 Posted by: venom121212 Posted at: 2018-12-18T16:57:12.595Z Reads: 109

```
Thank you for the clear and prompt response. Can't wait to get my unity Thursday :grin:
```

---
## \#19 Posted by: swimmydude Posted at: 2018-12-18T17:46:47.794Z Reads: 103

```
Boo!! Mine is due Friday. No fair! I bought mine first, isn't that how it's suppose to work? I'm gonna complain for a couple of more sentences. That'll really show how upset I am and how unfair life is. Booooooo
```

---
## \#20 Posted by: olestra Posted at: 2018-12-18T18:13:20.931Z Reads: 98

```
The linked generator is for rc models that run on gas-- it's just a way to get some electricity out of the fuel.
trying it on a already electric vehicle is... well, let's call it special.
```

---
## \#21 Posted by: venom121212 Posted at: 2018-12-18T18:55:23.137Z Reads: 91

```
To be fair, I ordered a few days before that and they charged me VAT tax so I had to cancel and reorder and that pushed me into the second batch by 2 orders. I think they felt bad so Carl helped me out. You're in the first batch though
```

---
## \#22 Posted by: Hummie Posted at: 2018-12-18T19:04:58.079Z Reads: 90

```
The linked generator runs on hydrogen. It wouldn’t be ideal as you’d have to find a source of hydrogen and can’t capture it straight from the air (don’t think).  But there’s a bunch of energy capturing devices that could be useful on a board with no losses to the system. Solar, piezoelectric, the thermoelectric jammy above
```

---
## \#23 Posted by: olestra Posted at: 2018-12-18T19:45:50.276Z Reads: 83

```
sorry, i was referring to the one linked in the first post. I'm pretty sure most methods of generating power won't be a net gain. I do know that the power cost to harvest hydrogen exceeds the energy gained by burning it
```

---
## \#24 Posted by: Hummie Posted at: 2018-12-18T19:52:25.849Z Reads: 82

```
Oo you were talking about that. 


It wouldn’t be burnt hydrogen though. Fuel cell. 

https://www.researchgate.net/blog/post/new-paint-product-can-harvest-hydrogen-energy-from-the-air
Maybe not it’s time yet but seems producing hydrogen is getting cheap n clean. Rather ethanol fuel cell though as it’s easy to handle and easy to make
```

---
## \#25 Posted by: AlanZhou Posted at: 2018-12-18T19:58:48.929Z Reads: 83

```
energy dosdent get destroyed or created it only gets turned into another form, so that means that you would get back very little usable energy.

most of it would be turned into heat and the drag from the alternator belt would chew up alout of energy too
```

---
## \#26 Posted by: skatardude10 Posted at: 2018-12-18T20:16:31.282Z Reads: 85

```
Check out this thread. https://www.electric-skateboard.builders/t/range-extender-plugged-into-charge-port/64327?u=skatardude10 Most people just carry extra batteries connected to a boost converter to boost to charge voltage, and charge while riding that way. 

95% of the time I'm riding I'm charging at 5 amps at the same time constantly. At the end of group rides I'm always at 90-98% battery while most others are dead. 

Another benefit to charging while riding is reduced voltage sag! 5A towards my power output helps noticably with my 25R pack.

Anyways, just having an extra battery to strap to your board seems a lot easier than carrying a generator with fuel. Plus, that generator by default can only do 4.8V at 800mA, or 3.8W, upgradeable to 4W... While my boost converter does 200W easy and it's the size of a focbox, but taller with the heatsink. I'd say 100W is the lowest I'd want to go for charging while riding.
```

---
## \#27 Posted by: longhairedboy Posted at: 2018-12-18T21:03:22.036Z Reads: 79

```
instead of bogging down your forward motion with more resistance by trying to extract electrical energy from it... essentially regen braking... 

maybe try using something like a larger magnet motor to spin a smaller generator.
```

---
## \#28 Posted by: AlanZhou Posted at: 2018-12-18T21:16:36.897Z Reads: 78

```
only problem with that is that more bms weren't designed to be charged and discharged at the same time even though it can can be done
```

---
## \#29 Posted by: TowerCrisis Posted at: 2018-12-18T21:23:12.606Z Reads: 74

```
It's at least impossible for a given wire to have current flow in both directions. A BMS that has one set of negative side wires (shares charge and discharge connection) will not charge through it when being "boosted". It will simply split the load between each pack.

Can't speak for BMS's with a dedicated charge port though. Those seem special.
```

---
## \#30 Posted by: AlanZhou Posted at: 2018-12-18T21:25:49.843Z Reads: 73

```
Most bms have separate change and discharge leads especially the cheap ones off of ebay.
```

---
## \#31 Posted by: dareno Posted at: 2018-12-19T03:15:59.708Z Reads: 64

```
[quote="Itsmedant, post:6, topic:78344, full:true"]
Necessity is the mother of invention my friend.
[/quote]

I would argue that conflict is.
```

---
## \#32 Posted by: Deodand Posted at: 2018-12-19T05:04:38.861Z Reads: 61

```
Or just boredom.
```

---
## \#33 Posted by: dareno Posted at: 2018-12-19T05:06:40.329Z Reads: 61

```
Nothing moves technology faster than a war.  Sad but true.
```

---
## \#34 Posted by: Deodand Posted at: 2018-12-19T05:07:49.730Z Reads: 59

```
People finally hand over the big monies for science when its time to kill eachother.
```

---
## \#35 Posted by: dareno Posted at: 2018-12-19T05:11:06.059Z Reads: 61

```
Nail on the head there fella
```

---
## \#36 Posted by: Kug3lis Posted at: 2018-12-19T05:54:47.145Z Reads: 59

```
Yo guys just buy this it's bit expensive but would propel you forever on the board never would need to charge.

![8A4BD19E-263A-4892-A120-4DBEAFECD7CA|500x330](upload://7upI8NwjRqI50OlbHIHAYII9Kj4.jpeg)
```

---
## \#37 Posted by: dareno Posted at: 2018-12-19T06:20:45.085Z Reads: 55

```
Is that iron mans heart?
```

---
## \#38 Posted by: Kug3lis Posted at: 2018-12-19T06:35:06.598Z Reads: 56

```
Nah that's arc reactor... In iron man movie it's a fake.

/s
```

---
## \#39 Posted by: Hummie Posted at: 2018-12-19T06:41:46.966Z Reads: 53

```
Has it actually worked practically. Fusion. 
https://www.google.com/amp/s/www.dailymail.co.uk/sciencetech/article-3202618/amp/Fusion-power-decade-MIT-reveals-small-reactor-claims-create-limitless-amounts-energy.html

“Up until now, however, the magnetic coils responsible for producing the magnetic fields have proven to be a huge bottleneck in the process.

The ARC reactor is slightly different to other tokamak systems in that it uses new commercially available superconductors made of rare-earth barium copper oxide (REBCO) superconducting tapes.”
```

---
## \#40 Posted by: dareno Posted at: 2018-12-19T07:39:18.203Z Reads: 51

```
Shit I thought that was real.  So spiderman was not really bitten by a spider then?  I used to think you knew your stuff but after that comment .....
```

---
## \#41 Posted by: lrdesigns Posted at: 2018-12-19T07:52:06.430Z Reads: 51

```
[quote="Jaeson, post:1, topic:78344"]
Let me know if you guys think this concept can somehow work. I feel like if we could even give our ride 30% more distance, it would be a worthwhile addition. What do you guys think?
[/quote]

Perpetual motion. No.  

If you could get 30% more power back into the battery it would take 35% more power to push it due to friction and electrical loses. 

Sorry.
```

---
## \#42 Posted by: AshR Posted at: 2018-12-19T11:11:38.602Z Reads: 46

```
You're nearly better off, wearing less clothes, losing weight on you or what you're carrying than what you would recover trying to gain power back from the board. 

The only reason an alternator works is because it's only charging a batter and running ancillary systems in a car. The petrol is what propels the car. 

If you had a petrol powered skateboard, then running a generator off this to charge the elec start battery would work.
```

---
