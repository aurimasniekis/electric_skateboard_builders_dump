# One motor dual drive build

### Replies: 80 Views: 3924

## \#1 Posted by: the1seabass Posted at: 2017-09-28T19:03:49.851Z Reads: 533

```
So for the past couple of months now I have been doing my research trying to figure out the best setup for me. I live in the on a campus with a lot of hills so right off the back wanted to go with a pully system rather than hub motors because of the more tork, however, I still wanted to have both of my back wheels powered. So instead of two vesc, motors, and everything else. I would just have a one vesc, one motor but two pulleys and gear sets on each of the back wheels the motor I was thinking of using is the alien power C8085 sensored Outrunner brushless motor 250KV 6000W ( Here is the link as well  http://alienpowersystem.com/shop/brushless-motors/c8085-sensored-outrunner-brushless-motor-250kv-6000w/) as for the rest of the build I am going to use a Vesc and a 10s2p li-ion battery that I will be making myself to keep the price down. 

As for my board setup, I am running a 36in bamboo deck with caliber2 44 degree trucks and 80mm orangutang wheels with risers. 

Anyway I think my main question is do u guys think this setup will work and if so where do you think I could find two 80mm motor mounts?

thanks for the help in advance.
```

---
## \#2 Posted by: mmaner Posted at: 2017-09-28T19:12:01.815Z Reads: 495

```
How are you gonna bake?  A 10s2p will not give very many amps, therefore sag will be a big deal.
```

---
## \#3 Posted by: bartroosen12 Posted at: 2017-09-28T19:20:26.085Z Reads: 490

```
So you will drive both wheels with 1 motor?
edit: Oh I had not seen that motor before, stupid question
btw you know that this is a huge motor? 80mm diameter, think about the ground clearance, I should go for bigger wheels (90mm-...)
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-09-28T19:33:50.566Z Reads: 485

```
Yeah, 10s2p isn't even half of what that motor wants. You're gonna end up with the equivalent of a solid rear axle, no diff, so you're gonna have some weird turning effects. I think you could get away with a 6374 or 6384 and still have more than enough power if you went with a 10s3p or larger.
```

---
## \#5 Posted by: Cobber Posted at: 2017-09-28T19:35:22.326Z Reads: 464

```
if you special ordered it with a super long motor shaft sticking out both ends it might all line up for you i guess?
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-09-28T20:04:20.795Z Reads: 466

```
what about rotational difference when turning?

if i'm not mistaken carvon did something with one motor driving two wheels but there's slip to account for rotational difference.

at best one of the wheels in your solid axle rear drive will drag, at worst motor shaft will brake.

<img src="https://ksr-ugc.imgix.net/assets/014/797/617/560d786bc8cbb462dd82359d4edc2623_original.jpg?w=680&fit=max&v=1481079808&auto=format&q=92&s=3b9e1fac25e14cd8c308caf9866480a3" />
```

---
## \#7 Posted by: the1seabass Posted at: 2017-09-28T20:36:25.446Z Reads: 436

```
So u think I should just scrap the idea then or at least try to find a small motor? my main concern is just trying to get up there god awful hills around me with out having the board go to a crawl
```

---
## \#8 Posted by: mmaner Posted at: 2017-09-28T20:46:01.332Z Reads: 429

```
You would be better off using a 190kv-200kv 6374 motor with a 10s4p or 5p pack, a 1024p made with Samsung 30Q's should be more than sufficient to give you decent hill climbing ability.
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-09-28T21:14:45.088Z Reads: 421

```
yea i can climb some big ass hills around here with a mono 6374, just use lower gearing (16/36T) with smaller wheels (83 or 90mm) and you should be fine.  back it up with a 10s or 12s, minimum 4p pack. probably wont go full speed up hills but you'll make it up.

only thing is there are very short, intermittent loss in traction, especially on steeper descent.

