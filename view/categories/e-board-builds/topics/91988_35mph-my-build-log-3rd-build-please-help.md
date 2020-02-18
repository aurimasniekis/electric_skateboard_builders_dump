# 35mph+? My build log ,3rd build, please help

### Replies: 76 Views: 961

## \#1 Posted by: Halbj613 Posted at: 2019-04-27T20:57:40.030Z Reads: 222

```
Hi,

Recently I made a bet with my brother that I could achieve 35mph on my board, I live In London so the roads aren’t great, but they are manageable

Here is my build please tell me what you think(and if it will work)

This is a dual rear driven setup
........

Vesc: focbox unity

Battery: 12s5p Samsung 30q by @Tinp123 (great builder and sick prices)

Bms: 12s beseech bms

Trucks:caliber2

Motor mount: hobbyking mount

Pulleys: 40t abec 3d printed pulley

Motor pulley:14t diyeboard pulley
 
Enclosure: self built wooden one

Deck: meepo/wowgo style 10’’ deck

Wheels:abec11 97mm flywheel

Motors:currently Tb 260kv 6355 motors(I have been told the erpm will be to high) here is my calculation, if it is wrong I will change to some sk3 or Tb 190kv 6355

........


A unity can do 100000 erpm

100000/7 poles is around 14200

14200/260 is around 54

12s is 3.7  *12 which is around 44(even at full charge 12*  4.2 is around 50v)

So the unity and motor should all fit in together

......

Please tell me if I should reach the speed and also what range I will get

I haven’t bought any belts yet but am looking for some (not sure whether to use idlers)

Thank you any feedback (good or bad) is appreciated

Thank you
```

---
## \#2 Posted by: Skunk Posted at: 2019-04-27T21:11:22.575Z Reads: 200

```
Yeah don't go over 200kv at 12s

Also you might wanna go 36t or even 32t on wheel pullys if you want 35mph on 97mm wheels.
```

---
## \#3 Posted by: Halbj613 Posted at: 2019-04-27T21:20:12.115Z Reads: 195

```
Why does my calculation not work

Also with that gearing and that kv will it work
```

---
## \#4 Posted by: Arzamenable Posted at: 2019-04-27T21:30:53.266Z Reads: 192

```
http://calc.esk8.it/

These are helpful. Those higher kv motors (200kv and up) are sluggish off the line if you are only using two.
```

---
## \#5 Posted by: rusins Posted at: 2019-04-27T22:02:50.581Z Reads: 183

```
Yeah with your setup you're getting way too much speed on 260kv, even if "possible according to Unity specs" which I wouldn't want to trust with my life.

[260kv entered into calculator](https://calc.3dservisas.eu/?Tc-7DsIwDAXQf8mMUJq24bG6qBMoEhLdaYYg0YfUEfHv-N62wHbs2DfJy9wlmaN5PobebLS4aJFvvXqSqzpzZFCWlGDAWsuiQpXNBxVm3NxnZqYckZEDf3tjQLeguAQxKi9JND35DWqTLEltOqn2lrxhvYA7WZI6hDvPXhiwXpC_-zsZ1p_FZlIedmB9Xodj3eCBmI28zJv3Bw==)

Go with the 190kv motors and change motor pulley to 16t, then you'll get your 35mph speed

[190kv and 16T pulley](https://calc.3dservisas.eu/?Tc_NDsIgEATgd-FsDBSK1is1njQkJvZue8BEpEmPxnd3Z1p_bt8uuwM81TUktVP3W3molRQnKezai6dwFpuKjMKaChjQWrNoUZn5oMVMNfeZaYQjMizwtzdGdB3FJYhRtibR9OQ3qE9hSerTXrTV5AXrDs5hScp8dsNeLLAjf_fnUD4_G7pJ2GzAwxFdT3Z4IGYHXubV6w0=)
```

---
## \#6 Posted by: Arzamenable Posted at: 2019-04-27T22:30:40.654Z Reads: 180

```
I agree, 190kv and get several sizes of motor pulleys. 14,16, 18 maybe.
```

