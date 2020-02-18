# Planning my first build&hellip;any and all input welcomed (needed =)!

### Replies: 96 Views: 887

## \#1 Posted by: whaddys Posted at: 2019-05-11T02:36:35.327Z Reads: 195

```
So this is all new to me, I do however seem to have some semblance and general knowledge about the parts, how they're connected in the build.  RN I just ordered a deck and some wheels from muirskate.  This build's gonna be ongoing through the summer because I'm broke and can't buy all the parts at once.  Anyway, logistically I'm still trying to figure out the motor pulley situation with the venom magnums.  Saw OKP had a build with these but I haven't heard anything after posting on that thread and messaging him about pulleys.  I may have to find a way to design these pulleys myself over the summer, we'll see.  Any suggestions on how I should proceed with these wheels?  ![53%20PM|690x406](upload://8yvGQaOEiMD3FHUNivnmasdxze8.jpeg)
```

---
## \#2 Posted by: Saturn_Corp Posted at: 2019-05-11T02:37:15.561Z Reads: 176

```
Dayum, free sunglasses!
```

---
## \#3 Posted by: goldrabe Posted at: 2019-05-11T02:52:35.252Z Reads: 174

```
I think I have seen that @moon might have a pulley option for you.\
Nice deck choice I dig all Kicktail classic shaped decks. What battery are you going to use?
```

---
## \#4 Posted by: whaddys Posted at: 2019-05-11T03:28:25.515Z Reads: 172

```
Yeah I wanted a cruiser with a kicktail, it's what I'm used to riding since I was a kid.  I haven't decided on the battery yet, but once I get my board I'll start considering that.  I've heard enclosures are a real pain if you haven't planned it out right.  I want to minimize the chances of this board exploding so I need to really read up and make sure I understand batteries and appropriate output for the motor and what not.  Any suggestion on programs to use for mac that are like CalcRC for calculating all that stuff?  CalcRC sadly for windows only =(
```

---
## \#5 Posted by: Itsmedant Posted at: 2019-05-11T03:41:12.294Z Reads: 160

```
You don’t really need to do any “calculations” 
They’ve all been done for you on this forum! You may have to make a custom enclosure for that deck unless someone has already done one.

Or buy one made out of abs and form it yourself, then wrap it in carbon fiber to make it strong. Check out @Sender’s work with carbon fiber, the man is a genius with it.

Do you know what motors you are getting? I would start there (instead of figuring out your battery). 

Then pick out what VESC you are going with, you can set battery/amperage limits in your Vesc to make sure it pairs nicely with your motor. Stick with trusted vendors and you should be good.

Good luck on your build!
```

---
## \#6 Posted by: Itsmedant Posted at: 2019-05-11T03:42:21.861Z Reads: 150

```
Oh wait, you’re looking at an earth wing...

@bigben, weren’t you talking about making an enclosure for that deck?
```

---
## \#7 Posted by: dareno Posted at: 2019-05-11T03:44:12.517Z Reads: 146

```
Nice choices there.  Going to be a tricky build but worth it in the end.  @moon is going to love you for the wheel choice.
```

---
## \#8 Posted by: Sender Posted at: 2019-05-11T03:47:57.121Z Reads: 146

```
[quote="Itsmedant, post:6, topic:93439"]
@bigben, weren’t you talking about making an enclosure for that deck?
[/quote]

Yassssss EW deck enclosure!
```

---
## \#9 Posted by: goldrabe Posted at: 2019-05-11T03:49:10.804Z Reads: 142

```
Those are two good calculators, you can make your own enclosure out of glasfiber and epoxy fairly easy. Also psychotiller.com has many enclosure choices who might fit. Choose your battery according to your motor size, needed range, torque and topspeed you want to achieve.

https://calc.3dservisas.eu/

https://calc./#/0
```

---
## \#10 Posted by: whaddys Posted at: 2019-05-11T04:16:23.647Z Reads: 132

```
I'm thinking a 220kV motor?  I'm 6'1", 190 lbs and don't need to go more than 27 mph.  Some uphill capability would be nice for my area. 
I'm totally noob so pardon my totally nOOb questions here, BUT...
what about something like this:

https://www.alibaba.com/product-detail/Maytech-5055-220KV-Electric-Skateboard-brushless_60494888821.html

Also what does the "5055" part of "5055 220 kv" mean?  What's that a measurement of?
I know I need to consider max cuurent, max power, and max lipo. cell.  The values for these are 30A, 1170W and 2-10 lipos, however I'm not certain what all these numbers mean and how they translate to my build.  Sorry again for the nOOb questions.
```

---
## \#11 Posted by: Skunk Posted at: 2019-05-11T04:20:37.738Z Reads: 122

```
5055 or 5056 or 6355 or 6374 are the motors size (length&width) 

If you're going 12s its best to keep it under 200kv. 170kv is a nice sweet spot. 

Great deck choice.  I've got the 33 of that deck and the 37 is next on my list.

Heads up tho.  The deck is kinda thin.  Making it harder to install threaded inserts fot mounting the enclosure.
```

