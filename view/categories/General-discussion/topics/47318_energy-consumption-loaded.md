# Energy consumption loaded

### Replies: 33 Views: 1585

## \#1 Posted by: Sirshaunsta Posted at: 2018-02-24T07:12:08.187Z Reads: 216

```
So I'm looking for some advice from anyone knowlegable about this topic, hypothetically if a 5000mah 37v battery had a tested range of 15km, a 40 000mah 37 would deliver 120km range using the same single motor in theory. Now adding a motor relieves the stress on each motor dividing the load by 50%  meaning they each draw less amps to achieve the same speed as the single. My question is If dividing the load by 4 and making a single 10 000mah 37v battery for each motor would still deliver 120km because of the lower needed amps in each motor, or if I would merely have insane power for 30km? @GrecoMan @psychotiller @scepterr
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-02-24T08:32:03.163Z Reads: 203

```
It wont matter if you have pack in one, or split up in four. The Wh will still be the same, and your range will too. 
But remember that 1 motor/ single drive, is more efficient than 4 motors/ awd..
```

---
## \#3 Posted by: Sirshaunsta Posted at: 2018-02-24T09:30:12.296Z Reads: 184

```
I don't understand how the efficiency drops yet, are you able to explain it? @FredrikHems
```

---
## \#4 Posted by: ducktaperules Posted at: 2018-02-24T10:17:05.023Z Reads: 176

```
in general larger motors are more efficient than smaller motors so 1 larger motor should be more efficient than 4 smaller motors. However if your just adding more larger motors i wouldn't think this should apply.

Also a a setup with 4 motors is probably heavier and will have a lot more friction from 4 sets of belts or gears.
```

---
## \#5 Posted by: FredrikHems Posted at: 2018-02-24T10:43:40.452Z Reads: 153

```
Its mainly because some of the energy going to the motor will end up in heat, and heat=energy. 
However, with 37v 40Ah, i dont think you should worry :wink:
```

---
## \#6 Posted by: Sirshaunsta Posted at: 2018-02-24T12:08:32.810Z Reads: 145

```
Four  6364 - 190kv powered by 40ah split into 10ah packs to each motor. 20/32 gearing and 97mm wheels. the board weighs just under 20 kg/40lbs and I weigh 160, I doubt the 4 will have any trouble pushing 100kg/200lbs. I just want to know how the displaced load will effect my riding/battery usage
```

---
## \#7 Posted by: Sirshaunsta Posted at: 2018-02-24T12:09:41.177Z Reads: 138

```
That's where I get stuck, while the belts cause rolling resistance, if I'm lowering the load to each motor wouldn't I get less heat in my motors? Thus making them MORE efficient? Also im using lipo, so that 37 is really 41/42v ;)
```

---
## \#8 Posted by: Sirshaunsta Posted at: 2018-02-24T12:21:45.771Z Reads: 130

```
Yes it's enough to make a small bomb ;)
```

---
## \#9 Posted by: FredrikHems Posted at: 2018-02-24T12:25:21.492Z Reads: 128

```
You are right that per motor it will be more efficient, BUT since you have four, together they will be more inefficient.

Li-ions does also go to 4.2V/Cell, but we use 3.6(Li-ion), 3.7(Li-Po) because that is the nominal voltage.
```

---
## \#10 Posted by: Sirshaunsta Posted at: 2018-02-24T12:26:35.376Z Reads: 128

```
How though, with each one don't I improve its ability to hit full speed with less drawn power(amps)? @FredrikHems
```

---
## \#11 Posted by: FredrikHems Posted at: 2018-02-24T12:30:08.878Z Reads: 109

```
I am not sure actually. Maybe some others know..?
```

---
## \#12 Posted by: Sirshaunsta Posted at: 2018-02-24T12:31:46.140Z Reads: 107

```
I just wonder because a single motor might draw 30 amps to propel up a hill where as with 2 it would divide the load making each draw 15 instead,  I'd think this effect continues the more you add wouldn't you? @FredrikHems @GrecoMan @psychotiller
```

---
## \#13 Posted by: krloz Posted at: 2018-02-24T14:00:24.450Z Reads: 101

```
You are not accounting for losses there.  You are missing the heat and friction produced in each motor which is also multiplied by each motor you add.
True more motors implies each will heat up less but in the end of one motor produces let's say 1 heat, 2 motors would produce around 0.75 heat each.  Totalling to 1.5 heat wich is more.
Yeah I'm using heat as a unit of measurement
```

---
## \#14 Posted by: onepunchboard Posted at: 2018-02-24T14:07:37.085Z Reads: 104

```
yeah but ur motor needs to overcome inertia and standing frinction everytime u acc or break. u will have more mass and friction with 4 motor and pulleys. now there is more surface area for heat to escape so it would be easier to be loose more energy. also nothing is perfectly same so there will be unequalibriam in each side of wheel=less efficiency.
not to mention all the resistance build up because of extra copper mass from wires. 
I probably have to do more research but I think it would be similar to sports car engine. u can increase only so much of diameter of piston or add piston before it eats gas like crazy.