---
## \#7 Posted by: J0ker3366 Posted at: 2019-04-27T22:32:31.709Z Reads: 173

```
Think about going with TB 218mm trucks. The wider stance on those 97mm will give better stability @ higher speeds. Granted you should be fine. Just remember 218mm tucks if you get squirley
```

---
## \#8 Posted by: Halbj613 Posted at: 2019-04-27T23:43:46.440Z Reads: 160

```
What cheap 190kv motors are there

Also what would happen if I used the 260kv motors with the voltage limited until the new ones come

Also what would the range be
```

---
## \#9 Posted by: Halbj613 Posted at: 2019-04-27T23:44:34.382Z Reads: 147

```
What belt size should I go for
```

---
## \#10 Posted by: yelnats8j Posted at: 2019-04-27T23:58:04.234Z Reads: 148

```
@dickyho motors are cheap and good
```

---
## \#11 Posted by: rusins Posted at: 2019-04-28T00:23:50.976Z Reads: 151

```
@Arzamenable pulleys ain't free boy!

 @Halbj613 you said yourself that you could go for either 260kv or 190kv TB motors. Go for the 190kv, TB motors are good value for the price. If you have 260kv motors on hand then of course you can use those, but you'll get weak breaking as before and bad acceleration / unreachable top speed which is way too high. No need for voltage limiting if you use a Unity.

Choose belt size according to what motors and truck you choose, TB 6355 motors allow you to run 12mm belts on a standard caliber truck in dual configuration, other motors (with a sensor bit sticking out) will require wider trucks.

You seem to be posting a lot of topics as of recent with similar questions / problems. Most of this information is on the forum, just read more :upside_down_face:
```

---
## \#12 Posted by: KaramQ Posted at: 2019-04-28T05:23:44.312Z Reads: 129

```
Everything your looking for can be calculated on the 3d services calculator. As for belt size, there is also a calculator but it really depends on your motor mount/ wheel pulley/motor pulley
```

---
## \#13 Posted by: Halbj613 Posted at: 2019-04-28T07:17:57.795Z Reads: 121

```
To mount 6374 motors would I need the 218 truck
```

---
## \#14 Posted by: Jinra Posted at: 2019-04-28T07:25:21.865Z Reads: 115

```
You could use the spiral helical drive like I'll be doing
```

---
## \#15 Posted by: Halbj613 Posted at: 2019-04-28T07:25:55.424Z Reads: 115

```
What??

10cha
```

---
## \#16 Posted by: Jinra Posted at: 2019-04-28T07:31:14.671Z Reads: 113

```
https://www.electric-skateboard.builders/t/spiral-bevel-gears-gearbox-pre-order/84074
```

---
## \#17 Posted by: Halbj613 Posted at: 2019-04-28T07:33:33.859Z Reads: 110

```
Sorry nearing end of budget will just sell motors and try find some other 190kv ones

Does anyone know any other motors with similar kv as if I order from Tb they will take 6 months to come
```

---
## \#18 Posted by: Halbj613 Posted at: 2019-04-28T08:05:42.336Z Reads: 108

```
Where can I buy from that will come within 2 weeks
```

---
## \#19 Posted by: RedBaron Posted at: 2019-04-28T08:07:58.045Z Reads: 106

```
I use maytech 6374 motors. Pretty fast shipping and they haven't given me problems.
```

---
## \#20 Posted by: Itsmedant Posted at: 2019-04-28T08:10:08.047Z Reads: 104

```
This thread seems pretty familiar....
```

---
## \#21 Posted by: Halbj613 Posted at: 2019-04-28T08:11:54.840Z Reads: 93

```
For the trucks I am curently using I need 6355

Might switch up trucks though

Can y send link

Edit:going to have to buy larger trucks anyone got a god idea
```

---
## \#22 Posted by: Halbj613 Posted at: 2019-04-28T08:12:49.553Z Reads: 86

```
Also anyone know where to buy protective gear
```

---
## \#23 Posted by: RedBaron Posted at: 2019-04-28T08:13:12.319Z Reads: 85