---
## \#12 Posted by: whaddys Posted at: 2019-05-11T04:54:03.278Z Reads: 120

```
Does this seem like a good choice if I'm going 12s4p?

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html

they seem maybe a little large.
```

---
## \#13 Posted by: moon Posted at: 2019-05-11T10:53:38.262Z Reads: 115

```
Saw the tag and was hoping speed vents 😂

I know @skunk is going to love the deck choice lol
```

---
## \#14 Posted by: dareno Posted at: 2019-05-11T11:23:13.402Z Reads: 110

```
[quote="whaddys, post:12, topic:93439"]
hey seem maybe a little large.
[/quote]

Mine is a little large.
```

---
## \#15 Posted by: b264 Posted at: 2019-05-11T11:26:12.610Z Reads: 107

```
How many motors: 1 or 2?
```

---
## \#16 Posted by: rusins Posted at: 2019-05-11T12:01:05.667Z Reads: 107

```
Just to sum up all the information currently given in this thread:

* Desired top speed: 27mph
* Needs enough torque to go up some hills
* Wheels are 78mm magnum's, meaning it's going to be a belt drive setup
* deck has a kicktale, meaning the enclosure needs to be small
* budget isn't infinite, can't go all out

For hills I would recommend a 63mm motor instead of a 50mm one. Because 27mph is quite fast, I assume you'll be riding on the road with cars, so having dual motors for extra traction and safety would be good (I think Brian would disagree though so it's debatable). I think it would be good to go for a drivechain solution that would allow you to upgrade to dual motors in the future if needed, but currently stick with a 1 motor setup just to keep the build costs low. Since you seem to be in north America, a TorqueBoards 6355 motor might be perfect, depending on the trucks / pulleys you can get.

Your range requirements + available enclosures will determine what kind of battery to get. (Lipo or Li-ion)
```

---
## \#17 Posted by: moon Posted at: 2019-05-11T12:03:50.412Z Reads: 100

```
No one mention the trucks?
```

---
## \#18 Posted by: whaddys Posted at: 2019-05-11T15:25:27.501Z Reads: 103

```
I'm thinking I'll go dual motors for the extra torque to help with uphill.  My budget is around $700-$800.  If it's an extra $100 for 2 motors vs. 1 I feel like that's worth it.  Belt drive for sure.  I'll be on the roads with thing, which I already do with my wowgo mini, but the dual hubs are terrible in terms of shock absorption.  Which is what inspired my build in the first place.  Having good wheels in the back seems like it would be a total game changer.  I figured I'll just take whatever trucks work with whatever mounts I can get, I feel like I can't be too choosey about the trucks.  Calibers seem to have the most options available for a secure motor mounting.  So for now I'm leaning toward those ToqueBoard 6355's @rusins.  Recommendations on trucks/pulleys for these motors?
```

---
## \#19 Posted by: whaddys Posted at: 2019-05-11T15:26:40.966Z Reads: 101

```
me thinks 2?
```

---
## \#20 Posted by: rusins Posted at: 2019-05-11T15:45:51.115Z Reads: 103

```
A dual drive VS single will cost you 1 additional  motor, 1 additional mount and pulley system, and 1 additional ESC unless you buy a dual drive ESC like the Focbox Unity from the get go. Usually it comes around to be an extra 300$ :confused:

Caliber 2 trucks might be fine for dual drive as long as you use 12mm wide belts and 8mm wide motor mounts. The hanger width is 184mm, meaning you have 92mm to fit each motor, mount, pulley system + wheel overhang. Kegel core wheels usually have a 12 - 15mm overhang so it fits with a 4mm space between the motors at worse, but I'm not sure about the dimensions of your wheels. You should ask someone, and also find out if 12mm pulleys are available.

If not, you'll have to go for a truck with a wider hanger, like TB extended 218mm caliber 2 clones. Best mounts for cheap are Dhiko's which you can find the ebay link somewhere on this forum. You can get motor pulleys from him too, or from TB. Wheel pulleys you need to get from someone on this forum who makes them.
```

---
## \#21 Posted by: moon Posted at: 2019-05-11T15:51:27.144Z Reads: 96

```
Yeah $800 for a dual is too small to make anything decent

And imo get a setup that allows you to upgrade to dual motors when needed 

So TB218mm or Surfrodz
```

---
## \#22 Posted by: whaddys Posted at: 2019-05-11T17:49:22.250Z Reads: 97

```
Alright, TB218's it is!  I'll drop the extra $$ for the dual, fuck it :grinning: I'm still on the fence about whether to get Turnigy Aerodrive SK3 - 6364-190kv or those those ToqueBoard 6355’s?  What are the main differences between these motors I should consider other than price?  
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html
https:///products/electric-skateboard-motor-6355-190kv
```

---
## \#23 Posted by: b264 Posted at: 2019-05-11T18:37:59.883Z Reads: 91

