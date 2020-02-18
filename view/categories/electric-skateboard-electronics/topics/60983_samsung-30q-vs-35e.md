# Samsung 30Q vs 35E

### Replies: 23 Views: 5057

## \#1 Posted by: untitled Posted at: 2018-07-05T18:25:42.062Z Reads: 432

```
Looking for some expert advice on which battery pack to build or buy. Price seems about the same. Is the 35E a newer version of the 30Q? or the other way around. Looking for low end torque as opposed to high speed, although I know this can be accomplished with a good VESC or even mechanically with gearing. Any advice from those who have experimented?
```

---
## \#2 Posted by: JohnA Posted at: 2018-07-05T18:44:08.111Z Reads: 424

```
The 30q is a battery that’s rated 3000mah and a 15 amp max continuous draw, the 35E is 3500mah and 8 amps max continoious draw. So you gain 500mah capacity but get half of the current ability of the 30q. If you put enough in parallel though you could make the 35E work, but for our application with limited battery space I would go with higher output cells.  Especially if you are looking for high torque and acceleration because that will be directly related to how many watts your system can pull from the battery. (Watts = voltage * current).

The 35E is just another battery model that Samsung makes, they offer a wide variety of different capacity batteries with different max continuous currents. The 30q has proven a great cell for our application with up to a 20 amp max current draw with a very slim voltage drop under high loads.
```

---
## \#3 Posted by: bartroosen12 Posted at: 2018-07-05T18:48:59.975Z Reads: 401

```
It depends on what kind of pack you gonna build.
The 30Q cells are good for 15A continue discharge while the 35E are good for 10A continue discharge.
![IMG_20180705_204557|690x388](upload://3xFfqi2oEJUuZkQHGbJFeBr2rI8.jpg)
You can clearly see a lot of voltage drop at 15A with the 35E. Even with 10A the 30Q is just better, as you can see on the picture below.
![chrome|690x388](upload://2QALL82RjaB6BlMAL5rcwUuRlt7.png)
Voltage drop is directly related to your speed, so you will get a lower max speed when you ride with the 35E batteries.
I think the range would not be much different.
```

---
## \#4 Posted by: Benjamin899 Posted at: 2018-07-05T19:24:05.443Z Reads: 341

```
35e just doesnt cut it, you don't even safe money because they cost almost the same. 35e will run hotter the more amps you pull, more heat and hence more internal resistance......heat kills your pack. But dunno, where you live or where you want to ride, how heavy you are ect ect. Everything is possible if done right.
```

---
## \#5 Posted by: Pedrodemio Posted at: 2018-07-05T20:00:42.987Z Reads: 315

```
The capacity is not less, but the energy is way less, so at the same high current you can go farther with the 30Q

The energy is the area below the discharge curve, just looking we can see that at 15A the 35E have 1/2 to a 1/3 leds energy than the 30Q

That being said, the average current of most of our boards is pretty low, I average 8A, in a 3P pack that’s 2.7A per cell

If you don’t climb hills 100% of the time you probably be ok with the 35E in anything more than a 10S3P

My city is pretty hilly and I use 10S3P of NCR18650GA, which is basically the 35E equivalent from Sanyo/Panasonic. 30A battery current and I can climb 15% hills keeping my speed and a lot more at lower speeds (24% is the steepest I’ve found so far)
```

---
## \#6 Posted by: Benjamin899 Posted at: 2018-07-05T22:00:39.095Z Reads: 262

```
my average is 15A on a single drive 6374 motor 15/40 97mm wheel and i live in flat area, but on my way there is a 2-3% incline over 7km and going at a good speed pulls good amps with my 80kg. 
Did anyone build a board with lg he2 and has some real feedback?
```

---
## \#7 Posted by: Pedrodemio Posted at: 2018-07-06T00:27:10.394Z Reads: 235

```
This 15A is battery amps? Sound really high for the ridding scenario you describe

What speed do you ride?
```

---
## \#8 Posted by: Benjamin899 Posted at: 2018-07-06T00:46:57.104Z Reads: 217