```
Google search
```

---
## \#24 Posted by: dareno Posted at: 2019-04-28T08:19:19.965Z Reads: 84

```
12s 5p and 192 motors.  97mm wheels and 15/36 gearing,  35 is a breeze.  Just go do it sunshine.
```

---
## \#25 Posted by: Halbj613 Posted at: 2019-04-28T08:20:17.028Z Reads: 87

```
Thanks mate what about the same as you but with 14:34 gearing
```

---
## \#26 Posted by: dareno Posted at: 2019-04-28T08:25:06.202Z Reads: 83

```
Put it this way.  I can go over 40mph with my set up and yours is no different.  15/36 and 14/34 is not a big enough difference.  Are you sure you want to go 40 plus?  Its a different ball game at those speeds.  Trust me.
```

---
## \#27 Posted by: Halbj613 Posted at: 2019-04-28T08:25:27.011Z Reads: 82

```
No just need t reach 35
```

---
## \#28 Posted by: Halbj613 Posted at: 2019-04-28T09:21:37.967Z Reads: 84

```
Thanks to everyone for the help will upload more pictures soon
```

---
## \#30 Posted by: Halbj613 Posted at: 2019-04-28T10:14:19.571Z Reads: 88

```
Ordered 2 flipsky 6355 190kv motors

Are they any good
```

---
## \#31 Posted by: Halbj613 Posted at: 2019-05-01T19:04:04.559Z Reads: 79

```
So I am now up to the stage of thinking about an enclosure what are my options about buying one for under $100 which will fit the following dimensions if anyone knows anyone who will do one preferably in the Eu please say

Here are dimension 40cm long...16cm wide....4cm high

@bigben @psychotiller
```

---
## \#32 Posted by: KaramQ Posted at: 2019-05-01T19:06:27.007Z Reads: 74

```
IKEA
Stödja
```

---
## \#33 Posted by: Halbj613 Posted at: 2019-05-01T19:31:24.754Z Reads: 69

```
Yes I thought of that but isn’t it cheap quality and going to break easily
```

---
## \#34 Posted by: Halbj613 Posted at: 2019-05-01T19:37:59.489Z Reads: 66

```
What about using a wooden enclosure built by myself 

If yes how do I waterproof it
```

---
## \#35 Posted by: KaramQ Posted at: 2019-05-01T20:18:47.167Z Reads: 61

```
There like 1 Dollie and it’s flexible as hell, you could always buy multiple ones
```

---
## \#36 Posted by: Halbj613 Posted at: 2019-05-01T20:21:09.019Z Reads: 57

```
Is here anyway to strengthen it up and how do you screw it down to the board
```

---
## \#37 Posted by: J0ker3366 Posted at: 2019-05-01T20:21:37.312Z Reads: 60

```
&lrm; Kydex
```

---
## \#38 Posted by: Halbj613 Posted at: 2019-05-01T20:24:31.316Z Reads: 63

```
How do you press the keyed down
```

---
## \#39 Posted by: Halbj613 Posted at: 2019-05-01T20:24:44.627Z Reads: 62

```
Kydex

No keyed
```

---
## \#40 Posted by: J0ker3366 Posted at: 2019-05-01T20:24:52.694Z Reads: 60

```
With your hands or a negative of your mold
```

---
## \#41 Posted by: Halbj613 Posted at: 2019-05-01T20:26:23.453Z Reads: 59

```
As in don’t you need a vacuum press or heat press
```

---
## \#42 Posted by: J0ker3366 Posted at: 2019-05-01T20:26:56.337Z Reads: 54

```
No. Stand by for photos
```

---
## \#43 Posted by: Halbj613 Posted at: 2019-05-01T20:27:28.121Z Reads: 53

```
Standing by
```

---
## \#44 Posted by: bigben Posted at: 2019-05-01T20:29:35.553Z Reads: 54

```
With Kydex you could make a positive and a negative and probably make something pretty neat?
```

---
## \#45 Posted by: Halbj613 Posted at: 2019-05-01T20:30:53.097Z Reads: 61

