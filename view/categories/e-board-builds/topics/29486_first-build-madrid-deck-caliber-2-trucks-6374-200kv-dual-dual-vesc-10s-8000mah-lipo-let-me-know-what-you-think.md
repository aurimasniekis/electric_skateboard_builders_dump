# First Build. Madrid Deck. Caliber 2 Trucks. 6374 200kv Dual , Dual Vesc , 10S 8000mah Lipo ///Let me know what you think

### Replies: 14 Views: 1150

## \#1 Posted by: HifuSk8 Posted at: 2017-08-02T20:55:08.617Z Reads: 206

```
Hi there Forum. 

Let me begin with saying thank you for all your free advises. 
I have been digging these Pages and i think i have finally found what i'm going to build.

What I have/What I have ordered so far:

Deck : Madrid Slight Concave<img src="/uploads/db1493/original/3X/e/f/efa9c7dafb621eb17801282ababaaa9b05fecf6b.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/a/3/a30be4b47d1de94068c82186dae91c3f1a1ce214.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/d/3/d3d4e463a74acf3b8b005d94081895a252e19976.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/1/6/169ea719cf869ef0bf7f37415613b61afe9e1853.jpg" width="666" height="500">
Vesc : 2X Original ESK8 controller 4.12 by esk8.de (they're from germany, wich is kinda close and they do sell theyr own vesc, so i thought lets give it a try)
Motors: 2X 6374 3300W 200kv sensored , also by esk8.de
Controller: Micro Remote by esk8.de
Trucks : Black Caliber 2 50°
Wheels : Black 83mm stickies 78a
Mount: Dual Mount Kit by esk8.de
Gearing : 12/36
Batteries : 10S (2X 5S1P 8000mah 30C Zippy Flightmax) with 5.5mm bullet connectors.

What I am not quite shure about:

I want to build my own enclosure, probably 3dprint something since i have acces to one. not sure about that
I should probably put in a nice switch but i havent found one so far and i will probably just build a U-Key for the start.
I would like to put together my own Remote wich is able to read some data back off the vesc, i have been following some people out here who dare to do so and I really hope to find a design wich suits me and wich I can actually put together myself. but until I have found such thing I will go with the Remote i have bought with the other stuff from the German Seller. 

So far so good. I will start posting pictures and build logs as soon as enough stuff arrives. If you see anything I am totally doing wrong or also if you have questions, suggestions, feel free to hit me up .
```

---
## \#2 Posted by: Guacamoleface Posted at: 2017-08-02T21:02:04.574Z Reads: 183

```
[quote="HifuSk8, post:1, topic:29486"]
Motors: 2X 6374 3300W 200kv sensored , also by esk8.de
[/quote]

Are you gonna buy extended calibers or diagonal mount them? 2x 6374 wont fit next to eachother on standard calibers, they are too big.

Edit: The Micro controller unless its the V2 is something I would advice against, Hade one mysefl, Lots of issues with connections on them. not sure if thats fixed in V2. the Mini remote is really reliable however.

Also make sure you check measurements on the batteries. So they are not to clunky / big. Will make it harder with enclosure and height. Especially if your board has flex.
```

---
## \#3 Posted by: joellind Posted at: 2017-08-02T22:26:17.903Z Reads: 154

```
Have you ordered everything from esk8.de? I placed order there last week and have had some troubles. Would like to come in contact with someone else with knowledge of buying from them.
```

---
## \#4 Posted by: Guacamoleface Posted at: 2017-08-02T22:30:57.339Z Reads: 149

```
Me and my friend ordered from there more than once, they were quick with sending both times. Good quality aswell.  What is the troubles?

Edit: PM so we dont hijack the tread to much :)
```

---
## \#5 Posted by: thisguyhere Posted at: 2017-08-02T22:34:12.011Z Reads: 146

```
to fit dual 6374 it'll have to be mounted criss-cross or diagonal.
```

---
## \#6 Posted by: HifuSk8 Posted at: 2017-08-11T20:05:22.487Z Reads: 143