```
The @torqueboards 6355 now are shipping pre-battle-hardened, so the choice is very, very easy :smiley:

Get the ones with the epoxy, aka the TB 6355
```

---
## \#24 Posted by: Arzamenable Posted at: 2019-05-11T18:42:30.383Z Reads: 90

```
Does the epoxy help with cracked magnets or is epoxy on the stator side?
```

---
## \#25 Posted by: b264 Posted at: 2019-05-11T19:02:23.060Z Reads: 89

```
Yes, yes, yes

Hopefully it's on both sides.  We need a new thread for reviewing these motors, they just dropped a couple days ago.
```

---
## \#26 Posted by: BigZwatt Posted at: 2019-05-11T19:28:56.385Z Reads: 88

```
Got my motor apart its toast so ill be getting @torqueboards 6374s ASAP
```

---
## \#27 Posted by: Skunk Posted at: 2019-05-11T19:29:11.203Z Reads: 91

```
I've never owned either brand.  The TB motors (6355) tho i feel like have a better warranty seeing the owner of the site is a community member. 

Alot if guys use both of those tho.  
They are the same kv so will be similar speeds but the bigger motor will stay cooler while doing it.

These are also on sale.
https://buildkitboards.com/products/6354-208kv-motor


Personally i run maytech motors on all my builds. But i understand setting budget.
```

---
## \#28 Posted by: b264 Posted at: 2019-05-11T20:01:58.007Z Reads: 87

```
The older TB6355 are really good.  The new ones I have not tried yet, they just dropped mere days ago
```

---
## \#29 Posted by: BigZwatt Posted at: 2019-05-11T20:06:26.964Z Reads: 86

```
@torqueboards if yall need someone to review your new motors. I live near Posper, TX
```

---
## \#30 Posted by: mmaner Posted at: 2019-05-11T20:11:52.590Z Reads: 88

```
You can build a single motor esk8 and then upgrade to dual later. I'm not saying you should, just that it's an option. 

Maybe look for a couple of refurbished or used focbox's to save some cash. 

@okp is still testing his SV pulley and mount system, prolly a couple of weeks it at first. It won't be cheap either, he makes quality gear. 

I'd suggest looking at flywheels and caliber 2s,  is ask @jlabsb about motor mounts, he had dinner that are easy to install and rockk solid. He has some good flywheel cones as well. 

Both @JLabs and @torqueboards motors are quality, you'll be happy with either one.
```

---
## \#31 Posted by: whaddys Posted at: 2019-05-11T20:56:51.181Z Reads: 83

```
So I'm thinking of just going all TB for the trucks, motors, and mounts: TB6355, TB218mm trucks and the V5 dual motor mount set.  I'm looking at the bottom and it says compatible with 6374 motors.  These are compatible with the 6355's too right?  IDK, getting all this stuff from TB seems like the easiest route for getting all this to fit together no?
https:///collections/electric-skateboard-motor-mounts/products/v5-fixed-motor-mount-set
```

---
## \#32 Posted by: Skunk Posted at: 2019-05-11T21:03:57.134Z Reads: 78

```
6355 6364 6374 6380 wil all have same mounting patterns.
63xx or 50xx is the important part when matching motors to mounts
```

---
## \#33 Posted by: dareno Posted at: 2019-05-12T01:24:28.659Z Reads: 79

```
I use a fair bit of tb stuff and that v5 mount is a good quality item.  The motors used to have a few issues but they have been sorted now but no real testing has been done yet.  The sk3 motor you linked is however pretty much bullet proof but is a sensorless unit.  Sensors just stop the cogging or shuddering you get when starting from a dead stop.  I barely notice it on my set up.  They are a big unit though measuring in at 86mm end to end so with that mount being fixed you may run into problems getting 2 in there.  They do fit the tb 6374/6380 and for someone of your weight thats the size I would be going for.  Not much difference in the power but the 6355 will get hotter when you push them.  Grab the lot from torqueboards and be assured that it all goes together and you will get some good back up.
```

---
## \#34 Posted by: torqueboards Posted at: 2019-05-12T02:40:17.546Z Reads: 77

```
@whaddys - Stick to 15mm wide belts as they'll be the compatible option for our AT tires in a few months if you want to go pneumatics.
```

---
## \#35 Posted by: whaddys Posted at: 2019-05-12T06:24:17.080Z Reads: 79

```
So just for logistics sake here, say I get everything TB; the 218mm trucks, dual 6355 (@dareno you think I should go 6374/6380?), 15mm belts, which motor pulleys do I go for?  Obviously15mm, but how many teeth?  Is there a consideration between motor pulleys, # of teeth on the motor pulleys and # of teeth on wheel pulleys that I need to consider in terms of compatibility with each other?  My main concern is that in the end all this is compatible with the wheel pulleys which I'll have to find from someone on the forum, and so far okc is the only on I've seen with anything.  I just don't know if his are going to be compatible or if he will even have any to sell me, I haven't gotten a response from him yet.  This is the nitty gritty part that I'm still clearly not very knowledgable on yet, I just want to make sure all the parts (specifically the pulleys and belts) will fit in the end before I buy all that stuff from TB.  Thanks again everyone for being patient with a noob and helping guide me in this!  This community is reallly badass!
```