```
[quote="bigben, post:44, topic:91988"]
positive and a negative
[/quote]
Those words mean nothing to me
```

---
## \#46 Posted by: J0ker3366 Posted at: 2019-05-01T20:31:48.707Z Reads: 66

```
All done by hand. Kydex hates 90° angles without a vacuum former though. But as you can see, even without a former, it comes out very good. I will eventually level both pieces and skin it in CF for a piece envlosure.
![20190501_142819|375x500](upload://d590jxDPU8fV5CiLSbmS8itzjx6.jpeg) ![20190501_142802|666x500](upload://s4pLoH0PROfJP9On1i9zciyyv76.jpeg) ![20190501_142739|375x500](upload://bl6LHqmwwLxhAJwNZ0KiYfb9U59.jpeg)
```

---
## \#47 Posted by: Halbj613 Posted at: 2019-05-01T20:32:56.133Z Reads: 59

```
Was looking at some videos about how to do it but how should I make the buck to begin with
```

---
## \#48 Posted by: J0ker3366 Posted at: 2019-05-01T20:34:34.203Z Reads: 60

```
I made a reinforced cardboard mock up (positive mold) and then applied the kydex and molded it with my hands (negative mold).
```

---
## \#49 Posted by: Halbj613 Posted at: 2019-05-01T20:36:04.828Z Reads: 61

```
Can you just heat up the kydex then just push it down with your hands onto a mould
```

---
## \#50 Posted by: Skunk Posted at: 2019-05-01T20:36:49.839Z Reads: 61

```
That's the idea.
```

---
## \#51 Posted by: J0ker3366 Posted at: 2019-05-01T20:38:04.582Z Reads: 67

```
&lrm; 👆👆👆👆
```

---
## \#52 Posted by: Halbj613 Posted at: 2019-05-01T20:38:45.328Z Reads: 68

```
K and can I just buy it on eBay also what does the mould need to be made out of
```

---
## \#53 Posted by: bigben Posted at: 2019-05-01T20:38:56.633Z Reads: 68

```
![fullsizeoutput_21af|690x268](upload://iEC5bpQUi45E1IKpc9Be1C16GlQ.jpeg)
```

---
## \#54 Posted by: Halbj613 Posted at: 2019-05-01T20:39:45.672Z Reads: 68

```
Also how thick does the kydex have to be
```

---
## \#55 Posted by: Skunk Posted at: 2019-05-01T20:40:04.390Z Reads: 67

```
Cardboard, wood, dirty clothes wrapped in duct tape. Your pick
```

---
## \#56 Posted by: Halbj613 Posted at: 2019-05-01T20:42:34.411Z Reads: 66

```
What thickness kydex and I will ask for some more help once I have finished mould
```

---
## \#57 Posted by: Halbj613 Posted at: 2019-05-01T20:46:42.107Z Reads: 65

```
In 2mm enough
```

---
## \#58 Posted by: brenternet Posted at: 2019-05-01T20:49:32.818Z Reads: 68

```
Does your brain and/or common sense think 2mm is enough?
```

---
## \#59 Posted by: J0ker3366 Posted at: 2019-05-01T20:50:19.994Z Reads: 64

```
[quote="Halbj613, post:52, topic:91988"]
what does the mould need to be made out of
[/quote]

Something structural. Meaning something you can put some weight on to mold to it. If it cant support pressure then your mold will colapse
```

---
## \#60 Posted by: Halbj613 Posted at: 2019-05-01T20:50:38.101Z Reads: 64

```
https://www.electric-skateboard.builders/t/thermoforming-a-kydex-battery-enclosure/8642
So this guy used 2mm

0.08inch =2mm
```

---
## \#61 Posted by: brenternet Posted at: 2019-05-01T20:52:24.669Z Reads: 63

```
You used search to answer your own question?!?!?!

BACK OUT BOYS, OUR WORK HERE IS FUCKING DONE
```

---
## \#62 Posted by: J0ker3366 Posted at: 2019-05-01T20:52:43.057Z Reads: 61

