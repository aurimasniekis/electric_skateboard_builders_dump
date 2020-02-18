# Mountainboards need motor sensors. Yea? Nah?

### Replies: 16 Views: 965

## \#1 Posted by: michaelcpg Posted at: 2018-01-14T20:23:20.649Z Reads: 187

```
I'm looking to do my first Trampa mountainboard build with one of @Nowind's E-Toxx DirectDrive gear kits. Will likely be 10S dual 6374. 

While I've previously built street boards with and without sensors (current board has sensors but I'm not using them), I'm interested to see how common sensored motors are on mountainboards, particularly seeing as your feet are strapped in, so you can't really do kick starts. 
My main concern with sensors though is that they're often not waterproof... 

Keeping in mind that I'll also be using FOC, do you guys think sensors are necessary?

Edit: If anyone has any recommendations for sensored 6374 motors that're waterproof that'd be much appreciated :)
```

---
## \#2 Posted by: Acido Posted at: 2018-01-14T20:24:02.090Z Reads: 178

```
Sensors are cool, yeah.
```

---
## \#3 Posted by: MrHappy Posted at: 2018-01-14T20:24:22.347Z Reads: 180

```
You could just rock forward a bit to make it easier on the motor, You dont really need them but it definetly makes the startup smoother.
```

---
## \#4 Posted by: Der6FingerJo Posted at: 2018-01-14T20:59:04.793Z Reads: 170

```
I would always choose sensored over non sensored, it's really essential sometimes when you're caught in the dirt. I'm using Overion 130kv motors, they are sensored, encapsuled and have a 8mm shaft.
```

---
## \#5 Posted by: Cobber Posted at: 2018-01-14T23:00:21.156Z Reads: 154

```
you just need to get this kit (hit the link it takes you to the relevant post with pictures) from @Nowind, then you can use any motor!

Jensobro for the eMTB win :checkered_flag:

 http://www.electric-skateboard.builders/t/e-toxx-directdrive-vs-trampa-vesc6-vs-leopard-8072-170kv-vs-nowind/30822/162?u=cobber
```

---
## \#6 Posted by: Nowind Posted at: 2018-01-15T09:56:40.177Z Reads: 130

```
Nice Dude, i owe you a beer (-;

Used 3 years unsensored setups... never missed anything
started last year with encoder sensor setup and really love it offroad
but also running MAX6 unsensored on a light freestyle eMTB

Cheers
Jenso
```

---
## \#7 Posted by: TarzanHBK Posted at: 2018-01-15T10:15:21.588Z Reads: 123

```
Since you should start everytime either with a burnout or a wheelie, you won´t experience any difference startup wise  ;)

Sensors are always nice to have, but not necessary. They also add, like you mentioned, a part which can get broken pretty quick from humidity or other stuff you´ll find in the woods.

Can´t tell you something about FOC without or with sensors running on an eMTB
```

---
## \#8 Posted by: DanSkates Posted at: 2018-01-15T11:55:53.886Z Reads: 115

```
Hey @michaelcpg I'm still in the process of getting my settings right and am on a bit of a break with a fractured pelvis (that's another story!) but I'm using dual FOCBOX and SK3 6374 motors on @Nowind's awesome Direct Drive setup and the start up without sensors in BLDC was awful - I had to jump in or rock every start.  That said the performance was amazing.  Interstingly when I switched to FOC sensorless, the start up was totally smooth with no cogging!!!  Amazing!  However for some reasons it runs much hotter and I get cut outs when I go too hard.  I never had that in BLDC.

I'm currently waiting for @Kug3lis's [dual CNC alu case](http://www.electric-skateboard.builders/t/dual-vesc-cnc-machined-aluminium-case/37788) which I'm going to have exposed in the top of my enclosure so the fins catch the air flow.  If this works then I'll have a really grunty, powerful set up and when I'm fixed I'll be ripping it!   Gonna link in some bluetooth modules to to get an insight in to what's happening there.  I'll keep you posted!  :metal:t2:

So I guess in summary you can get away without sensors in FOC and get smooth start up.  I'm running 12s too so 10s would likely run cooler...
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-01-15T12:34:22.627Z Reads: 103

```
hehe, I think it will run way cooler than normal focbox'es. I saw the post there guy just added heatsink via thermal paste to original focbox and got 20 degrees off, so I think it will be able to stand at around 30-40 degrees using fins and good air flow. Sorry that I could not provide better numbers as we do not have any single working focbox (Still waiting for fulfillment from black friday)
```

---
## \#10 Posted by: DanSkates Posted at: 2018-01-15T12:41:34.132Z Reads: 100

```
[quote="Kug3lis, post:9, topic:43724"]
so I think it will be able to stand at around 30-40 degrees using fins and good air flow
[/quote]