of course the electrical motor is much efficient so it wouldn't be much different but it would certainly do less than just one motor. 

brushless motor is at best 95% energy efficient. so in 4 motor ur lossing about 15% in comparison to 1 motor.
```

---
## \#15 Posted by: krloz Posted at: 2018-02-24T14:10:25.457Z Reads: 88

```
So as in every comparison where both options both have pros and cons the only way to find out for certain is...
Go at it..... for science!!!!
O And measure, it wouldn't be science then
```

---
## \#16 Posted by: Sirshaunsta Posted at: 2018-02-24T14:24:03.371Z Reads: 86

```
I like the sports car reference, aren't most of them 4wd? ;) you are right though in cars a 4wd uses more power than 2wd but also the given power to ground ratio grows significantly in comparison
```

---
## \#17 Posted by: Sirshaunsta Posted at: 2018-02-24T14:24:37.423Z Reads: 90

```
I will just have to go at it and see I guess
```

---
## \#18 Posted by: onepunchboard Posted at: 2018-02-24T14:43:04.062Z Reads: 85

```
most sports cars are 2wd rear i thnk. but yeah 4wd has more torque and traction but use more fuel, tho it is mechanical so not sure if u can compare.
```

---
## \#19 Posted by: ducktaperules Posted at: 2018-02-24T18:22:24.837Z Reads: 79

```
4wd car is a bad example cause it still only has 1 engine. 

You are right that If you have 1 motor at 30A its the the same as 2 motors at 15 amps, or 4 at 7.5 amps. in an ideal world your amps for the whole board are the same and your watts will be the same. 

With regards to heat,Imagine 5% of that 30A is lost as heat. 5% of 30A is more than 5% of 7.5A so in a 4 motor system each motor runs cooler. however there are 4 motors the amount of energy being converted to heat is the same either way. 

Also in the real world each motor has resistance, each bearing has resistance and each belt has resistance. 4 motors and drive systems will have 4 times as much resistance to overcome and resistance costs in efficiency.

Going back to the car reference, this is why almost all electric cars use 1 large motor instead of separate hub motors in each wheel. This is also why helicopters are very common but full size multi rotors are quite rare.
```

---
## \#20 Posted by: Sirshaunsta Posted at: 2018-02-24T23:20:46.452Z Reads: 71

```
Thank you that actually helped. @ducktaperules
```

---
## \#21 Posted by: pakue Posted at: 2018-02-25T00:03:48.994Z Reads: 73

```
From an electrical point of view 4 motors should be more efficient as heat-loss is caused by amperage and voltage drop. The voltage drop increases linearly with current therefore the heat-loss rises exponentially with higher current.

For example:
R<sub>motor</sub> = 0.1&Omega;
I<sub>motor</sub> = 30A

P<sub>loss motor</sub> = U<sub>voltage drop</sub> * I<sub>motor</sub>
U<sub>voltage drop</sub> = R<sub>motor</sub> * I<sub>motor</sub>
=> P<sub>loss motor</sub> = R<sub>motor</sub> * I<sub>motor</sub><sup>2</sup>

1 Motor:
0.1&Omega; * 30A<sup>2</sup> = 90W 

4 Motor:
4 * 0.1&Omega; * 7.5A<sup>2</sup> = 22.5W 