```
2mm is fine for an enclosure. @brenternet is just in a mood lol. I used 2mm on mine as well. I would advice though, if using 2mm, attach your components to your board. Dont let the components rest on the enclosure when mounted
```

---
## \#63 Posted by: Halbj613 Posted at: 2019-05-01T20:53:24.069Z Reads: 59

```
Would 3mm work any better
```

---
## \#64 Posted by: J0ker3366 Posted at: 2019-05-01T20:55:48.327Z Reads: 57

```
Thats for you to decide. 3mm is going to be a little more work to make it mold correctly. 2mm will work. Just velcro your components to your board.
```

---
## \#65 Posted by: Halbj613 Posted at: 2019-05-01T20:56:31.856Z Reads: 58

```
K cool will go for it how much of the stuff will I need
```

---
## \#66 Posted by: Halbj613 Posted at: 2019-05-01T20:56:51.534Z Reads: 57

```
Will a3 be fine or will I need a2
```

---
## \#67 Posted by: J0ker3366 Posted at: 2019-05-01T21:00:07.247Z Reads: 52

```
[quote="Halbj613, post:65, topic:91988"]
how much of the stuff
[/quote]

Amazon (ebay should have them as well) has 12"x12" sheets. I get a pack of 4 for around $20. Build your mold first for the board. Measure that mold and then buy sheets accordingly
```

---
## \#68 Posted by: Halbj613 Posted at: 2019-05-01T21:22:51.165Z Reads: 52

```
K thanks

10cha
```

---
## \#69 Posted by: stealth71 Posted at: 2019-05-01T22:12:12.878Z Reads: 59

```
2mm or .080 is plenty.  All my batteries and electronics are in the enclosures with no velcro.  Well over 200 miles and no problems.
```

---
## \#70 Posted by: Halbj613 Posted at: 2019-05-03T10:56:18.338Z Reads: 51

```
what bldc tool should i use for unity @Ackmaniac or the one on enertion website
```

---
## \#71 Posted by: J0ker3366 Posted at: 2019-05-03T23:45:14.042Z Reads: 48

```
Both are reliable. Ack is more techy though. Vesc tool is your less techy version.
```

---
## \#72 Posted by: Dougz Posted at: 2019-05-04T01:19:37.241Z Reads: 42

```
Hope you have some safety gear dude, make sure ya got a helmet on cause at 35mph!!!!
BE CAREFUL
```

---
## \#73 Posted by: kuphjr Posted at: 2019-05-04T18:12:48.911Z Reads: 40

```
As someone who has used dual 6355 w/ a 12s5p battery for nearly a year, I am disappointed with my low end torque when I geared it for a max speed for 40. (60A each 190kv 14/36 w/ 110mm wheels)


Spend the money and get 6374s if you have the cash. I have some on group buy now.

Don’t get me wrong, it’s still crazy powerful, but I wish I could accelerate as quickly as a bike from a slow speed or stop.
```

---
## \#74 Posted by: kuphjr Posted at: 2019-05-04T18:15:12.100Z Reads: 39

```
I think this thread is older than I realized. Sorry if it’s  irrelevant.  If you already have your 6355 motors I’d like to hear how they are performing for you.
```

---
## \#75 Posted by: RedBaron Posted at: 2019-05-04T18:41:46.063Z Reads: 38

```
3mm is crazy hard to work by hand. And most times its unevenly heated leading to warping. 2mm should be the minimum you use also.
```

---
## \#76 Posted by: Halbj613 Posted at: 2019-05-04T20:53:22.495Z Reads: 37

```
Thanks to everyone

Why does unity tool say it only supports firmware 2.53 I thought firmware goes up to something like 3.3
```

---
## \#77 Posted by: Halbj613 Posted at: 2019-05-12T21:13:58.227Z Reads: 28

```
So here is the update

Using flipsky 6355

Enclosure being made by @Tinp123

I have 15t motor pulley 

32 and 40t wheel pulley

Probably going to use 40:15

What do you think

....

Also starting to think about vesc settings such as motor min max and etc...
```

---