what you're proposing seems overly complicated with many points of failure.
```

---
## \#10 Posted by: the1seabass Posted at: 2017-09-28T22:30:57.383Z Reads: 393

```
would Samsung INR18650-25R 18650 2500mAh 3.7v Rechargeable Flat Top Batteries work if I did them in 10s4p for the 6374 motor
```

---
## \#11 Posted by: thisguyhere Posted at: 2017-09-28T22:32:07.053Z Reads: 377

```
of course, those are the cells i used on my first build and were the go-to cells before the 30q came around.
```

---
## \#12 Posted by: the1seabass Posted at: 2017-09-28T22:34:39.324Z Reads: 364

```
which would u prefer if you were making your first board again?
```

---
## \#13 Posted by: thisguyhere Posted at: 2017-09-28T22:41:19.205Z Reads: 356

```
30q, apparently less sag and more capacity compared to 25r.
```

---
## \#14 Posted by: Stef Posted at: 2017-09-28T22:50:31.296Z Reads: 351

```
Take note that a VESC is only rated for about 60A and a max voltage of 12S. With one vesc you will get 60*12*3,7=2600 watts of continuous power. With a larger motor you might still get more torque but you wont get any more power out of it...
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-09-28T23:45:41.981Z Reads: 339

```
If you were to use the dual drive idea you would probably need a differential of some sort to be able to turn around in less than 5 miles...
```

---
## \#16 Posted by: pat.speed Posted at: 2017-09-29T00:31:10.374Z Reads: 338

```
Or he could just board slide when he wants to turn😂 You could use some sort of ratcheting system to allow one wheel to turn slower
```

---
## \#17 Posted by: MysticalDork Posted at: 2017-09-29T00:41:50.215Z Reads: 342

```
Yeah, but then he'd only be able to turn left. Maybe that's what they do with Nascar!
```

---
## \#18 Posted by: the1seabass Posted at: 2017-09-29T01:23:20.952Z Reads: 340

```
lol we could always make a longboarding NASCAR team and start racing them
```

---
## \#19 Posted by: the1seabass Posted at: 2017-09-30T00:49:54.893Z Reads: 316

```
could I go above that 2600 watt limit or should i try to stay below it?
```

---
## \#20 Posted by: MysticalDork Posted at: 2017-09-30T00:53:14.110Z Reads: 313

```
Unless you're accelerating up a steep hill at wide open throttle, you probably won't be anywhere near that limit for more than a few seconds. I wouldn't sweat it too much.
```

---
## \#21 Posted by: the1seabass Posted at: 2017-09-30T00:55:57.442Z Reads: 283

```
do u think this motor would work then for a vesc and a 10s2p battery? http://alienpowersystem.com/shop/brushless-motors/alien-6374-outrunner-brushless-motor-170kv-3200w/
```

---
## \#22 Posted by: the1seabass Posted at: 2017-09-30T00:58:52.608Z Reads: 280

```
sorry meant this one http://alienpowersystem.com/shop/brushless-motors/alien-6374-outrunner-brushless-motor-170kv-3200w/
```

---
## \#23 Posted by: MysticalDork Posted at: 2017-09-30T00:59:44.687Z Reads: 285

```
Those are the same and Yes, that will do nicely. The power ratings on these motors are always best taken with a few pinches of salt anyway, there's no standardized testing method that I know of that they use to determine the maximum output; I think a lot of the numbers came out of someone's ass.
```

---
## \#24 Posted by: GrecoMan Posted at: 2017-09-30T01:00:46.289Z Reads: 288

```
If you end up ordering from him, you can ask for a super long shaft and he'll do it for you.  Same with the power and kV
```

---
## \#25 Posted by: the1seabass Posted at: 2017-09-30T01:02:14.547Z Reads: 273

```
really LOL well if that's the case what would u recommend for a good motor that is reliable and can go a decent speed but can also get up some nasty hills
```

---
## \#26 Posted by: GrecoMan Posted at: 2017-09-30T01:04:01.386Z Reads: 269

