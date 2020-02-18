# Bad Speed wobbles at 40km/h+

### Replies: 23 Views: 366

## \#1 Posted by: MaxMalouf Posted at: 2019-01-06T02:20:36.216Z Reads: 151

```
Hey guys, recently upgraded to a dual 6374 motor setup and wanted some help as when I get toward the end of my throttle, it feels like one motor spins faster than the other even though the Kv 170 for both. When this happens I get deadly speed wobbles!

should I set a max erpm and see if that helps?

just need to see if anyone has expirenced this, I want to fix this before i end up in a wheelchair
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-01-06T02:21:36.994Z Reads: 151

```
running canbus or split ppm? Try checking your logs after a ride
```

---
## \#3 Posted by: MaxMalouf Posted at: 2019-01-06T02:25:08.499Z Reads: 149

```
canbus, should i run canbus and split ppm at the same time?

also @mynamesmatt do i just look for faults? wdym by logs?
```

---
## \#4 Posted by: DeathCookies Posted at: 2019-01-06T02:33:36.850Z Reads: 142

```
[quote="MaxMalouf, post:3, topic:80060"]
canbus, should i run canbus and split ppm at the same time?
[/quote]
No. It is recommended to use canbus for additional features like traction control (which prevents the wheels to spin faster than the other)
```

---
## \#5 Posted by: DeathCookies Posted at: 2019-01-06T02:35:09.768Z Reads: 137

```
You could check both motors kv. connect the pc to one vesc and enter in the terminal command "kv". connect to the other vesc and repeat the step to compare the value
```

---
## \#6 Posted by: mmaner Posted at: 2019-01-06T02:45:32.626Z Reads: 133

```
It's unlikely that 1 motor is spinning faster than the other, possible but unlikely. I would look at your bushing srtuo first.  Go look the Riptide/@Alphamail, he has dozens of recommended setups.
```

---
## \#7 Posted by: MaxMalouf Posted at: 2019-01-06T02:47:19.407Z Reads: 128

```
great idea
ill give it a go
```

---
## \#8 Posted by: MaxMalouf Posted at: 2019-01-06T02:48:06.685Z Reads: 125

```
yeah my trucks are getting old ill get new bushings etc.
```

---
## \#9 Posted by: mmaner Posted at: 2019-01-06T02:49:34.084Z Reads: 121

```
What trucks are you using, how much so you weigh and how wide is your stance at speed?

Also, if you trun your front foot almost straight and angle your back foot in you can reduce wobbles.
```

---
## \#10 Posted by: MaxMalouf Posted at: 2019-01-06T02:55:05.892Z Reads: 115

```
ive been riding evolve for years, the board that im having the issue on is a pimped evolve gen 2 so i have kept the evolve trucks and everything, just running dual 6374 and focbox with 10s4p vtc6 (120a) its a beast.

Its not to do with my stance i dont think i was riding 45kmph comfortably with single drive so its weird
```

---
## \#11 Posted by: Friskies Posted at: 2019-01-06T03:01:58.763Z Reads: 113

```
[quote="MaxMalouf, post:10, topic:80060"]
i have kept the evolve trucks and everything
[/quote]

Pretty sure the problem is here.
```

---
## \#12 Posted by: dareno Posted at: 2019-01-06T03:09:21.408Z Reads: 106

```
Without a doubt this  :point_up_2:
Upgrade your bushings and pivot cups to a harder duro and see.  Riptides are your best bet but evolve do sell a full set of differing duro bushings too.
```

---
## \#13 Posted by: MaxMalouf Posted at: 2019-01-06T03:14:50.537Z Reads: 107

```
 hopefully the issue is as simple as that. ill get right to upgrading those
```

---
## \#14 Posted by: dareno Posted at: 2019-01-06T03:18:01.115Z Reads: 105

```
You will not believe how much a proper set up will help with speed issues.  It certainly is not the motors spinning up differently.  When you accelerate on an esk8 the trucks walk if the bushings are bad.
```

---
## \#15 Posted by: mmaner Posted at: 2019-01-06T03:18:17.480Z Reads: 106

```
Ok, 2 things. 

1.  Evolve trucks are much more prone to in ones because if the double kingpin. 

2.  Wobbles are caused by vibrations from outside forces (outside of the truck).  The addition of another motor is creating a combination of vibrations that start the wobbles at a certain speed.

A bushing upgrade will keep the vibrations isolated to a degree, but this trucks will always be prone to wibbles.
```

---
## \#16 Posted by: dareno Posted at: 2019-01-06T03:20:38.342Z Reads: 96

```
Personally speaking I would not ride dkp's over 45ks period.  Scary stuff. :grimacing:  just not sure those old gen 2's are dkp.
```

---
## \#17 Posted by: mmaner Posted at: 2019-01-06T03:22:16.784Z Reads: 96

```
I feel ya. I like the carve of DKPs but not the lack of stability at speed. SR TKPs are at least as carvy and much more stable at speed. The bushing seat replaces the 2nd kingpin, does a much better job.
```

---
## \#18 Posted by: MaxMalouf Posted at: 2019-01-06T03:27:36.477Z Reads: 97

```
@dareno @mmaner yeah okay definatly will try, just was a little confused before because the dual kingpins have always been fine at high speeds for me.
```

---
## \#19 Posted by: psychotiller Posted at: 2019-01-06T03:36:17.508Z Reads: 87

```
Lose the double kingpin trucks. They aren't as good or stable as you think they are.
```

---
## \#20 Posted by: yelnats8j Posted at: 2019-01-06T03:38:32.460Z Reads: 87

```
You better do as @psychotiller said or he might personally come over there and get rid of them for ya.

Also he is right about the Kingpins get rid of them and get some Surfrodz or even Calibers.
```

---
## \#21 Posted by: Lunasi Posted at: 2019-01-06T03:39:16.877Z Reads: 81

```
 Personally I think you should speak to @Alphamail to get a better bushing and setup recommendation
```

---
## \#22 Posted by: dareno Posted at: 2019-01-06T03:52:57.330Z Reads: 78

```
[quote="psychotiller, post:19, topic:80060"]
Lose the double kingpin trucks.
[/quote]

You've been told now.  :sunglasses:
```

---
## \#23 Posted by: Boxer86 Posted at: 2019-01-06T08:56:50.634Z Reads: 62

```
I run have run calibers and evolve supercarver trucks on a twin setup and the calibers gave me zero speed wobbles at 60km plus with riptide bushings. I then changed to the supercarver for more turnability and have tried a number of riptide bushings to get the best setup for carving and stability. The best I have found is riptide Krank chubby 92 red bushings matched with the 96 evolve hard cone bush on the back truck and on the front I have krank 93 barrels with evolve medium cone bushings. Then you simply tighten to increase stability and loosen to give you turning. That being said with this setup you can do 60km with the trucks tight and weight on the front truck but you will have limited turning. I run them a bit looser and can do 50km without a hassle and have good carvabilty.
```

---