---
## \#36 Posted by: rusins Posted at: 2019-05-12T16:44:15.678Z Reads: 73

```
@okp's pulleys for the magnums are 32T (tooth). TB motors are 190kv. Hard to say what motor pulley tooth count you should go for before you've decided what battery you'll be getting. You can use [this simple esk8 calculator](http://calc.esk8.it/#{%22batt-type-lipo%22:0,%22batt-cells%22:10,%22motor-kv%22:190,%22system-efficiency%22:85,%22motor-pulley-teeth%22:15,%22wheel-pulley-teeth%22:32,%22wheel-size%22:78}|) to see how different battery configs will affect your top speed.

However, you don't want too few teeth, because then your belts could slip. I'm using 14T pulleys and my belt slips if the tension isn't perfect, so I would recommend either 15T or higher.

Playing around with the more advanced calculator ([calc.3dservisas.eu](https://calc.3dservisas.eu/?Tc7BCsIwEATQf8lZJLFprF6jeFICBXu3HiKYNtCj-O_uTIJ6ezvsTvJSNx_VXj0f86RWMlxkaNZOvPhebDQZhJbyWNC6xAdMpi3Gzqbk7DTCjI4G-LvLoa91OfAIYlXTkggd-S0ao69NYzyKOk1ecW7h5GtT4rd3zMIMW_L3fvKMsXwfFuG2A09npI4csM0FPubU-wM=)) to see minimum speed as well, I think 16T motor pulleys with a 10s Li-ion battery would be perfect, giving you an average loaded speed of 27mph, and max loaded speed of 31mph. (Minimum 22.5mph)

As for motors: dual 6355 will be completely enough for you; my dual 6355 bring me up steep hills just fine; would be silly to put anything heavier on your kicktale deck anyway :slight_smile:
```

---
## \#37 Posted by: rusins Posted at: 2019-05-12T16:53:27.868Z Reads: 69

```
Just realized @okp's pulleys have an integrated bearing (they don't clamp onto the wheels from both sides), so you'll need a truck with an extended axle to use them. Luckily, the TB trucks have an extended axle, so they are still a great choice.
```

---
## \#38 Posted by: Skunk Posted at: 2019-05-12T17:25:50.712Z Reads: 67

```
Is it enough axle tho?  I know he designed them on surfrodz trucks which have shoulder bolts for axles so you can get different lengths.
```

---
## \#39 Posted by: Skunk Posted at: 2019-05-12T17:34:38.390Z Reads: 66

```
[quote="whaddys, post:35, topic:93439"]
Is there a consideration between motor pulleys, # of teeth on the motor pulleys and # of teeth on wheel pulleys that I need to consider in terms of compatibility with each other?
[/quote]

So. The closer together the teeth count, the higher the top speed. Further apart, more acceleration. 

So let's say you start at 16t motor pulleys and 40t wheel pulleys. 
If you went from 40t to 42t on wheels, you'd lose top speed for more acceleration.  Or you could go to 32t (wheel pulleys) for higher top speed. 

Now if you go from 16t (motor pulleys) to 18t , you'll now be at 18-40.  you'll lose acceleration for speed this time.
```

---
## \#40 Posted by: wafflejock Posted at: 2019-05-12T17:41:13.164Z Reads: 64

```
Just to add about the belt size, there is length and width of the belt (as well as tooth shape/spacing but that's basically standardized).  Think most people here use at least 12mm wide belt but 9 or 15 are options too, wider the belt less likely it will break (also want it tensioned tight enough to not have teeth skip but not so tight to put stress on the bearings in the motor).  The motor mounts typically have a slot for the screws so you can adjust the tension by hand (would be nice to have a bolt for this like on my mk3 printer but hand tensioning works fine).  The length of belt will depend mostly on the diameter of the wheel pulley.
```

---
## \#41 Posted by: Skunk Posted at: 2019-05-12T17:47:04.708Z Reads: 68

```
I'll also mention that these wheels are wide.  On tb trucks you're gonna have a real wide stance.
@Frenchy has a great picture of them on multiple sets of trucks.

I wanna get a set but i plan on running 150mm rkp sr or 100mm tkp sr and running dual diagonal motors.

Found it.*

![0e50b139960fbb4d21bd949c674a28ba43e46fba_2_750x1000|375x500](upload://20u6tx1FNbcjAcGrp4has9ZH2Sy.jpeg)
```

---
## \#42 Posted by: rusins Posted at: 2019-05-12T17:57:20.852Z Reads: 66

```
Yes, TB website says the axles are also 10mm longer than standard longboard trucks.
```

---
## \#43 Posted by: whaddys Posted at: 2019-05-12T18:29:10.033Z Reads: 64

```
oh hell yeah, thanks so much for that explanation @Skunk I understand the meaning of that ratio a lot better now!
```