```
149kv with 12s and 16 to 36 gearing should get you some pretty nice hill climbing ability but also a decent top speed
```

---
## \#27 Posted by: MysticalDork Posted at: 2017-09-30T01:05:15.266Z Reads: 263

```
190kv is about the highest kv that won't break the 60k limit on 10s.  Hill climbing is dependent on gearing. Go to calc.esk8.today and start plugging in numbers, see what you come up with.
```

---
## \#28 Posted by: the1seabass Posted at: 2017-09-30T01:24:48.157Z Reads: 260

```
so I typed in some number and found that with a 10s battery the highest kv that does that is under 60k is a 230kv motor giving me 59570 erpms with all that i'm thinking this motor will work right? http://alienpowersystem.com/shop/brushless-motors/alien-6355-outrunner-brushless-motor-230kv-2400w/
```

---
## \#29 Posted by: MysticalDork Posted at: 2017-09-30T01:32:53.510Z Reads: 255

```
Check your math there, I think you used the nominal cell voltage instead of the full-charge voltage. 230kv * 4.2v * 7 pole pairs * 10s battery is over 67K.
```

---
## \#30 Posted by: the1seabass Posted at: 2017-09-30T01:45:31.027Z Reads: 260

```
full charge voltage? i was going to use samsung inr 18650-25r cell and they said they had a 3.7 volt charge would that be 3.7v* 230kv* 7 pole pairs* 10sbatter which equals 59570 right?
```

---
## \#31 Posted by: BigBoyToys Posted at: 2017-09-30T01:51:50.187Z Reads: 255

```
Has anyone actually made a dual drive single motor? I dont think the steering would be affected that much. Gokarts should have the same problem but they turn great.
```

---
## \#32 Posted by: mmaner Posted at: 2017-09-30T03:59:12.388Z Reads: 243

```
It's the brakes that are the problem.
```

---
## \#33 Posted by: BigBoyToys Posted at: 2017-09-30T04:24:02.126Z Reads: 237

```
Whats the problem with brakes?
```

---
## \#34 Posted by: MysticalDork Posted at: 2017-09-30T05:05:20.792Z Reads: 245

```
No, that's the nominal voltage, or the average. 18650 batteries have a maximum voltage of 4.2v when fully charged and a minimum voltage of between 2.5 and 3v when fully discharged. Generally when calculating speed etc, you should use the 3.7v number because that's what the board will be running at most of the time, but when the batteries are freshly charged, the voltage is 4.2, and you have to use that number for motor selection because that's the highest number the motor will see.
```

---
## \#35 Posted by: mmaner Posted at: 2017-09-30T14:45:58.806Z Reads: 235

```
To have decent turning while accelerating you would need to use one way bearings in the drive Wheels, hence no brakes. It's all been covered here...
http://www.electric-skateboard.builders/t/carvon-x-your-thoughts/14027?u=mmaner
```

---
## \#36 Posted by: BigBoyToys Posted at: 2017-09-30T16:32:38.275Z Reads: 233

```
Ohh I meant using 1 motor without a freewheeling mechanism. People say the board wouldnt turn, but has anyone actually tried it?
```

---
## \#37 Posted by: Cobber Posted at: 2017-09-30T18:35:53.741Z Reads: 244

```
[quote="BigBoyToys, post:31, topic:34203"]
Has anyone actually made a dual drive single motor?
[/quote]

yeah like BBT said?
Jenso has mentioned some guy on a German forum who made a eMTB dual drive single before... he said it worked fine.
Thane wheels tend to slide around when you carve/turn anyhow...
```

---
## \#38 Posted by: mmaner Posted at: 2017-09-30T19:38:27.208Z Reads: 251

```
I honestly couldn't say.  It seems to me that turning would be handicapped, but who knows.
```

---
## \#39 Posted by: Jedi Posted at: 2017-10-03T05:37:18.544Z Reads: 244

```
https://www.youtube.com/watch?v=BjJrPzoXaeI
```