```
**Update!**

@Guacamoleface
@joellind
@thisguyhere 

 About the Big Motors I figured that I have three Options, wich I will be pursuing in the following Order:

1. I Mount them "ZigZag" , wich as far as I understand means mounting both motors on the same Truck, one under the Board and one facing out the Back, right?
I dont have the Parts yet so I dont know about clearance under the Deck but if that doesnt seem to be to big of a Problem I will probably go with this Way of mounting my Motors.

2. I Mount them diagonally on both Trucks facing both out the Front and Back of my Board.
That would eliminate any Clearance Problems I could potentionally face (with the Motors/Mounts) but first of all it would get me into Trouble with keeping all my Wiring nice and short since I would have to run the Power Wires from the Loopkey all across the Board so I can connect the ESC at both Ends of the Board.

And it would make it more complicated with the Enclosures on the Bottom since I would either need one big long one to house the Batteries in the Middle and both ESCs at the Ends, or I would have to make separate Enclosures for the Batteries and then the two ESCs individually

All in all I dont like the Idea and the Looks of this Option.

3. I would have to get wider Trucks to be able to mount them paralel at the Back, facing out. But as far as my quick Research went, it is not to easy to get them where I live.(Switzerland) Maybe I'm just Dumb and dont see the obvious Offers around...

About the Size of the Batteries : They're 40mm's laying down flat and I will add a Picture where I show them laying on my Deck, even though right now it has standart Paris Trucks and 73mm Wheels, so the clearance is going to increase even further with the Bigger Wheels and different Trucks. 

I hope the Micro controller works well enough to get me started and if it does not, this will probably just make me work faster and harder on my DIY Remote.

A Week passed since my Order from esk8.de so I hit them up to know how they were doing with my Stuff.
Attila replied within hours, very nicely explained theyr situation and the current State of the Order and asked me about some details of the Shipping.

So far I am very happy with the Job they seem to be doing. 

The Batteries , some spare Stuff like Shrinktubes and Bulletconnectors, a new Dual Channel Charger http://www.isdt.co/d2.html arrived a couple days ago and I have to say I am ******* impressed with international shipping nowadays. The Batteries came from HK and the Rest from the Netherlands and it was all shipped in under 5 days after being handed over to the shipping-services... =) very nice

The Voltages of the different Cells were very even (within 0.01V) and came in with a Voltage of about 3.75V , so i balance-Charged them to 3.8V per Cell, so I can leave them until I'm gonna use them. (and just because I wanted to try out the Charger , as far as I'm concerned 3.75 ist a good storage Voltage too)

Down below I will add some pictures , mainly the Batteries , some charging Adapters I made and the Charger.

So far so good. 

Enjoy the Weekend

<img src="/uploads/db1493/original/3X/2/7/27f9aa7e2864aaa1ae39172c6ed921f5ef0a420a.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/2/a2c2a081ee69883d45adc226d36d6d9a6018847f.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/f/e/fe2f4a2226c294b2672f7fa184c533c0690c9c38.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/6/9/695998ec9c48555d32ade8227d2c5390828c5ad6.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/1/7/177742f9aaf798efba2ebd221a062343d71656fb.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/f/4f8291ccba65dfb424d7e7cde995ecef6a488289.jpg" width="374" height="499">
```

---
## \#7 Posted by: Guacamoleface Posted at: 2017-08-11T20:16:01.063Z Reads: 126

```
For longer trucks, I think DIYelectricskateboard is the best way to go.(overseas and expensive shipping however)

About zig-zag mounting on same truck, one front facing and one back - Make sure the motor mounts are compatible with mounting backwards, As the truck require a tad longer motor mounts( atleast on caliber trucks) for facing backwards. My standard DIYelectric motor mount wont mount backwards due to being to short.

as for diagonal I read earlier that it was better keeping longer motor cables and shorter battery cables for the vesc. Worth checking that if you are taking that route. or ask someone like @chaka or anyone else familiar with diagonal mounting. 

Also the micro should get you going, Just be careful of the cutoffs it may get.

My enclosures are around 40-45 mm I think and I got some flex. I have small risers but clearance isnt a problem for me atleast :)
```

---
## \#8 Posted by: thisguyhere Posted at: 2017-08-11T21:01:59.011Z Reads: 106