```
30-40km/h, maybe lower, i just flew other my last log, sure there were passages with lower amps. There are always so many variables influencing those values. ah right i forgot, this is an 6s setup on a 245kv motor so that plays a role in it too.
```

---
## \#9 Posted by: Pedrodemio Posted at: 2018-07-06T01:35:09.819Z Reads: 204

```
6S would be higher. Yeah, just looking over is nowhere near average value, but I guess it's all good
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-07-06T10:30:32.026Z Reads: 173

```
i got everything here for my 10s setup...building is a bitch but so much fun too^^
```

---
## \#11 Posted by: untitled Posted at: 2018-07-06T12:09:32.058Z Reads: 162

```
Exactly what I was wondering - thanks for confirming.
```

---
## \#12 Posted by: Holyman92 Posted at: 2018-07-06T12:13:02.855Z Reads: 157

```
What about the samsung 20S? it only has 1Ah less than the 30Q but at twice the continuous amps.... with a 6P pack ur still getting roughly 46Km (~29 miles)
```

---
## \#13 Posted by: Benjamin899 Posted at: 2018-07-06T12:16:17.261Z Reads: 156

```
20S? Do you have a link, because i have never heard of that battery
```

---
## \#14 Posted by: Holyman92 Posted at: 2018-07-06T12:16:38.670Z Reads: 154

```
https://www.imrbatteries.com/samsung-20s-18650-2000mah-30a-battery/
```

---
## \#15 Posted by: Benjamin899 Posted at: 2018-07-06T12:18:57.298Z Reads: 149

```
not worth it for that pricetag, imo
```

---
## \#16 Posted by: Holyman92 Posted at: 2018-07-06T12:27:43.232Z Reads: 152

```
€317.10 = 371.78
![image|690x387](upload://lcWPYQoIlgx4AD2p5vIUqkPo7T0.png)
I live in the same city that IMRbatteries is based out of.. so 371$ and wait a month to get my cells or, 423.67 and have them the same day...

these prices are based on buying 100 30Q cells
```

---
## \#17 Posted by: Holyman92 Posted at: 2018-07-06T12:29:07.794Z Reads: 140

```
now keep in mind that NKON doesnt charge u import fees or anything... that is handled through fedex so there will still be more $$ that is gonna need to be paid :confused:
```

---
## \#18 Posted by: Benjamin899 Posted at: 2018-07-06T12:30:48.317Z Reads: 141

```
dude did you post your adress in that screenshot?
I don't buy on nkon. but even if i would, i live in germany, so i don't pay import fees.
But i am confused by your numbers, what is what now?
```

---
## \#19 Posted by: Holyman92 Posted at: 2018-07-06T12:35:46.129Z Reads: 136

```
i did haha... its all good i fixed it, and the difference in price between 30Q and 20S is $0.50 per cell its really not tht big of a diiference as far as price goes... idk, i think for a 4wd setup it could be worth it
```

---
## \#20 Posted by: Benjamin899 Posted at: 2018-07-06T12:44:05.876Z Reads: 132

```
oh wow didnt realise the 30q are also that expensive. i pay 3.30€/30q
```

---
## \#21 Posted by: Holyman92 Posted at: 2018-07-06T12:46:57.331Z Reads: 121

```
Yea, that's the cost from nkon, but shipping to the US plus customs is what drives the cost up... plus if u don't buy from a US supplier u usually have to wait a month or longer
```

---
## \#22 Posted by: faithfulpuppy Posted at: 2018-07-06T16:01:01.556Z Reads: 112

```
[quote="Pedrodemio, post:5, topic:60983"]
The energy is the area below the discharge curve, just looking we can see that at 15A the 35E have 1/2 to a 1/3 leds energy than the 30Q
[/quote]
the graphs have a break to 2.0V. In reality the difference is nowhere near that stark, that would just be a shit battery.
```

---
## \#23 Posted by: Pedrodemio Posted at: 2018-07-06T16:25:08.502Z Reads: 104

```
True true, I forgot that to look at the voltage scale, sorry
```

---