---
## \#44 Posted by: Skunk Posted at: 2019-05-12T18:31:00.977Z Reads: 60

```
No problem.  Took me a bit to understand myself.
```

---
## \#45 Posted by: whaddys Posted at: 2019-05-12T18:33:28.854Z Reads: 60

```
I know, they're insanely wide and have a pretty big overhang but the wideness of them is what I love about those magnums.  I used to have a long board with some really wide 75mm Bustin William Royce's, and I loooove the feel of those wheels.  Sadly they are completely solid units and I couldn't mount them
```

---
## \#46 Posted by: Skunk Posted at: 2019-05-12T18:38:27.548Z Reads: 63

```
I totally agree, I love really wide wheels. I wish I could adapt more of my old downhill Wheels to esk8 without just drilling holes in good urethane.
I plan on picking a set of these wheels up but I'm going to find the narrowest trucks I can (that have mounts available) and run diagonal Motors.
```

---
## \#47 Posted by: Skunk Posted at: 2019-05-12T18:40:19.025Z Reads: 61

```
I think @psychotiller new hex hanger trucks would be rad if he'll do a custom hanger length. 
That or Ronin katanas..... mmmmm
```

---
## \#48 Posted by: moon Posted at: 2019-05-12T18:44:57.910Z Reads: 59

```
Needs to be better truck options out there for sure
```

---
## \#49 Posted by: Skunk Posted at: 2019-05-12T18:46:35.686Z Reads: 60

```
High end precision are just so expensive lol.
It's hard enough to convince people that surfrodz are worth it over calibers.
```

---
## \#50 Posted by: whaddys Posted at: 2019-05-12T19:21:33.869Z Reads: 59

```
I'm a little worried about fitting a 15mm belt considering how aggressive the overhang is on those... @Skunk  Are those 12mm's in the photo?
```

---
## \#51 Posted by: Skunk Posted at: 2019-05-12T19:23:03.592Z Reads: 59

```
Idk.... have to ask @Frenchy
```

---
## \#52 Posted by: whaddys Posted at: 2019-05-12T19:33:17.167Z Reads: 61

```
@Frenchy what's the set-up you've got going for your venom MACH 1's?  I'm trying to see if 15mm belt will fit with that overhang.  Those look friggin beautiful BTW
```

---
## \#53 Posted by: Skunk Posted at: 2019-05-12T19:35:53.107Z Reads: 60

```
[quote="whaddys, post:50, topic:93439"]
I’m a little worried about fitting a 15mm belt considering how aggressive the overhang is on those
[/quote]

If you go surfrodz you can just replace with longer axles and add wheel spacers and make it fit no matter what.
```

---
## \#54 Posted by: whaddys Posted at: 2019-05-12T19:42:46.051Z Reads: 54

```
Yeah 10s4p seems like a solid standard for my first build
```

---
## \#55 Posted by: whaddys Posted at: 2019-05-12T23:06:34.763Z Reads: 52

```
Does anyone know  a guide to help understand the torque ratings anywhere?  Trying to figure out what the different between 9.5 ft-lbs and 10.5 ft-lbs would feel like.
```

---
## \#56 Posted by: rusins Posted at: 2019-05-13T00:09:59.155Z Reads: 53

```
Probably miniscule. In either case, the torque ratings shown by the calculator are incorrect, because they assume the motors will be run at a current equal to their power in watts divided by system voltage, whereas actually for startup acceleration and hill climbing at below max speed, you can drive the motors with more current than your battery can give. It comes down to what your ESC can handle and how hot your motors get (larger motors get hot slower/less). 

You just have to trust that dual 6355 motors paired with a VESC is way more powerful than most if not all premade production boards. As long as your theoretical max speed (based on battery size, motor kv, pulleys and wheel size) isn't ridiculously above what you'll be actually using, the torque will be just fine ;)
```

---
## \#57 Posted by: J0ker3366 Posted at: 2019-05-13T01:49:17.584Z Reads: 51

```
[quote="rusins, post:16, topic:93439"]
Because 27mph is quite fast,
[/quote]

The need for speed is not within this one, young padawon.
```

---
## \#58 Posted by: Frenchy Posted at: 2019-05-13T02:48:55.805Z Reads: 52

```
Those are 140 bear Kodiak trucks with 14mm extended axels to make a160mm hanger with normal 33mm Axel's..it's like a 14mm axel extension for removable Axel's makes them about 47mm of axel to play with with fits a press fit and a bearing.. now those are 36t x 12mm pully..and it's tight I'm going with a 32 for smidge more clearence and top end
```

---
## \#59 Posted by: Frenchy Posted at: 2019-05-13T03:11:42.184Z Reads: 50