---
## \#40 Posted by: jmasta Posted at: 2017-10-03T06:37:44.318Z Reads: 238

```

This has been discussed before, and I had the idea to use a 0° baseplate in the rear (1 motor powering both rear wheels).  With RKP geometry on a 0° plate, the truck will lean but does not produce any turn.  I understand the need for a differential in cars, but they have an axle length measured in feet;  a skateboard axle is so much shorter that the difference in speed between the inside and outside rear wheels would probably be negligible on a 0° baseplate.  Because once again, it's all lean and no turn.  A 50°/0° setup still turns because the rear tracks the front, much like a racecar

However I was basically called an idiot and told it would never work.  Because "physics". _Like I'm sure high school physics was very challenging for you, but I have a Master's degree in engineering and still think it might work._ Who's knows? Maybe I really am idiot :joy:  My coworker and some people on here sure thought so!

I am still undecided on how well it would work...
```

---
## \#41 Posted by: Cobber Posted at: 2017-10-03T18:46:28.551Z Reads: 224

```
[quote="jmasta, post:40, topic:34203"]
Because "physics"
[/quote]

yeah there is some funky physics involved with skateboard motion and turning, not all of it is intuitive. On most other 4 wheel vehicles the outside wheels generate most grip. On a skateboard you can lift the outside wheels off the ground...
```

---
## \#42 Posted by: stormboard1 Posted at: 2017-10-21T02:09:57.975Z Reads: 211

```
single motor dual drive would have one wheel locked on turning think of a rwd car with a locked differential..one wheel skips n bounces when taking tight turns
```

---
## \#43 Posted by: PXSS Posted at: 2017-10-21T04:27:35.900Z Reads: 206

```
No, it wouldn't. Think about the turning radius wrt the axle length. A car's average turn radius / width is ~3.25 (my fiat can do 2.85, my friends buick park ave can do 3.25, my f150 does 3.69 at worst (according to google)) . That would be equal to less than 3ft turn radius on a board with 10in wide trucks... I dont know about you, but I definitely cannot make a 3ft u turn on a longboard...

A longboard with a fairly short wheelbase of 23.5in, and a 45deg truck angle has a turning radius of 6ft at 10deg of lean.
```

---
## \#44 Posted by: stormboard1 Posted at: 2017-10-21T04:39:39.868Z Reads: 189

```
true but at high speed would it not slide especially in wet?
```

---
## \#45 Posted by: PXSS Posted at: 2017-10-21T04:42:22.749Z Reads: 188

```
as would a regular skateboard and car with differential brakes... given enough speed on a wet road, anything and everything slides lol.
```

---
## \#46 Posted by: stormboard1 Posted at: 2017-10-21T04:58:49.989Z Reads: 175

```
ya those were just the problems that came to mind every time I thought of this good to know theyr not a problem then..was thinking too much from a car perspective lol..dont know why this hasn't been done..
```

---
## \#47 Posted by: PXSS Posted at: 2017-10-21T05:18:23.247Z Reads: 179

```
A kid I know from school did it on his setup. But its a real ghetto setup with lipos and esc just taped to the bottom of his board and within a year, he's had a broken ankle and wrist. I've never ridden his board though
```

---
## \#48 Posted by: stormboard1 Posted at: 2017-10-21T19:35:34.916Z Reads: 173

```
rough ya esc are very on/off power rode a koowheel and it was all go straight away cool but think a vesc would help it
```

---
## \#49 Posted by: Acido Posted at: 2017-10-21T20:49:57.842Z Reads: 180

```
Isnt here any car guy?

It would be like driving a car with a welded diff

Not so nice
```

---
## \#50 Posted by: Jellybean Posted at: 2017-10-21T21:06:42.026Z Reads: 187

