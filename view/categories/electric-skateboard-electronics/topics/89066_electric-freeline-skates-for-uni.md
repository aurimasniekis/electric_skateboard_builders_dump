# Electric freeline skates for uni

### Replies: 12 Views: 646

## \#1 Posted by: tristanhood Posted at: 2019-04-02T07:01:42.437Z Reads: 179

```
Hi all, I need some guidance on my build, any help would be greatly appreciated!

So I pretty much want to build a pair of freeline skates with a hub motor on the back of the rear foot. I do not need a long battery life, I does not need to be fast, I just need a good amount of torque for small hills

7s battery pack with bms using
- Sony VTC4 18650 2100mAh 30A Battery (7 of them) from IMR
- BMS for 7S 25.9V Max continuous current 30A
http://bestechpower.com/259v7spcmbmspcbforli-ionli-polymerbatterypack/PCB-D189.html

70mm 350W Hub motor from aliexpress,
Could anyone suggest a better wheel? I don't mind spending more. (needs to be 70mm hub motor)

Torque esc bldc speed controller
https:///collections/electric-skateboard-starter-collection-performance/products/torque-esc-bldc-electronic-speed-controller

And then just a default controller,
Could anyone suggest charging ports, on off buttons or battery percentages?

Thank you for your time!
```

---
## \#3 Posted by: sk8l8r Posted at: 2019-04-02T07:55:37.526Z Reads: 158

```
[quote="tristanhood, post:1, topic:89066"]
70mm 350W Hub motor from aliexpress
[/quote]

these have about 5mm max of thane
```

---
## \#4 Posted by: Andy87 Posted at: 2019-04-02T08:24:17.981Z Reads: 155

```
[quote="tristanhood, post:1, topic:89066"]
freeline skates
[/quote]

:thinking: i think @Vanarian has some good experience related skates stuff.
```

---
## \#5 Posted by: Vanarian Posted at: 2019-04-02T08:39:52.966Z Reads: 152

```
At work ATM, will come back to OP later :beers:
```

---
## \#6 Posted by: tristanhood Posted at: 2019-04-02T10:05:53.014Z Reads: 141

```
should be ok for the current project, I might look into bigger wheels for future iterations though, thanks for letting me know!
```

---
## \#7 Posted by: sk8l8r Posted at: 2019-04-03T08:43:27.142Z Reads: 112

```
saw this and remember this thread - personally would have gone front wheel drive, rear driven like that scares the back of my head lol

https://youtu.be/8LCenSHFkp4
```

---
## \#8 Posted by: Riako Posted at: 2019-04-03T09:41:16.760Z Reads: 102

```
Nice one ! Plus this should be really torqued!   
did you already saw this before @Vanarian !?? :face_with_monocle: looks very interesting no?

 BTW, very cool project @tristanhood :D I stay here to see more!
```

---
## \#9 Posted by: Vanarian Posted at: 2019-04-03T12:28:11.891Z Reads: 92

```
Agreed, project is super cool 👍🏽

Thanks for the video, yea this guy managed to do something awesome with close to nothing! SLA battery, a DC motor and a ON/OFF trigger and voilà.

@tristanhood since you use freeline skates,where are you goin' to put your enclosure for batteries and all? If you can, a geared setup would be better if you go single drive. If you dual drive that's another story!

You cannot skip the custom frame I think or cut a bit through the standard one (either for motor mount or for the hub).

Maybe you can raise the platform and put electronic there. Or add extra platform around the standard one and put it there, you'll at least not need to raise your footing. Do you have any design already?

Can you put 70mm wheels or similar? Arcboards sells pulley ready wheels.

You should also add open Hook to keep that thing around your feet and still be able to jump out. Maybe two hooks to be able to climb sidewalks?
```

---
## \#10 Posted by: tristanhood Posted at: 2019-04-07T04:12:23.690Z Reads: 59

```
I was thinking of thickening the base that the user stands on to make room for the batteries, esc and bms. I am pretty keen on the hub motor within the back wheel, going to machine the frame on a 5 axis milling machine then store the electrical package within a plastic container. 
Open hook is a smart idea! riding freeline skates is not easy and i think it'd be smart to incorporate a quick release system that has to be intuitive, easiest would probably be open hook.

I was wondering if anyone could just check out the technical package I have in the first post? would the bms work with those batteries, and would that be enough for the hub motor?

I have attached early sketches for the assignment if people are interested :slight_smile:![Concept%202%20Poster|353x499](upload://u9dCJcQUdI2nLDsnQlyWtim8e2b.jpeg)
```

---
## \#11 Posted by: Vanarian Posted at: 2019-04-10T17:37:48.697Z Reads: 46

```
Nice design ! Careful with the truck design but you must have done your homework already 👍🏽

You should replace the Sony VTC4 with Samsung 20S if you want same range but better power, or go 21700 cells and put some 3000mah or 4000mah cells.

If you really wanna go hub, you really should double it cause single tiny hubs are inefficient to max (if you can achieve 30% efficiency on 1WD tiny that's a LOT).

Edit : What about friction drive in the middle ?
```

---
## \#12 Posted by: tristanhood Posted at: 2019-04-12T07:24:46.673Z Reads: 35

```
Thank you for your help! I can't wait to order stuff in to start prototyping.

I will substitute for 18650 samsung cells, I don't need this thing to go really fast, just at max 15-20km/h, i did kind of need torque for small hills though so I will go with two hub motors underneath the rear foot,

Could you recommend a decent bms for 7 samsung 20s batteries?
and could anyone recommend a reliable hub motor other than one of aliexpress? ahaha

What is friction drive?
```

---
## \#13 Posted by: Vanarian Posted at: 2019-04-12T16:01:42.416Z Reads: 25

```
You're welcome :beers: 

IMHO if you bypass discharge and only balance on charge you can use a standard one (I have a tiny 10s BMS for sale haha but maybe you can get an even smaller one if you get a 7 or 8 s and just use the 7s pins),you can also check ebay.

Friction drive refers to using a drive wheel pressed against your actual wheels 

https://www.alizetibikes.com/uploads/1/3/1/0/13107479/1-generalview-modif_1_orig.jpg

It also works if you put a rubber sleeve around the motor can and press fit it between your skate wheels in the middle.

What's the point ? It's super simple and compact and you get a reduction ratio due to motor and wheel diameter, so you gain more torque and can try 1WD, just like a belt drive but more compact (and lighter). This should be way enough for your speed and torque requirements. You can also use any standard skate wheels instead of hubs so better ride quality.
Motor is exposed to air so you can cool it better.

The negative : you stress the motor structure so you really need a sturdy motor (maytech has this new fancy motor with two bearings built in). When the rubber around motor wears out, you get slippage so you need to replace at some point.
```

---