```
[quote="moon, post:48, topic:93439, full:true"]
Needs to be better truck options out there for sure
[/quote]

Please some one do a area rf1 that's all we need trust me ..

[quote="Skunk, post:49, topic:93439"]
so expensive lol. It’s hard enough to convince people that surfrodz are worth it over calibers
[/quote]
Lol  surf rodz are not real precision just because they have nice shinny colors and machines that do the work and making of the truck don't make them precision at all for exactly what we do..they are expensive cheap ass truck that just work better then a stock caliber for comparison ..there is a big article here just to make them actually work properly by alpamail the bushing master ..the bushing seat suck and the adjustble base plates are another story ..but ya ..caliber are great lol..Paris is batter I'd say.. and CRonin are the best bang for a buck until we get some AERA RF1 MOUNTS..
```

---
## \#60 Posted by: Skunk Posted at: 2019-05-13T03:29:01.513Z Reads: 47

```
[quote="Frenchy, post:59, topic:93439"]
Lol surf rodz are not real precision just because they have nice shinny colors
[/quote]

Did i say they were? Nope.
```

---
## \#61 Posted by: whaddys Posted at: 2019-05-13T03:57:56.423Z Reads: 44

```
@Frenchy thanks for the input!  I wanted to get the TB 218mm trucks which have a 47mm axel, and their V5 dual mount set and 15mm belts.  If you're running 47mm axels with 12mm belts and it's tight, that means I won't be able to get away with 15mm belts on my build eh??
```

---
## \#62 Posted by: Frenchy Posted at: 2019-05-13T04:09:12.006Z Reads: 47

```
@whaddys  Tb 218mm truck are as wide a 747 jet there are 320mm wide you can fit all sorts on there..those trucks I have are bear Kodiak precision trucks 140mm with the extended axels makes them total of 240mm wide..
```

---
## \#63 Posted by: Frenchy Posted at: 2019-05-13T04:13:03.007Z Reads: 47

```
[quote="Skunk, post:60, topic:93439"]
Did i say they were? Nope.
[/quote]

Yes you are correct sorry if it sounded that way I was just chuckling and throwing it out there as they are NOT precision as you like to rep the shit out of them and could use some of that help with real equipment ..
```

---
## \#64 Posted by: Skunk Posted at: 2019-05-13T04:19:06.314Z Reads: 48

```
[quote="Frenchy, post:63, topic:93439"]
as you like to rep the shit out of them and could use some of that help with real equipment …
[/quote]

Get off your high horse. 
Ya i can't drop $300+ on Ronins. No help needed, thanks.
```

---
## \#65 Posted by: whaddys Posted at: 2019-05-13T05:18:01.542Z Reads: 49

```
So I gotta figure out this battery situation here, which is a whole other shibang now...I know I'm going 10s4p lion, my question is do I find a pack and order it online and what should I look out for?  I have zero capabilities in building a pack, I've seen some people get packs custom built from folks on this forum, and I've also read about having to open enclosures and recharge batteries everytime?  Do I just want a battery pack and a BMS if I want to build this so that I can simply plug it into the wall without opening enclosures all the time?
```

---
## \#66 Posted by: Skunk Posted at: 2019-05-13T05:34:57.470Z Reads: 50

```
I'd recommend @psychotiller or @hyperIon1 for buying a battery.  (Both my batterys came from them) 
Theres also guys like @longhairedboy  & @thisguyhere but i personally haven't used them so im only recommending what i have experience with.
```

---
## \#67 Posted by: whaddys Posted at: 2019-05-13T15:39:25.968Z Reads: 46

```
hot damn those suckers are expensive.  Do you save yourself maybe $100 if you build the pack yourself vs. buying a pack?  I'll prolly order from @psychotiller but i'm just curious about the price diff.
```

---
## \#68 Posted by: Skunk Posted at: 2019-05-13T15:42:37.284Z Reads: 47

```
[quote="whaddys, post:67, topic:93439"]
Do you save yourself maybe $100 if you build the pack yourself vs. buying a pack?
[/quote]

With the investment in tools and supplies and the potential for wasted materials during learning  you only really save money if you plan on building more than a few batteries.

Not to mention if you build a battery incorrectly or poorly, you're making a bomb that will burn down your house.
```

---
## \#69 Posted by: whaddys Posted at: 2019-05-13T17:57:38.402Z Reads: 41

```
Well guys, I'm about to drop some serious cash at torqueboards, going with them all across the board for motors, turcks, mounts, pulleys, battery and vescs.  They have some kits that will save me a little $$ plus they seem like they're reliable and decent quality.  I'm gonna take their 12s4p battery instead of finding a 10s4p because they come with an enclosure and the price seems right.  Also I'm getting the kit to mount kegels so I can mount the caguamas I got lying around while I wait for a pulley option to become available for the MACH 1's.  So I'll be sacrificing some torque all together but gaining some top speed and range on my cags for the time being.  I still need a remote, and I wasn't too impressed with TB's remote options.  Any suggestions?  Anything I need to consider when buying a remote in terms of compatibility with TB's vesc's?
```

---
## \#70 Posted by: Saturn_Corp Posted at: 2019-05-13T23:20:02.017Z Reads: 38