```
It would be exactly like driving with a welded diff. When turning the outside wheel will go its normal path but the inside wheel will hop. This is because of extra energy built up on the from it not spinning. Both wheel get the same amount of energy since they are physically connected, but only the outside wheel can put the energy to the ground smoothly. The inside wheel isn't as smooth because it has the same energy to deliver, but is restricted by traction. The inside wheel axle will bend slightly until it can release the energy as a slip or hop. 

In my opinion it won't be noticeable because you'll never turn as sharp as a car with a welded diff, like @PXSS said. The wheels will probably balance themselves out every time you hit a rock or the road is a little rougher. The hopping will probably only feel like you ran over a small rock at the very most, it shouldn't be too noticeable/obvious.
```

---
## \#51 Posted by: PXSS Posted at: 2017-10-21T21:28:19.090Z Reads: 192

```
The regular turn radius of a board is 7ft. 
The car equivalent would be a 50ft turn radius!
100ft to make a u-turn... Plus urethane wheels gave a lot less traction than car tires. It would not be noticeable at all...
```

---
## \#52 Posted by: GhettoFab.rictation Posted at: 2017-11-07T11:57:20.364Z Reads: 190

```
Unless you did mountain board 6374 149kv like I was going to do<img src="/uploads/db1493/original/3X/c/c/cc7101036fff56e319905c20aad74baa4eb1875b.jpg" width="690" height="388">
```

---
## \#53 Posted by: Maxid Posted at: 2017-11-07T12:02:09.965Z Reads: 186

```
Are you seriously planning on using that pulley on a wheel this large?
```

---
## \#54 Posted by: GhettoFab.rictation Posted at: 2017-11-07T12:03:35.515Z Reads: 175

```
I have been but I have a large motor pulley,and I'm ghetto
```

---
## \#55 Posted by: Maxid Posted at: 2017-11-07T12:04:25.776Z Reads: 176

```
Makes no sense - small wheel pulley would only make sense with even smaller motor pulley.  Your ride must have been inefficient AF
```

---
## \#56 Posted by: GhettoFab.rictation Posted at: 2017-11-07T12:05:30.490Z Reads: 173

```
Are you sure because it works had a high top speed and I'm light took off amazing for everyone who wasn't 300lbs
```

---
## \#57 Posted by: GhettoFab.rictation Posted at: 2017-11-07T12:07:16.606Z Reads: 167

```
I'm broke dude and young... but I made it work rather than talk about what wouldn't work
```

---
## \#58 Posted by: Maxid Posted at: 2017-11-07T12:07:46.846Z Reads: 165

```
Everything will work - it's a matter of how well it will work. I myself was using a 35/14 on 10S and 149kv with 150mm wheels and it was not nice. You waste all torque for a top speed you'll never reach plus the inefficiency which is why I now ride uneven dual
```

---
## \#59 Posted by: GhettoFab.rictation Posted at: 2017-11-07T12:09:09.061Z Reads: 169

```
I reached mine on the 97mm when I put these on I had balance issues though.. hence the "high speed" 1$ ada tires under my hot gun I won in ebay hahah
```

---
## \#60 Posted by: Maxid Posted at: 2017-11-07T12:10:20.638Z Reads: 169

```
No idea what you are saying. You have to adjust your gearing when you switch tires as the diameter changes (especially when going for something drastic like those)
```

---
## \#61 Posted by: GhettoFab.rictation Posted at: 2017-11-07T12:11:16.241Z Reads: 155

```
Well yeah but I need balanced tires first is what I'm saying, not enough$ yet
```

---
## \#62 Posted by: GhettoFab.rictation Posted at: 2017-11-07T12:15:02.540Z Reads: 162

```
Unless you want to buy it for me haha, but as far as single drive maybe later this year I'll do a complete rebuild anyway I was thinking https://www.ebay.com/p/TOMCAT-G50cc-Gas-Giant-Airplanes-Brushless-Outrunner-180kv-Motor-Tc-g-8825-kv180/2162960030?iid=282090587473 this with a two speed transmission on new project with one wheel mayyybe two the motor would need to be modified though
```

---
## \#63 Posted by: Okami Posted at: 2017-12-11T13:14:12.944Z Reads: 157

