# 10s?p battery for quad hub motor build

### Replies: 10 Views: 209

## \#1 Posted by: sammyg Posted at: 2019-11-13T03:06:52.104Z Reads: 62

```
Hi everyone!

I am currently building a 4 hub motor board that will later be used as the basics of a “micro-kart”... it’s for my senior thesis... but anyway!!!

4x maytech hub motors (100kv)
[https://maytech.cn/products/brushless-hub-motor-hall-sensor-motor-mto9055hbm-100-ha?variant=21911777574976](https://maytech.cn/products/brushless-hub-motor-hall-sensor-motor-mto9055hbm-100-ha?variant=21911777574976)

Each on their own Flipsky 4.12 VESC
[https://flipsky.net/products/torque-esc-vesc-®-bldc-electronic-speed-controller?variant=8712049918012&currency=USD&gclid=CjwKCAiAzanuBRAZEiwA5yf4uh6c-EhZNPzQgwgJeWx7uuQM7YKIBLgirQCGOSVoItuNbFRceNMHcRoCJaIQAvD_BwE](https://flipsky.net/products/torque-esc-vesc-®-bldc-electronic-speed-controller?variant=8712049918012&currency=USD&gclid=CjwKCAiAzanuBRAZEiwA5yf4uh6c-EhZNPzQgwgJeWx7uuQM7YKIBLgirQCGOSVoItuNbFRceNMHcRoCJaIQAvD_BwE)

And for now, all signaled by a single Flipsky remote via PPM (with only one ECS providing power)

My question is **if each motor can draw 22A max should I go for 10s4p? 10s5p? 10s6p???**

Thanks in advance and any comments or suggestions are welcome!!!
Sam G.
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-11-13T04:00:02.047Z Reads: 58

```
Depends on range and use, if you just want the power, get a lipo battery
```

---
## \#3 Posted by: sammyg Posted at: 2019-11-13T04:34:48.332Z Reads: 55

```
Range I don’t really care about.  I want to use the full ability of the motors. 

As far as use goes... this is a test bed for my later project of a “micro-kart” that uses this hardware.  I need response, power (as in torque), reliability and safety from this battery powering the 4 motors and there VESC.

I just want some input on the max continuous amps... (both batteries are built of 30Q cells)

10s2p is rated at 30A which means each motor is limited to 7.5A.

10s5p is rated at 75A which means each motor is limited to 18.75A which is very close to its 22A rating.
```

---
## \#4 Posted by: Fosterqc Posted at: 2019-11-13T05:13:43.698Z Reads: 50

```
This is something people get tripped up about early on. 

[quote="sammyg, post:3, topic:103842"]
input on the max continuous amps
[/quote]

You will have a very hard time pulling 22A from all motors for more than say, 1 second. Therefore the 10S5P/4P minimum I'd say would be suitable.

And what @ZachTetra said is good advice for a prototype build. Not clear if you already have the 30Q cells and ability to weld or something.  But even a cheap 10S lipo setup would give plenty of amps. Look for hobbyking sales, don't waste too much money on them if you go this route.
```

---
## \#5 Posted by: sammyg Posted at: 2019-11-13T05:25:22.339Z Reads: 44

```
Thank you

I had read that motors usually peak for short amounts of time and had kind of assumed that 18.75A to a 22A motor would be fine. 

Just wanted to be told that I wasn’t being wasteful and unrealistic for buying a 5p battery...  

This is my first DIY eskate and I am in it for some serious coin for what is essentially a school project and hopefully a hilariously fun awd go-kart.  I have made the mistake enough that when you cheap out, you end up paying more when you have to replace broken or weak stuff and want to do this right.
```

---
## \#6 Posted by: Fosterqc Posted at: 2019-11-13T08:58:53.978Z Reads: 39

```
Haha I actually went lipo for my first build. It was a $380 in parts + longboard single drive. It did not last long. 

Care to share something to illustrate your kart build? Interested to see the steering/size.
```

---
## \#7 Posted by: Sn4pz Posted at: 2019-11-13T11:32:12.525Z Reads: 37

```
10s5p Samsung 40t pack 

