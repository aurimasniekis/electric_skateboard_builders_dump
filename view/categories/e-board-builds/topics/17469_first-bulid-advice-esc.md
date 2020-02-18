# First Bulid. Advice - ESC

### Replies: 28 Views: 1709

## \#1 Posted by: Migro Posted at: 2017-02-09T21:55:00.618Z Reads: 164

```
Hi
So i've been looking into making an eletric longboard for a long time know, and after months of research on and off. I have come to ask you for some advice. 

My main question is if anyone knows anything about HobbyKing Red Brick 100A ESC 5VBEC V2

My plan so far is:
Turnigy Aerodrive SK3 - 6374-192kv Brushless Outrunner Motor
15:30 ratio(Maybe later upgrade to 20:30 if i want to go faster)
4x ZIPPY Flightmax 5000mAh 3S1P 25C(2 and 2 in series and maybe those 2 in parralle if possible so that i dont need to swtich between batteries for the long range)
The wheels on my board is 70mm.

I've made the controller allready with at wiinunchuck, but not sure how to test if it works because i dont own a oscilloscope.

EDIT:
After further reading i wondered if anyone got some advice if i should choose my planned 192kv motor or an 245kv?

The rest i should be able to do myself. (Hopefully)
Any advice is welcome.
```

---
## \#2 Posted by: lowGuido Posted at: 2017-02-09T23:31:52.846Z Reads: 147

```
Dont use the red brick. Its really bad. If you want to get a hobby king esc get the xcar beast 150A it works way better.
```

---
## \#3 Posted by: Migro Posted at: 2017-02-10T07:17:53.461Z Reads: 133

```
Okay thanks.
Im going to look into that one. but the price is more than double and kinda ruining my budget.
```

---
## \#4 Posted by: saul Posted at: 2017-02-10T08:33:34.442Z Reads: 132

```
Esc is probably the most important component. not where you want to try to save a few $.

vesc all the way. then you have the option to wire to 12s for real performance! :sunglasses:

also those are ratios are not realistic. on 15/30 you'll be ok on smaller wheels but 20/30 no way. and mounting to 70mm wheels is another headache on its own....
```

---
## \#5 Posted by: Migro Posted at: 2017-02-10T08:53:46.668Z Reads: 120

```
Hmmm.
The vesc seems pretty expensive. Especially where im from. 

With the calculator i've used im getting a decent speed with the 15:30 ratio and 245kv motor.

As far as i understand the more cells i only going to give me more speed right? But i think 22mph/30ish kmh seems fast. So i'm more into the long range.
Haven't looked so much into the mounting. I think that's some trial and error.
```

---
## \#6 Posted by: nmagz3 Posted at: 2017-02-10T09:00:56.820Z Reads: 118

```
Hey there!  And welcome to the community!  I'd second the VESC but that's just me.  A friend of mine is running on an ESC and has a program box.  It looks like there is a ceiling with the ESC.  And that really is where the VESC shines!  The possibilities are endless when it comes to customization and tuning.  Good luck with the rest of your build, and post before and after pics :slight_smile:
```

---
## \#7 Posted by: Migro Posted at: 2017-02-10T09:21:00.971Z Reads: 117

```
Thanks :slight_smile: 
I think the only thing to do is more research as the vesc is an expensive option.
```

---
## \#8 Posted by: ACIN Posted at: 2017-02-10T09:41:31.710Z Reads: 115

```
Hi, where about are you from? 
More voltage=more speed but also more range, since what translates into range is Watthours (Voltage*Amphours), I have a 12S (3,7V*12=44.4V) 5500 mAh (5.5 Ah) Battery so I have 5.5Ah*44.4V=244.2  Watthours worth of Energy (theoretically) stored in my charged Batteries.
The rule of thumb here is 10 Wh give you rougly 1km of range, depending on heat efficiency, weight, friction, terrain, the way you ride, aerodynamics and a lot more... So I get about a 24 km range.

About the VESC, you will have the advantage of a huge amount of possibilities of customization, like how much your board accelerates at which trigger position (and I hear it is a lot smoother than cheap ESC's), you will be able to implement LED lighting or a phone charger if you want to, furthermore you can make your motor run as silent as a grave and also your battery will give you more range if you use a VESC since it recharges the battery as you break.

There is a reason why this thing is so expensive...


If you are aiming for range focus on increasing your Battery Capacity or S count, and consider saving a bit more for a VESC. But as said the right ESC from hobbyking will move you too!
I will try to find a cheap VESC seller near you (I got mine for about 85€ on a group buy).
```