Mind you the values are just guesses and the "gain"  in efficiency from more motors will likely be eaten up by the mechanical resistances, but for direct drives this may be a net gain.
```

---
## \#22 Posted by: Sirshaunsta Posted at: 2018-03-01T12:52:04.126Z Reads: 59

```
So by your example I would end up using the same 90w but the heat will be reduced by 75%? @pakue meaning cool running motors at all times and ample power to be tapped at any time being my 3.2 torque would become 12.8 and my motors would be able to achieve a higher weighted rpm while staying cooler than a single drive
```

---
## \#23 Posted by: pakue Posted at: 2018-03-01T13:11:32.599Z Reads: 55

```
In that example I was just calculating with the heat loss (90W for the single setup). The actual power you pump in is obviously higher, maybe 500-1000W, but that is what gets you moving (TotalPower = HeatLoss  + MechanicalPower). 
The total torque in my example would stay the same as you are still giving a total of 30A (thats what determines the torque of the motor), which are just spread over more motors. If you would want the 12.8 Nm in total **each** motor needs 30A and the heat output is again 90W **per** motor. 
Under the same conditions a 1WD will always generate more total (electrical) heat than a 4WD.
```

---
## \#24 Posted by: Sirshaunsta Posted at: 2018-03-01T14:16:40.219Z Reads: 52

```
Yes, that is what I thought, this build will enable 60 amps to each motor as 4 batteries are 10s 10ah each @pakue motors are rated to 2450w and 65amp each but i figure a limit of 60  amp through vesc should be safe. Battery total is 1480w/h and each pack has a 200-300amp ability
```

---
## \#25 Posted by: Sirshaunsta Posted at: 2018-03-02T04:26:33.171Z Reads: 53

```
@pakue as you've been the only one to show you know the science involved, do you concur with my estimation that this build will be able to travel up to and over 100km/70m range on a single charge whilst overcoming hills and hitting speeds in excess of 40km/25mph
```

---
## \#26 Posted by: E1Allen Posted at: 2018-03-02T04:52:47.189Z Reads: 53

```
Don't forget if you draw less continuous amps from your batteries you will increase your range as well🤔🤔🤔 more to think about...
```

---
## \#27 Posted by: Sirshaunsta Posted at: 2018-03-02T05:00:57.129Z Reads: 55

```
I love when people hit me with nice news @E1Allen
```

---
## \#28 Posted by: Sirshaunsta Posted at: 2018-03-03T06:36:44.758Z Reads: 52

```
Yes, that was my hope because a 10ah battery would probably only give me 30km range with a single motor, my hope is using 4 I will increase the range 400%
```

---
## \#29 Posted by: Sirshaunsta Posted at: 2018-05-01T10:34:23.527Z Reads: 44

```
Quick update guys![20180414_163151|374x500](upload://h5yfXCUoHqcuVMxq77vcHQ5p5J.jpg) this is almost the whole 4wd setup assembly, now all I need is my 4 motor mounts belts and pulleys.
```

---
## \#30 Posted by: sismeiro Posted at: 2018-09-14T16:13:52.418Z Reads: 32

```
Hi, isn't the lengh of the adapter cables and all the connectors be bad for the amps that are going to flow through them?
```

---
## \#31 Posted by: Pantata Posted at: 2019-02-15T17:10:12.499Z Reads: 26

```
I am not sure If I get you correctly. You do not get double the range with 2 motors instead of 1 or 4x the range with 4. It's just that using 1 motor for the same amount of work instead of 4 will be less efficient. By some percents, several, maybe even 10+.
```

---
## \#32 Posted by: Pantata Posted at: 2019-02-15T17:15:36.362Z Reads: 24

```
not really but you really need to know your stuff to be able to calculate what the differences are. Longer cables mean more heat, connectors mean more heat... 2 motors are more efficient than one... Yep... But unless someone like pakue shows you the real calculations and specific examples you have no clue how important that difference between having 2 feet of wires vs 1 foot and having 3 plugs vs 5 will make. In most cases it doesn't matter. But to know for sure you need to understand everything there is about  it.
```

---
## \#33 Posted by: Hummie Posted at: 2019-02-15T18:02:40.693Z Reads: 23

```
It’s not complicated. :::::: I^2R ::::::losses (current squared x motor resistance) are by far the biggest loss and four motors will allow a much lower squared current number in what would be then four equations reducing ultimate losses.  So other than friction increasing from multiple belts and pulleys (which could vary greatly) having more motors is going to be more efficient.

  Cables and plugs will have the same I^2R losses and the more motors and wiring and escs you have the less current they individually have to transfer so more efficient for the same power output compared to a single motor, wiring, and esc.
```

---