```
@GhettoFab.rictation  Well.. that sure does look a bit funny - the big wheel with the small pulley.. anyway, have you made any other plans / progress with dual drive / single motor system or similar?
```

---
## \#64 Posted by: GhettoFab.rictation Posted at: 2017-12-11T22:49:09.712Z Reads: 163

```
<img src="/uploads/db1493/original/3X/2/9/29731a5899085e2387ee1a1d5b8b886dc39ceb37.jpg" width="281" height="500">
```

---
## \#65 Posted by: pat.speed Posted at: 2017-12-11T22:50:30.766Z Reads: 158

```
Is that a Jenso direct drive or Diy one?
```

---
## \#66 Posted by: GhettoFab.rictation Posted at: 2017-12-11T22:51:26.894Z Reads: 157

```
Jenso but I'm going to possibly make my own in the future for just my boards
```

---
## \#67 Posted by: Deckoz Posted at: 2017-12-12T05:15:38.059Z Reads: 162

```
[quote="jmasta, post:40, topic:34203"]
This has been discussed before, and I had the idea to use a 0° baseplate in the rear (1 motor powering both rear wheels).  With RKP geometry on a 0° plate, the truck will lean but does not produce any turn.  I understand the need for a differential in cars, but they have an axle length measured in feet;  a skateboard axle is so much shorter that the difference in speed between the inside and outside rear wheels would probably be negligible on a 0° baseplate.  Because once again, it's all lean and no turn.  A 50°/0° setup still turns because the rear tracks the front, much like a racecar

However I was basically called an idiot and told it would never work.  Because "physics". Like I'm sure high school physics was very challenging for you, but I have a Master's degree in engineering and still think it might work. Who's knows? Maybe I really am idiot :joy:  My coworker and some people on here sure thought so!

I am still undecided on how well it would work...
[/quote]

Well...
<img src="/uploads/db1493/original/3X/2/9/29c67b07b1d9398f64545ca187ed1917a9ccb0e3.jpg" width="550" height="332">

http://landyachtz-longboards.com/the_r5

Just saying...
```

---
## \#68 Posted by: lock Posted at: 2017-12-12T06:44:45.063Z Reads: 164

```
This thread just made me do some maths.

5m radius U-turn, 30cm (0.3m) truck width, 90mm (0.09m) wheels, 'locked diff'.

Inner wheel distance = 5 * pi = 15.71m
Outer wheel distance = (5 + 0.3) * pi = 16.65m
Difference = 0.94m = 0.94 / (2 * pi * 0.09/2) rev = 3.32 revolutions (over whole turn)

OR, for every 1m the inside wheel travels the outside wheel must travel 1.06m. 

It doesn't sound too bad in my unqualified opinion. I mean it's not like a car that has a similar turning radius, but much larger track width whereby the outer wheel might have to cover double the distance. But if that was the case why do RC cars have differentials.
```

---
## \#69 Posted by: mmaner Posted at: 2017-12-12T15:31:56.971Z Reads: 153

```
THe only advice I can give after shredding 3 buggy diffs is dont use stainless steel.  Use something harder and more resistant ti friction damage.  Steel at a minimum.  Maybe seal the diff and pack with lithium grease?
```

---
## \#70 Posted by: jmasta Posted at: 2017-12-13T01:53:30.872Z Reads: 152

```
[quote="Deckoz, post:67, topic:34203, full:true"]

Well...
<img src="/uploads/db1493/original/3X/2/9/29c67b07b1d9398f64545ca187ed1917a9ccb0e3.jpg" width="550" height="332">

http://landyachtz-longboards.com/the_r5

Just saying...
[/quote]

Not too sure what you are implying.  I know a 0° rear works fine on a typical skateboard.. I have a few setups like that.  I just don't know how well it would work with one motor powering both rear wheels on a zero degree plate.  Specifically is the turning radius of the inside rear wheel different from the outside rear wheel?  If it is different, is it significant enough to make a difference on a 0° rear?   Probably not

The physics get a little tricky.  With a normal setup, the outside wheels spin faster than the inside ones in a turn.  But on a zero degree plate, the rear does not actually turn.. it only leans.  So maybe the rear wheels are effectively pivoting instead?

An interesting test would be to mount a dual rear drive setup on a 0° plate. Then run bluetooth telemetry on both  VESC's and compare RPMs of the left/right wheel during turns
```