^ a very high discharge (meaning what each hub will be draining won't have a huge effect on the systems voltage), large capacity pack that should honestly get you 25miles of high-speed fun

I don't know how those hubs perform though 🤷

4p would be acceptable, but that's my minimum for a 4wd build
```

---
## \#8 Posted by: sammyg Posted at: 2019-11-13T13:33:52.585Z Reads: 34

```
Size will be around 27” wide and 40” long and the frame will be bent plywood like a skateboard but probably 3 peices for seat back and lower steering support.

The hubs have a keyed square in the motor so building an axle for them will be less complicated than the typical eBay hub motors that have a square axle protruding for you to lock into the truck... I have a sketch of my first idea but this will be a few months in the making.  The whole thing is really to explore the characteristics a user can control in an electric vehicle and make it more interesting... easiest way to explain it is what will manual drivers do with their hands when the world is mostly EV?  Tesla’s are fast but you have to like a big screen in tour face and little control.  Porsche Taycan is better but more could be done for the driving experience.
```

---
## \#9 Posted by: Airwolf Posted at: 2019-11-14T01:47:08.507Z Reads: 17

```
I have been working on a 4 wheel drive electric skateboard for some time now. Let me share a bit about where I'm at with my project.

#1: For me the most important concept in Reliability is this: Your Motors come with "Maximum Specifications" such as Max amps. Also, your Vesc will have "Maximum Settings" for many parameters. 

Do Not ever set your VESC to the Maximum Specifications for your Motor Wheels. I recommend trying everything at 77% to begin with. For example, if your Motor wheels are rated at 22 amps, try setting your vesc maximum motor current to 77% of 22 amps. 

There is a rule in electronics that is something like government your self at least 15% capacity above what you will actually need. For Reliability in ESK8, go 20 to 23%. Then slowly adjust 1 parameters at a time up from there. 
( * Some exceptions to this rule exist. Like for example, my motor wheels are rated for 12S, but I recently pared my 12S battery down to 11S for Reliability. 

The point im trying to make is: Dont go in on the first day with the mind set  that the 1st thing you want to do is make sure all of the advertised maximum specifications are correct to see what the true maximum power output can be like myself and everyone else does. Its hella expensive this way.



#2: The Documentation that comes with Vescs is usually minimal. However, I'd you go to the Website of the Original Vesc which was created by Benjamin Vedder, You will find Tutorials that basically define what the settings in the software are with more accuracy than almost any other source.

Be cautious because the original vescs are for 1 motor wheel only. You may or may not be using a Dual vesc. That Dual vesc may be using the same software for 2 motors, or may not. Just try to find some indication in the wording or try calling or emailig whoever's you get your vescs from and ask then to recommend some safe starting parameters or some average start iij ng parameters. There recommendation may clarify if the setting is for 1 wheel or for each.

#3: As for your "Maximum Regenerative Braking Current". Find out the maximum charging current for the specific type of battery in your pack. Now multiply that times the number of batteries in parallel. Now, MOST IMPORTANT THING TO REMEMBER, divide that number by 2 if you are using 4 wheel drive with 1 battery pack. Otherwise you will burn a small Integrated circuit on your Vescs PCB.

#4: There is not much "Linear  Correspondance" between the Max ilk m UK m Amps specification of the Motors and the amount of amps being dr aw wn or delivered from the battery pack. This next thing I'm going to say is a rough example of what I mean, but is not technically correct. 

" So You can set a limit to how much current your battery pack is allowed to supply. And You can set a limit to how much current your vesc can allow to go to your wheels. Also, there is a Duty Cycle modulation which can be imagined as a square wave with variable time for each pulse thus delivering more or less power per second.

So basically, when you start to accelerate on esk8 board, my very rough understanding is that the battery pack allows current to flow out of the battery pack while the duty cycle is at about 10 percent. Once the Battery Pack Amp limit is reached, then the amperage continues to increase until the Limit set for the Motor Wheels is reached. ( (Or Visa-versa depending on which l I'll kit is reached first.) Only then does the duty cycle start to go up from 10% to a maximum of 95%.

So the point is that that didnt make that much sense in a "Linear" type of conceptual theory. It has to do with 3 phase not drawing power 100% of the time, some power reverberating in the motor coils, etc. 

The point is that almost none really truly can explain in simple terms the way a vesc works. If you figure that out, I'd love to know.

#5: You do not need to oversize your Conduits in your battery pack. Just use several pure nickel strips between each battery at first and you'll probably be fine. 

Definitely use a spot welder. If you have access to 220VAC, buy one of the 220VAC Source Power Spot welders. It will be a lot stronger. It will probably cost a few hundred bucks, but it's the only good way to do it. 

Weight is important, fewer batteries mean lower weight. Less overkill on the connections between batteries can mean less weight. A overly heavy board is kind of lame.my board is way heavy because I overkolled my battery pack with lead and copper on top of the nickel strip. By the way, JB Weld can come in handy on the battery pack. 

Also, the best way I've found to solder us with a phosphoric acid flux. And 50%lead/50%tin solid core solder. Rosin Core is garbage. Just get a bottle of Rust Remover Gel from your local hardware store. Make sure it has phosphoric acid as an ingredient. This shit works miracles. After words, sprinkle some baking soda on your soldered jo I'll nta and rinse off with water then dry.

Other than that, you can use "butt connectors" to connect your parts together to test them the first time around. Tou dont need to make every wire connection bullet proof like old iron sides. If you use a butt connector and some electric tape, worst thing that can happen is a practically insignificant increase in resistance.

And btw, you dont need to connect the sensor ribbon cables for you electric skateboard to work. It just wont be quite as smooth from 0 to like 3 miles per hour. But it will still work. 

You could set it up without the sensor wires the first time around or if your in a rush to get something working at the end of the semester etc. 


Other than that, Have a Good Time; )
```

---
## \#10 Posted by: sammyg Posted at: 2019-11-14T02:17:01.863Z Reads: 16

```
As of today, I got the board running (with only 2 motors as I am working with a 10s2p battery I had) and programmed the VESC's.  The FOC motor wizard popped out 30A for the motors and I had very unimpressive results at the 22A motor setting I had configured.  I confirmed with the nice sales rep of Maytech on Alibaba that 30A is correct.  It is a ripper compared to the cheapo single hub motor prebuilt board I bought off FB market place.

Do know, I have the battery max amps at 15A per VESC.  I also ordered a 10S5P made of 30Q cells so that should be here in 2 weeks maybe and I can get the other 2 motors on the board.

Thank you for all the pointers!  

Here are some images of what I did last night (a lot of xt60 connectors and an anti spark key)
 ![IMG_1745|375x500](upload://yWiyw7QymRm8ZMaDOCZPbg1y77H.jpeg)

today with the electrical taped components (I know it is sketchy!) 
![IMG_1761|375x500](upload://wLYrcH5nPqvgTtSntreta0FUpB8.jpeg)

as well as the initial sketch for this all wheel drive micro-kart idea
![IMG_1760|375x500](upload://uoJyM434tWxwkX1Q3tJnFdQBcUk.jpeg)
```

---