---
## \#9 Posted by: Migro Posted at: 2017-02-10T10:10:21.247Z Reads: 110

```
Im from Denmark.
Thanks for the detailing info. Much appreciated. 

I get the part from the vesc where it is possible to charge while braking. But other things as the "slow" acceleration could be done in some programming to the controller. (selfmade).

More research into batteries for me i guess. 

Your help is much appreciated. :slight_smile:
```

---
## \#10 Posted by: saul Posted at: 2017-02-10T10:22:31.154Z Reads: 98

```
the vesc is a bit more expensive compared to car escs, but its at least 10x better. worth it. :sunglasses:
sure you can smooth a cheap esc a bit the the controller but that work would still go further on the vesc....

as for batteries, lipo is the cheapest for me, but now you can get a premade 10s3p or 4p pack with a bms and charger, it makes everything much nicer to actually use...

there are more then a few sellers in the eu and uk,
Whats your budget, speed, range requirements?
```

---
## \#11 Posted by: Migro Posted at: 2017-02-10T10:30:42.820Z Reads: 96

```
My budget is around 290$ and i already have the board and controller. As far as range and speed. range is probably number one priority. As i think theres a law for eletric bikes to a max of 25kmt so longboard is the same i think. So probably around the 30kmt mark maybe a little more.
```

---
## \#12 Posted by: ACIN Posted at: 2017-02-10T10:58:16.430Z Reads: 95

```
Should you go for a VESC you can get it for 95 GBP on proto-boards.com (great site, ordered before and it was delivered really fast/cheaply) or for 89 GBP on alienpowersystem.com (not sure about shpping here)...
Esk8.de is a lot more expensive unfortunately.

Then there are also almost always group buys happening where you can get VESC's for down to 80$ if you are a bit more patient, just search Europe GB on this forum or contact @ajaynagra.
```

---
## \#13 Posted by: Migro Posted at: 2017-02-10T12:09:23.198Z Reads: 95

```
Okay thanks. I'll look into that.

But if theres anyone who could recommend and ESC for more options that would be great
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-02-10T12:55:15.468Z Reads: 97

```
my opinion:

6s ESC to keep it cheap: 
x-car beast 120 or 150A
FVT 120A
You can´t really go cheaper.

Better option, if you spend more:
VESC

Other ESCs are most likely not usable or way to expensive.
```

---
## \#15 Posted by: Okami Posted at: 2017-02-10T13:45:55.637Z Reads: 90

```
I'd also suggest FVT 120.. 6s (around ~50usd, if from china) + 8usd pc usb link for programming

Later on, if you got more money.. u can go into vesc thing..

I believe for 6s you might as well would like to get 245kv.. but im not totally sure

Perhaps, ask @lox897 his opinion about kv's as I havent built a e-longboard so im not sure will you get away with that 15/30 or 20/30 ratio for 245kv..

--

Check your countries tax policy for imported goods.. you might be cautious about ordering from website outside EU, if your country puts customs tax for items over 20Eur or so..
```

---
## \#16 Posted by: Migro Posted at: 2017-02-10T14:54:49.380Z Reads: 85

```
Wow this forum is amazing one again thank you. 
Unfortunately my country it pretty strict with imported goods. Aslong as it is inside the EU every thing is fine. 

It's possible for me to find the fvt 120a but if i import from china and then im toging to pay alot. 
Some of the other people suggested the x-car beast 120A or 150A, and those i can import without problem. 
So 120A or 150A?


Sad part is im going on vacation later today, so this projekt is set on standby. Advice still welcome, but i dont know on the internet situation down there.
```

---
## \#17 Posted by: psychotiller Posted at: 2017-02-10T15:37:12.357Z Reads: 79

```
Hi @Migro