---
## \#71 Posted by: Deckoz Posted at: 2017-12-13T02:08:26.103Z Reads: 142

```
Well... At 45 degrees, you have an even amount of turn to lean. Really the important part is the turn. The more lean, and less turn you have...the less the wheels pivot as well. The closer the wheels stay to on track like a car, the greater the difference in speed between the inside and outside wheel. 

Where as when you have a truck with turn, it points into the turn, making the difference between the inner and outer wheels less...

If single motor doesn't feel right in the 40-60degree baseplate range. It will even more noticeable the inner outer difference the lower your baseplate angles...(higher 70-90 not realistic)
```

---
## \#72 Posted by: Rutherford Posted at: 2017-12-13T12:56:51.629Z Reads: 134

```
Maybe a torsion truck would help, seems like they turn more than they lean so they would point into the turn more? Might feel weird though and I don't know how it would be with one on the back only
```

---
## \#73 Posted by: Ouch Posted at: 2018-12-23T22:51:39.397Z Reads: 97

```
Has anyone actually tried this? Would be nice to hear from someone who actually had a go. I'm going to have a go, I think it could work, I don't think a diff is required due to the short track and no Ackerman, plus the out side wheel is unloaded during a turn and will be able to spin, + it works fine in a go kart!
```

---
## \#74 Posted by: sayekim Posted at: 2018-12-24T02:47:58.808Z Reads: 96

```
It’s been done but I don’t know what happened to it. 

http://esk8builds.com/photo/view/?id=120
```

---
## \#75 Posted by: Ouch Posted at: 2018-12-30T13:36:16.993Z Reads: 88

```
So I had a couple of hours in the work shop today, made a proof of concept.
Got to say solid rear axel works fine, I reduced the truck angle and the track, I have more grip in acceleration and breaking and it feels better in cornering especially when on power.
Really happy, if I can make it light enough it makes for a good dual light weight simple set up.
![IMG_20181229_183943498|375x500](upload://y9mt31IXFkVhV5OUJtwKikYyc15.jpeg)
```

---
## \#76 Posted by: hiboute Posted at: 2018-12-30T13:58:09.783Z Reads: 75

```
Yes, i know a builder in France who only use this for quad build. Those are real rockets. For having tried it, you don’t feel any difference. But i don’t think he is on this forum.![image|666x500](upload://3PlWKdBeKD6ga5nZhkOptaiIJ8F.jpeg)
```

---
## \#77 Posted by: hiboute Posted at: 2018-12-30T14:01:39.059Z Reads: 75

```
It is a 12s5p. With dual SK3 6374 with external sensor (in the black tube).
```

---
## \#78 Posted by: Riako Posted at: 2018-12-30T14:59:44.772Z Reads: 75

```
thx for share @hiboute ! I doesn't know this new build :blush: I like every picture he post on esk8 (is that right the Lyonnais rider ?)
```

---
## \#79 Posted by: drassak Posted at: 2019-01-02T16:08:38.560Z Reads: 55

```
it's lui meme :smiley:
```

---
## \#80 Posted by: Darkie02 Posted at: 2019-01-02T18:07:57.453Z Reads: 49

```
So are people saying most quad bikes and go carts that have locked rear axles can not turn a corner? Go look on YouTube and join the flat earth society! Not the most efficient way of turning but I can see more advantages better grip much better brakes. the negs wheels dragging on turns wereing out quicker larger turning radius.

All comes down to personal choice what you want to compromise on cost wight grip reliability.  There’s no right answer hear as long as it works for you.
```

---