My HT-10s have just turned up so I'll be sure to do a before and after keeping the same settings ;-)  be intersting to see how much difference it makes.
```

---
## \#11 Posted by: rich Posted at: 2018-01-15T20:12:15.266Z Reads: 92

```
Sensors and FOC are a must have on mountainboards IMO. I started with BLDC hybrid mode which sucked a lot at least in my case. You can see the difference in startup performance from standstill in the beginning of the video. 

Which HW do you use for FOC?

https://www.youtube.com/watch?v=ptlHqK7kqCA&t=15s
```

---
## \#12 Posted by: michaelcpg Posted at: 2018-01-15T20:24:46.355Z Reads: 89

```
Cheers for all the feedback guys. Seems like a good middle ground for now would be to go FOC unsensored and then if need be, upgrade to @Nowind's fancy encoder sensors if he's selling them :stuck_out_tongue:

Anyone used these motors before?
http://alienpowersystem.com/shop/brushless-motors/aps-6374hev-outrunner-brushless-motor-170kv-3300w/ 

@rich I'm still trying to work out what ESC's to use but it'll most likely be a 10S8P 1KWh pack paired with a couple of FOCBoxes now that Ollin Boards aren't really selling separate parts anymore. VESC 6 would be preferable but I can't justify the price that Trampa are asking atm and I haven't really seen many other DirectFET options out there currently.

@Kug3lis are you going to have more of your FOCBox aluminium cases available after preorders? Might be something I'll have to look into :) 

@DanSkates that's rather interesting to hear. From what I've read on these forums and from my own personal experience, FOC usually runs cooler as it's supposed to be more efficient. I'll definitely keep this in mind. Other than that, do you find a couple of FOCBoxes to have enough power to properly drive a mountainboard up hills etc offroad etc?
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-01-15T20:41:46.256Z Reads: 81

```
Yes, there will be some extra for everyone who wants after pre order but not that much ;)
```

---
## \#14 Posted by: Okami Posted at: 2018-01-15T20:59:59.972Z Reads: 77

```
I would be with @rich on this one. In my experience sensors help a lot.. It might be especially important when starting in grass or uphill. though it probably does depend a lot on what motor controller u gonna use in the end and what gearing u will have / also motor kv...
```

---
## \#15 Posted by: michaelcpg Posted at: 2018-01-15T21:11:41.864Z Reads: 77

```
Yea it's a bit of a tough one. 

My biggest concern with using standard integrated hall sensors is that they're generally not waterproof and one of my aims with this build is to make it so that I can basically hose down the board without having to worry about getting anything wet.
```

---
## \#16 Posted by: DanSkates Posted at: 2018-01-16T02:42:06.495Z Reads: 64

```
[quote="michaelcpg, post:12, topic:43724"]
FOC usually runs cooler as it’s supposed to be more efficient.
[/quote]

Yeah I gotta say I heard the same.  I need to investigate further and I'm hoping the BT modules will give me a better indication of what's happening.  I'm running my motor max / battery max both at 80A with the absolute max set to 155A so perhaps it's cutting out not because it's hot but because I'm breaching my max setting?  Again, I need to experiement more.  Defo take the advice of the gurus here as I'm still only just embarking on this adventure and may actually upgrade my motors to sensored in the future because moving to FOC made a massive imporvement to start up and looking at @rich's video It's clear that FOC is the way to go!
```

---