```
Keep it simple and go with a monodrive to start. A single 6374 is surprisingly fast, and it'll keep cost and complexity down.
```

---
## \#9 Posted by: HifuSk8 Posted at: 2017-08-11T21:18:02.578Z Reads: 103

```
I appreciate your Suggestion since i know you try to help a first time Builder Out :) 
...but I am certified Electrician and I currently work as a Sound Engineer at a Concert-Venue where I do Lots of Maintenance (Soldering, Electronics-troubleshooting) and I have built some Race-drones so I don't consider myself a Beginner that much ;)

And I am aware that my Plan ist going to be quite overbuild , but there is no Build like overbuild.
```

---
## \#10 Posted by: Guacamoleface Posted at: 2017-08-11T21:23:54.598Z Reads: 106

```
as @thisguyhere say - unless you felt the power or is experienced on a board or live in a very hilly area where you gonna need power to climb hills, then a single motor setup would be better to start off with. You still have the parts you can use for a dual as you want after you get to feel it more.
 
Im currently running a single 6374, and Im really confident on a longboard or any skateboard. The power is sweet. I do not have any steep hills or so that I need to climb so cant speak on that. 

it still has enough power to scare me, think Im pretty much blind for the speed I keep on that thing atm. :joy: 

But yeah I feel you - was looking into dual 6374 just because why not.. but when I think of the weight it adds and so on I kinda decide not too. Parts I want to improve in my opinion is keeping the weight lower, and making it more manageable whenever u cant ride.
```

---
## \#11 Posted by: HifuSk8 Posted at: 2017-08-11T22:00:27.881Z Reads: 112

```
My Goal ist to eat Hills Like the following with ease.
 `<img src="/uploads/db1493/original/3X/0/3/034952e990feff0871c56f006ff98b1b84c6d9b9.png" width="281" height="500"><img src="/uploads/db1493/original/3X/0/a/0afd04d2f906fe6ba1d433655546d092530cd6ba.png" width="281" height="500">
And to be able to push my Girlfriend uphill on her Bike without anything getting warm.

So I was thinking about overbuilding the Hardware-Side of Things and then use the Settings in my VESC to Run everything a Lot under Specs so I have Lots and Lots of Power to do everything as stated  above and still be running the Hardware so Low ampwise that its gonna stay cool and last long.

But maybe I'm underestimating 3.3kw of brushless Power and I am now thinking about going single 6374 first and then ramp up the Number of Motors if the VESC or Motor get warm whilst pushing myself (about 80kg with Protection-Gear and Bag) and my Girl and her Bike (maybe 70kg maybe 80kg I'm guessing and trying not to be rude :P ) uphill 17-20° ... 

I have a FLIR-camera in my Cellphone and am going to find out. :)
```

---
## \#12 Posted by: Guacamoleface Posted at: 2017-08-11T22:11:26.186Z Reads: 108

```
So far I've tried one hill, it was pretty insane and I couldnt get up there but got limited by traction, which is less of a problem on dual.

However starting with  single drive and upgrading if not enough sounds like a good idea economically atleast ;)
```

---
## \#13 Posted by: NickTheDude Posted at: 2017-08-11T22:36:18.577Z Reads: 105

```
If I were you I'd set it up single motor for now then order some 218mm trucks to go dual with later. diy-electric-skateboard-kits-parts/torqueboards-218mm-trucks/
```

---
## \#14 Posted by: HifuSk8 Posted at: 2017-08-16T20:08:01.584Z Reads: 96

```
So Attila from esk8.de contacted me today and told me that with their specific Trucks my Setup (going Criss-Cross) wasn't going to fit, since they machine their Trucks so the Motor-Holder only matches one way around. And also going diagonal over both Trucks wasn't going to work because only one of the Trucks in their Kit is premachined.

He was very kind to me and explained that he didn't want to ship mismatching Gear and offered me to ship two sensored 6354 2200W Motors instead and pack an Vedder Antispark and some extra replacement Belts on Top to make up for the price Difference.

I agreed to do it the proposed Way because first of all it gives me a better Option over the Loopkey and probably it is going to make the Build a lot easier overall because I can just mount the Motors normally on the rear Truck.
```

---