```
it's a good batt, you won't be dissapointed. 

I think the bkb mini will work and it's pretty cheap and loads of people like it. I'm about to try it out in a few weeks as well.

GT2b never is a bad choice, it's a bit bulky though if you don't modify the housing. That's my daily driver and it's top notch.

A more expensive option is the Hoyte puck remote, they should have a cheaper ~$100 version coming out soonish.
```

---
## \#71 Posted by: Saturn_Corp Posted at: 2019-05-13T23:22:24.739Z Reads: 36

```
I should say though, the included 2 amp charger for the 12s4p is god awfully slow to charge. If you completely empty your pack it's gonna be 10+ hours to charge to full again. Best pick up the 4 amp one or a different 12s one that has an even higher amp rating.
```

---
## \#72 Posted by: whaddys Posted at: 2019-05-14T00:38:39.976Z Reads: 37

```
cool, thanks for the heads up!:grinning: any idea what sort of range I could expect for a 190 lb-er?
```

---
## \#73 Posted by: Saturn_Corp Posted at: 2019-05-14T00:46:02.664Z Reads: 37

```
Depends on quite a few things. I would say 20-30 miles. 

I get about 30 miles on mine. I weigh 130 lbs and get around 11wh/mi.
```

---
## \#74 Posted by: whaddys Posted at: 2019-05-14T01:14:49.090Z Reads: 37

```
OK @torqueboards I just dropped some big time $$.  Lemme know if you got any coupons when those AT wheels come out :joy::rofl::sweat_smile: ![21%20PM|499x500](upload://noZayCm3l5ZMnp06MaiqyB6r1xq.png)
```

---
## \#75 Posted by: torqueboards Posted at: 2019-05-14T03:38:23.160Z Reads: 35

```
@whaddys working on em! :smile:
```

---
## \#76 Posted by: whaddys Posted at: 2019-05-15T18:41:44.164Z Reads: 27

```
Shoot, well I think I goofed up and didn't consider my bettery and vesc enclosure sizes fitting on my deck.  #nOOb shit.  The deck has a 20.5-24in wheel base and the 12s4p battery enclosure from TB is 20.2 in. long.  I didn't take into account clearance for the motors and VESC mounts, clearly, and goofed this one up.  Am I SOL now for using this deck with all these parts?  Here's another look at all the pieces I got:

https://www.muirskate.com/longboard/decks/55251/earthwing-muirderer-fallen-one-37-longboard-skateboard-deck-w-grip

https:///collections/battery-enclosures/products/12s4p-enclosure-v2

https:///collections/electric-skateboard-pulley-belt-combo-kits/products/36t-kegel-pulley-15mm-combo-kit

https:///collections/electric-skateboard-motor-mounts/products/v5-fixed-motor-mount-set

https:///collections/electric-skateboard-power-kits/products/dual-motor-electric-skateboard-kit
```

---
## \#77 Posted by: Skunk Posted at: 2019-05-15T18:45:40.570Z Reads: 27

```
Well you could put the motors under the tail.  But that would kinda ruin you using the tail.
Or...

You can do what im doing and go forward mount on fwd.

Im actually doing it on the 33 inche version of that muirskate deck.
```

---
## \#78 Posted by: Sn4pz Posted at: 2019-05-15T18:46:03.861Z Reads: 30

```
To be frank with you, the TB enclosures used to be quite brittle.  If your deck allows you to use it (flex /  concavity wise) then go for it. Otherwise, you might be interested in looking at other solutions when the time comes. 

@eboosted and @bigben are the two most prominent figures in the enclosure bizzy
```

---
## \#79 Posted by: Skunk Posted at: 2019-05-15T18:46:29.616Z Reads: 30

```
![b93768934bf48a74af426365e078c802542baa80_2_1332x1000|666x500](upload://6Nld1gC7GizbTaKJSbM5EvSvq3A.jpeg) ![4d9fa5c90b63cc8a17a0e8fb7c32791f31fa4df6_2_1332x1000|666x500](upload://c8Hsr74DglogIxkqPiTIkmSnOW5.jpeg) ![39afdf183caf40e73ef265dfaccac88ac75ba874_2_1332x1000|666x500](upload://mRHxAZsVHhYZRiHm6nRwZWmpmX4.jpeg) ![8230af88fc74e484529b5fca57a3def3b3867878_2_750x1000|375x500](upload://62vRwUevHXPq5TQcRRguXD7I6x5.jpeg)
```

---
## \#80 Posted by: Skunk Posted at: 2019-05-15T18:48:57.511Z Reads: 28

```
[quote="Sn4pz, post:78, topic:93439"]
@bigben are the two most prominent figures in the enclosure bizzy
[/quote]

Is actually going to be making an enclosure that should fit this deck very well but it's going to be a while.
```

---
## \#81 Posted by: Sn4pz Posted at: 2019-05-15T18:49:59.138Z Reads: 28

```
[quote="Skunk, post:80, topic:93439"]
Is actually going to be making an enclosure that should fit this deck very well but it’s going to be a while.
[/quote]


Additionally, Ben tends to be cheaper. Im not sure if thats because of a difference in materials, but I havnt heard much to complain about from either vendor. :+1:
```