If your budget is truly $290, I would suggest just buying one of the mulitple cheap amazon or ebay boards. Not to discourage you from a build. That's definitely the way to go, but at $290 you aren't going to be able to make a good/safe/fun board. 

You need a good ESC with failsafe features that will enable you to accelerate and stop without issue.
```

---
## \#18 Posted by: ACIN Posted at: 2017-02-10T17:51:18.584Z Reads: 67

```
I second that, it will be nearly impossible to build anything satisfying for less than around 400$, maybe 350$ if you already have the board and remote. Even if you are buying a cheap motor and cheap batteries, the greatest quality bottleneck of the board is the brain.
```

---
## \#19 Posted by: pennyboard Posted at: 2017-02-10T18:09:42.732Z Reads: 73

```
I tried to make my first board for under $300. Basically ended up using low quality parts and having to replace them after a few weeks, costing me more money than if I just did it right the first time. My advice is save yourself the trouble and spend the money to do it right the first time. 
Also, I'd recommend wiring those 4 3s batteries all in series to make 12s, as the overall watt hours, which is really what determines range, is the same as 2 and 2 in parallel, and you get higher voltage which means your top speed will be at least 25mph with that gear ratio and motor.
```

---
## \#20 Posted by: Migro Posted at: 2017-02-11T19:07:32.791Z Reads: 61

```
What does the fail safe do? 
And the acceleration is allready programmed into my controller. (Great Scott wiinunchuck).
Mainly i tweaked Great Scotts build to my prefrences. And that one seemed to Work.

As of my understanding i dont see the need for All the best things for this. But what do i know. 

I have just seen alot of cheaper builds. And the speed of 25mph seems really fast?
```

---
## \#21 Posted by: Tuomalar Posted at: 2017-02-12T18:24:32.695Z Reads: 50

```
25mph does not feel very fast in my opinion, mut hurts like hell when your wii nunchuck lose signal and you smash your head to pavement.
```

---
## \#22 Posted by: Okami Posted at: 2017-02-12T18:41:53.050Z Reads: 48

```
failsafe - after remote loses signal - it either keeps the motor's speed, accelerates it to the max.. or gradually powers down the motor..

Usually it is set to lower / cut the power for the motor..
```

---
## \#23 Posted by: Migro Posted at: 2017-02-12T19:25:52.452Z Reads: 48

```
Hmm i think its fast when om between 20-30 kmh downhill om my board. 

Hmm okay i get the fail safe then. Could be pretty important. 

But if i dont have the ekstra Bucks for a vesc what ESC would be recommend. Some recommend the x-car beast series. Any other recommendations?
```

---
## \#24 Posted by: Okami Posted at: 2017-02-12T21:00:53.632Z Reads: 45

```
Check 'banggood motors'' thread, there I showed what programming options FVT 120 Esc has.. 

I can personally recommend it, since I've been using it for a while.. silent operation.. ''tolerates mountainboard''.. Fan might be a bit noisy if you are in a room but while outside wont matter that much..

Brakes are silent.. can be regulated ar 10% steps.. might cut-off / shut-off if you want to brake really hard.. has happened to me..
```

---
## \#25 Posted by: Migro Posted at: 2017-02-12T21:30:30.252Z Reads: 43

```
Okay thanks i'll take a look at that thread. Only problem is import of the fvt because og customs tax. 
But defintely appreciated
```

---
## \#26 Posted by: Okami Posted at: 2017-02-12T21:56:14.445Z Reads: 40

```
If you do look it up.. try to get the version with 3caps and no-sensor port.. there was a user on this forum who got a smoking fvt while riding his eboard.. though he had 2caps version..
```

---
## \#27 Posted by: dylantrygg Posted at: 2017-02-13T01:09:17.830Z Reads: 42

```
Not sure what's in your budget but I got the new VESCX and it's the best part of my board. I can customize it for every ride style I want. You could get it for $160 with a coupon. I run 8s and still get too much torque lol. 

Dylan
```

---
## \#28 Posted by: Migro Posted at: 2017-02-13T16:24:28.731Z Reads: 40

```
Will do okami. And thanks again. Dont Seem that fun with a smoking board.

Hey Dylan i see the adantages with the vesc and vescx. But that price tho..
```

---