---
## \#82 Posted by: whaddys Posted at: 2019-05-15T18:50:40.049Z Reads: 30

```
Ahh, i see I see!  Hmmm...Well I already ordered the V5 motor mounts for inward mounting; they have an outward mounting option but I opted inward.  I guess I'll just have to see what this all looks like when it arrives, getting a different board style seems like the easiest route.  Ahhh so much to think about...
```

---
## \#83 Posted by: Skunk Posted at: 2019-05-15T18:51:42.318Z Reads: 29

```
[quote="Sn4pz, post:81, topic:93439"]
Im not sure if thats because of a difference in materials,
[/quote]

Not really. 
 Form/ function = eboosted/ bigben
```

---
## \#84 Posted by: Skunk Posted at: 2019-05-15T18:52:14.116Z Reads: 26

```
You already have the deck?
```

---
## \#85 Posted by: whaddys Posted at: 2019-05-15T18:52:47.683Z Reads: 27

```
@Skunk how long is "a while"?? :joy:
```

---
## \#86 Posted by: whaddys Posted at: 2019-05-15T18:53:06.072Z Reads: 27

```
It's on it's way
Friday should be here
```

---
## \#87 Posted by: Skunk Posted at: 2019-05-15T18:53:15.232Z Reads: 27

```
He's a busy guy with other enclosures to make and he doesn't even have the deck to mock up an enclosure on yet.
```

---
## \#88 Posted by: Skunk Posted at: 2019-05-15T18:56:17.922Z Reads: 25

```
I've got a first gen landyachtz osteon deck. Used but great shape. 
Its a bit thicker than the muirskate deck ( which is great for getting threaded inserts installed)

![748d2de7d441b2ef8a3ad5849c0ab9124b826142|666x500](upload://gD3Rr17LD9By20kCpu3NvkmVFu2.jpeg) ![76b5de9f6cafada1b40c80757275c279ac1f4d70|375x500](upload://gW9ZIedDrklq8Ea6d7YqkxJXNEA.jpeg) ![b3ac69ad685764204ab84d10f77580138e363dfe|375x500](upload://pDsRjAIKd9g7PNLZgDF44NQasA6.jpeg) 

Should fit your enclosure/ motors no problem. 
I'd be open to trading. If that deck doesn't work for you.
```

---
## \#89 Posted by: whaddys Posted at: 2019-05-15T19:01:14.911Z Reads: 25

```
Oh shizzy, that's pretty slick I likey!  What's the clearance between trucks?  I still gotta fit my VESC on there too, not sure how big that enclose will be but prolly atleast 6 in?  Unless  there's a more efficient way of mounting dual vescs?  This deck is v cool though and I'm def interested, will keep U informed when the earthwing shows up!
```

---
## \#90 Posted by: Skunk Posted at: 2019-05-15T19:01:19.970Z Reads: 23

```
I really don't want to have to drill all the way through my deck to mount my enclosure but none of the five different types of threaded inserts I have are short enough for how thin the 33 inch version of that deck is.
Hopefully the 37 is a few layers thicker. 
I'm probably going to try and pool up some epoxy on the bottom to add some girth to the bottom of the.
```

---
## \#91 Posted by: Skunk Posted at: 2019-05-15T19:06:03.007Z Reads: 23

```
Max wheel base is like 26.5

It's got a really nice subtle microdrop in the nose that kind of acts as a footstop and helps you really get locked in.

I really like the deck and I've been wanting to Electrify it for a while, but I've got multiple projects and no funds to finish them lol. 

So if its a better fit for you just say the word.
```

---
## \#92 Posted by: whaddys Posted at: 2019-05-15T19:07:40.061Z Reads: 23

```
@Skunk is it hard to find short enough threaded inserts?
```

---
## \#93 Posted by: whaddys Posted at: 2019-05-15T19:08:38.767Z Reads: 23

```
I also have this thing lying around

![IMG_4762|375x500](upload://lSCFsRu1PhOUgeVQZRbY9QA4fMQ.jpeg)
```

---
## \#94 Posted by: Skunk Posted at: 2019-05-15T19:08:53.658Z Reads: 23

```
I haven't really tried, I just already have a bunch of different kinds. I would imagine that the 37 has to be a few Plies thicker than the 33 tho.
```

---
## \#95 Posted by: Skunk Posted at: 2019-05-15T19:11:10.212Z Reads: 25

```
Looks like it migh be flexible.  

Personally,  i like flexible decks for pushing and pumping or going 25mph and under.
I don't want flex going 30mph +

But thats just me.

Looks like a nice deck tho.  Definitely a solid brand.
```

---
## \#96 Posted by: whaddys Posted at: 2019-05-15T19:14:51.334Z Reads: 24

```
@Skunk Yeah it's pretty flexy.  SUBOPTIMAL at best for this build.  I'll be in touch about that trade though!
```

---
