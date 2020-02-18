# Maytech 90mm 60kv 800W hubs trouble shooting

### Replies: 59 Views: 2043

## \#1 Posted by: goldrabe Posted at: 2017-09-30T03:17:18.176Z Reads: 221

```
Hi there,
please help me with my build!
I bought two 90mm 60kv 800W Maytech hubs, a 10S5P battery and a esc for dual hub motors which looks similar to the one used in the Meepo board. I could assemble everything and wire it correctly, but somehow top speed and torque is quite disappointing. Also the range i will get with this large battery seems to be off, i only can ride it for a max 12 Miles. My top speed is like 15-16 mph. And the motors are really getting hot. 
Now if i would replace the esc with two vescs will this improve speed, torque and range, or are the motors just so bad? Could there be a problem with the battery and how can i check for it?

Your help would be really appreciated and thanks in advance!!
```

---
## \#2 Posted by: willpark16 Posted at: 2017-09-30T03:23:13.153Z Reads: 201

```
Post vesc settings
```

---
## \#3 Posted by: goldrabe Posted at: 2017-09-30T03:25:38.109Z Reads: 202

```
Thanks for replying to my post!
At the moment i have the hubs connected to a generic not programmable esc, so i can´t tell you the settings.
```

---
## \#4 Posted by: mmaner Posted at: 2017-09-30T03:30:28.598Z Reads: 198

```
It's unlikely it's the ESC, I'm running the same ESC on one of my boards and it's too fast for me.  The acceleration curve is crap and the brakes are unpredictable...but it is fast. 

I would guess you either have a battery issue or motor issues.  You. An test the battery by doing a full charge then measure the total voltage.  If it's 42v, you prolly don't have a battery issue. It's still possible, just unlikely. 

I would check the motors by replacing with outrunners on the bench, if you have spares.  I've not heard a lot of good things about Maytech hub motors, so they just not be very good. As the KV is so low that's a predictable top speed.
```

---
## \#5 Posted by: goldrabe Posted at: 2017-09-30T03:40:44.922Z Reads: 186

```
Thanks for your reply!
So, putting them on vescs will not affect top speed by much i guess.
Unfortunately no other motors to test the esc.
Would you recommend buying 110kv over 60kv then? How will this affect torque? Can i still go up hills with a 110kv motor?
```

---
## \#6 Posted by: mmaner Posted at: 2017-09-30T03:49:33.082Z Reads: 175

```
I really couldn't say, I've never run hubs before.  My understanding is that 90kv to 110kv is the sweet spot. Maybe ask @Hummie?
```

---
## \#7 Posted by: goldrabe Posted at: 2017-09-30T03:51:41.245Z Reads: 176

```
Thanks for your help and time really appreciate it!!
```

---
## \#8 Posted by: Namasaki Posted at: 2017-09-30T03:59:10.399Z Reads: 177

```
Can you post links for the hub motors and ESC's and battery so that we can look at the specs.
```

---
## \#9 Posted by: goldrabe Posted at: 2017-09-30T04:08:34.820Z Reads: 181

```
Thanks for your reply, here are the parts as bought.

The hubs:
http://www.diyeboard.com/hub-motor-9055mm-800w-60kv-for-diy-electric-skateboard-p-430.html

The ESC:
http://www.diyeboard.com/dual-bldc-motor-sine-wave-foc-esc-speed-controller-for-diyeboard-p-522.html

The battery:
http://www.diyeboard.com/10s5p-11ah-lg-battery-power-kit-with-bmschargerenclosure-p-572.html
```

---
## \#10 Posted by: Namasaki Posted at: 2017-09-30T04:34:19.441Z Reads: 173

```
about the motors, their specs contradict their performance claims:
24v-36v is only 6s - 8s
Max current 22a
Max output 800w
36v x 22a = 792w
36v x 60KV = 2160 rpm
according to my calculations, the board should go 22 mph with no rider.
The excessive heat might be because your using a 10s battery 42v when the motor is only rated for 36v max.



<img src="/uploads/db1493/original/3X/4/0/4017c95c950899c23f64a20afbaedf7affe1d837.png" width="547" height="500">
```

---
## \#11 Posted by: Namasaki Posted at: 2017-09-30T04:41:19.589Z Reads: 162

```
About the battery:

According to their specs, the maximum continuous discharge is only 15a
This limitation is likely because of the bms they use and not the cells.

<img src="/uploads/db1493/original/3X/8/0/803c6e0f008eb2ee0d36f402289644db565cea44.png" width="502" height="500">
```

---
## \#12 Posted by: goldrabe Posted at: 2017-09-30T04:44:31.382Z Reads: 148

```
Thank you for your time looking at the parts!
I thought 10S is 10 cells at 3.6V , so connected in series will give 36V.
Is 15a too low for a discharge rate?
```

---
## \#13 Posted by: Namasaki Posted at: 2017-09-30T04:56:20.328Z Reads: 149

```
3.6v per cell is the nominal voltage. 
3.8v is storgage voltage
4.2v is fully charged voltage.
I would not necessarily expect a beginner to know this, but I am little shocked at the way this website is describing their products. It looks like they don't have a clue about what they're selling.

15a battery current is probably not enough. thats only 7.5a per side.
```

---
## \#14 Posted by: Esk8HubsUS Posted at: 2017-09-30T05:00:24.846Z Reads: 146

```
We run these hubs (Maytech 90mm 800w) on our board (www.pulseboards.com) , paired with dual Maytech VESC and a 10s2p Samsung 25r 5.0ah pack , and it flies.  25+mph and serious hill climbing.   It sounds like the Diyeboard sinewave ESC could be your problem... check with Jason at DIYEboard maybe he can get you a replacement. That or swap out for VESC
```

---
## \#15 Posted by: goldrabe Posted at: 2017-09-30T05:23:14.224Z Reads: 146

```
Thanks for both of your replies,

@Namasaki now i get confused, all the Li/Ion 10S batteries i have looked at where rated as 36V. The Lifepo4 ones are rated higher right? But i think the DIYeboard sites product description are just copied and pasted from other Alibaba sites, they have all the same descriptions

@Esk8HubsUS  so you think VESC´s might solve my problem, or they sent me a wrong rated ESC like for 6s or 8s?
Could wrong wiring affect speed and range?
```

---
## \#16 Posted by: Namasaki Posted at: 2017-09-30T05:46:11.164Z Reads: 139

```
<img src="/uploads/db1493/original/3X/d/c/dcc4e3e90e2f073ca5779815c10bb71f33174d33.jpg" width="690" height="387">
```

---
## \#17 Posted by: Namasaki Posted at: 2017-09-30T06:08:25.895Z Reads: 136

```
Vescs are by far the best motor controller available but I don't think it's gonna help.
The motors are only rated for 22a and your battery is only rated for 15a.
If you do decide to get a couple vescs, dont get the Maytech vescs. Rumor on the street is that they are not reliable.
```

---
## \#18 Posted by: goldrabe Posted at: 2017-09-30T06:12:27.660Z Reads: 138

```
@Namasaki, Sorry, maybe i get you completely wrong, but my really basic understanding of batteries is like this:

The S’s:
 
A single LiPo cell has a nominal voltage of 3.6 volts. Since battery packs come in different sizes and voltages, it is more convenient to denote the voltages by saying 10S rather than 36 volts. To find out the nominal voltage of any pack, take the number before the S and multiply it by 3.6. This will render the voltage for the pack. So, a 13S pack will have a nominal voltage of 46.8 volts. 
A single LiFePO4 cell has a nominal voltage of 3.3 volts. Since battery come in all sizes, it is more convenient to denote the voltages by saying 12S rather than 36 volts. To find out the nominal voltage of any pack, take the number before the S and multiply it by 3.3. This will give you the voltage for the pack. So a 16S pack will have a nominal voltage of 52.8 volts.
This is taken from the site " Basic understanding of batteries"
In my conclusion that means i can use the motors with a 10s battery pack, but the description is horrible because it mentions even 12s packs and the description for the 90mm 110kv motors are the same.
So you mean i confuse the input volt of 36V is compatible with a 10s pack right? So if i want to use a 10s 36V pack the input voltage of the hubs should be 42V?
I don´t want to offend you, just try to understand what you are saying, i really appreciate your time!!
```

---
## \#19 Posted by: Namasaki Posted at: 2017-09-30T06:20:37.108Z Reads: 128

```
Look at the chart I posted. It shows various states of charge for Lithium ion and Lithium polymer batteries.
A 10s lithium battery is only 30% full at 36v and 100% full at 42v
```

---
## \#20 Posted by: boramiNYC Posted at: 2017-09-30T08:00:02.494Z Reads: 123

```
I would think 15A is for each cell. So only # of parallel would be multiplied. So for the whole pack it should be 75A max continuous.
```

---
## \#21 Posted by: pat.speed Posted at: 2017-09-30T08:41:53.352Z Reads: 112

```
Or maybe they are using very low c rated cells. I wouldn't expect 75amps from that pack. The seller is actually in here maybe he can help @diyeboard
```

---
## \#22 Posted by: pat.speed Posted at: 2017-09-30T08:43:43.225Z Reads: 112

```
The voltage of a lithium ion/ lithium polymer battery is 36v at its nominal charge, when it is fully charged the battery will be at 4.2v so 4.2 x 10 = 42v like @Namasaki said
```

---
## \#23 Posted by: goldrabe Posted at: 2017-09-30T12:26:23.625Z Reads: 116

```
Thanks for all replies!!

Yeah i get that a fully charged 10s pack should be 42V, but everyone refers to it as 10s 36V right? So for example motors meant for electric bicycles will be rated or described as 36V motors for a 10s pack or not? 
But my biggest hope is that if i would connect two VESC´s like Enertion Focbocx or another quality vesc, the communication between motor and energy source will get better, meaning that i will get faster speed, less heat and better range. 
My question is will the vescs help me achieving that or will there be just a marginal change?
Thanks!
```

---
## \#24 Posted by: pat.speed Posted at: 2017-09-30T12:32:43.841Z Reads: 110

```
They will not help you to gain speed it is that simple. The reason you aren't getting much speed is likely because you are only able to draw 7.5amps per motor which is not enough. Your best bet is most likely a battery that can output more amps. You should be getting around 35km/h or 22mph top speed
```

---
## \#25 Posted by: dickyho Posted at: 2017-09-30T12:39:07.204Z Reads: 112

```
I know this motor, I was want to sell on ebay before.  quality is ok, just very easy too got hot. 

As I remember, this one have 2 version, 24V version can go up to 25km/h,  36V version can go up to 35km/h.

and this one don't have max 800W, it shall be arround 500W.
```

---
## \#26 Posted by: goldrabe Posted at: 2017-09-30T12:39:51.375Z Reads: 108

```
Thanks for hanging in here with me!
 My top speed is only 25km/h, very disappointing, the Meepo gets with less powerful motors better speed and hill climb. If it´s the battery that means i have to change the bms? Why do i get only 12miles of range out of this battery?
I am really puzzled now hopefully there will be solution.
```

---
## \#27 Posted by: pat.speed Posted at: 2017-09-30T12:47:38.183Z Reads: 106

```
possibly voltage sag. Try asking the manufacturer what cells are used in the pack
```

---
## \#28 Posted by: dickyho Posted at: 2017-09-30T12:50:56.989Z Reads: 106

```
10S5P shall have above 30km range, unless you battery already damaged.

I did tried, for a 24V version of this hub motors, even use on a 36V battery, it still will not go faster.
```

---
## \#29 Posted by: goldrabe Posted at: 2017-09-30T13:32:09.345Z Reads: 104

```
Are your hubs really the same 60kv? Can you show me your wiring and all the other specs of your set up? You are giving me hope, hopefully i can get more out of my spend money.
```

---
## \#30 Posted by: Hummie Posted at: 2017-09-30T14:59:13.621Z Reads: 103

```
50 cells w only a 15 amp continuous discharge is weirdly low. Their descriptions are lacking. What cells are they and what bms.  

Lipo and li-ion have different voltage at different states of charge and li-ion can go lower

I don't know those MOTors or why they would get hot but going slowly and getting hot ..I'd think ud at least be free from one of those
```

---
## \#31 Posted by: JdogAwesome Posted at: 2017-09-30T15:16:42.454Z Reads: 100

```
Ok first off let me start by saying I think it's definitely a problem with that speed controller. I have two 60kv Maytech Hubs on my 6S 10Ah board with dual VESC and I have a top speed of 20mph and a range of 12-14 miles. I also have my max motor current set at 50A and the motors haven't even gotten above 40c. I think that with your 10S configuration you should be getting a lot more speed and range from your board so I think your ESC could possibly be setup wrong maybe for a belt drive motor and not a hub. Also if your battery can really only supply 15A continuous then that's really crappy though I think it could handle burst of like 30-40A when accelerating. Oh also my motor max is set at 50A **THOUGH** I do not live near any hills whatsoever l, if you do **DONT** set it that high you'll kill the motors or the VESC when going up a hill.
```

---
## \#32 Posted by: Namasaki Posted at: 2017-09-30T19:26:50.662Z Reads: 104

```
[quote="boramiNYC, post:20, topic:34345, full:true"]
I would think 15A is for each cell. So only # of parallel would be multiplied. So for the whole pack it should be 75A max continuous.
[/quote]

It could be that they where talking about individual cell discharge but they did not make that very clear.
Neither do they give any specs for the bms that they use and from their description of the battery it sounds like they are not bypassing the bms for discharge. 
And for all we know, they could have a 15a bms in there.
```

---
## \#33 Posted by: Namasaki Posted at: 2017-09-30T19:37:44.700Z Reads: 103

```
[quote="JdogAwesome, post:31, topic:34345"]
I also have my max motor current set at 50A and the motors haven't even gotten above 40c.
[/quote]


The specs for the motors he got says max current 22a
<img src="/uploads/db1493/original/3X/9/b/9b3211295b52fb265935b24c6895a40b3c312dad.png" width="566" height="397">
```

---
## \#34 Posted by: JdogAwesome Posted at: 2017-09-30T19:52:16.400Z Reads: 92

```
Yeah the max current for my hubs is also 22A but 50A is working fine. It also only draws that much current when accelerating and only for a couple of seconds, nominal current is about 15A. And the hubs he linked have the exact same specs as well as they look identical to my Maytech hubs.
```

---
## \#35 Posted by: boramiNYC Posted at: 2017-09-30T20:15:27.911Z Reads: 91

```
Yeah, it really could be 15A discharge which is pretty bad for a 10s5p pack..
```

---
## \#36 Posted by: boramiNYC Posted at: 2017-09-30T20:16:36.458Z Reads: 94

```
That's because the factory that supplies Maytech recently launched the retail website, which is DIYeboard.com.
```

---
## \#37 Posted by: Namasaki Posted at: 2017-09-30T20:18:18.798Z Reads: 90

```
If the bms is in fact the bottle neck, it could easily be corrected by modifying the battery wiring to bypass the bms for discharge.
And replacing the esc with a pair of Vescs but I would make one modification at a time and test it.

Then again, he is only getting 12 miles range from a 10s5p and that doesn't sound right.
Since the website doesn't give any info on the cells used in the battery, I'm wondering whats in there. 
Could even be counterfeit cells.
Chinese companies have been known to use counterfeit fake cells.
```

---
## \#38 Posted by: boramiNYC Posted at: 2017-09-30T20:24:56.372Z Reads: 90

```
On their site, OP's motors are recommended to be used with VESC.
```

---
## \#39 Posted by: evoheyax Posted at: 2017-09-30T21:19:49.696Z Reads: 92

```
I can say with a fair amount of cofidence that if you want hub motors that go faster than 15 mph and climb any sort of incline, you have three options: Hummies hubs, enertions hubs (which you must buy as a complete), or carvons. The rest are simply too small. You need a motor twice that size at a minimum. For me, I need 4x double sized hubs to not have issues. All of these hubs not coming from the community are garbage. Their tests are a joke, they put them on a rack and run them at no load speed for 8 hours. The problem with that is you are pulling very little amps, because theres no load. So of course they don';t over heat. Put a real world load on them and ride them hard for a few hours, thats a real test. These factories don't care about the quality, they just care about numbers.
```

---
## \#40 Posted by: boramiNYC Posted at: 2017-09-30T21:31:15.690Z Reads: 90

```
Not vouching for their quality but I've been using the hubs on Meepo for about 200 miles and it goes 22mph easy and climbs 20%. And I'm pushing it with 7-8 higher voltage than the original. Still heat is no problem after a long climb. Pulse Echo will be shipping soon and it uses Maytech/DIYeboard motor with 25mph.
```

---
## \#41 Posted by: Namasaki Posted at: 2017-09-30T21:39:41.324Z Reads: 99

```
[quote="boramiNYC, post:40, topic:34345, full:true"]
Not vouching for their quality but I've been using the hubs on Meepo for about 200 miles and it goes 22mph easy and climbs 20%. And I'm pushing it with 7-8 higher voltage than the original. Still heat is no problem after a long climb. Pulse Echo will be shipping soon and it uses Maytech/DIYeboard motor with 25mph.
[/quote]

Would you mind sharing one important factor, your body weight?

As for the Pulesboard, I did not see one video of it climbing any hill.
On their website where they claim it can climb 25% hills they just have a picture of it sitting in front of a small ramp that looks like about 5% maybe 10%

<img src="/uploads/db1493/original/3X/2/f/2f6be5abf70e865ff5292f39b6f2fc820c1e0857.png" width="690" height="473">
```

---
## \#42 Posted by: Esk8HubsUS Posted at: 2017-09-30T21:48:37.341Z Reads: 99

```
Here’s our testing on a 20% grade hill :  https://instagram.com/p/BZPpc7Fh3lm/   . I was able to climb 18-20% no issues when we were running the LG MF1’s in 10s2p , however we had a couple issues with voltage sag and the BMS topping out on full throttle up some hills so we decided recently on moving to the Samsung 25r’s and a better BMS
```

---
## \#43 Posted by: Esk8HubsUS Posted at: 2017-09-30T21:52:27.929Z Reads: 97

```
And btw , our board is fully modular (ebike connectors from ESC to motors) so we plan on making motor upgrades possible.  We’ll have esk8hubs as an upgrade and possibly also a belt drive setup 

<img src="/uploads/db1493/original/3X/b/3/b39e517bf57a4909b725e0cbb5ef683fa4ecd4a8.jpeg" width="666" height="500">
```

---
## \#44 Posted by: boramiNYC Posted at: 2017-09-30T22:03:04.152Z Reads: 94

```
I need to lose some but I'm pushing 170lb. BTW, one factory is making all these motors, Meepo, Pulse Echo, Maytech motors. I heard Meepo motor are pretty heat tolerant or should say resistance. At 22mph doesn't seem to tax at all heat wise. A very long half a mile 7-8% climb makes it hotter but not hot enough so you can't touch for 2 sec. That's my experience with it. I don't know anyone who runs these Meepo motors other than the cheap ESC, but it seems that ESC doesn't play well with the Maytech version, which OP has.
```

---
## \#45 Posted by: Namasaki Posted at: 2017-09-30T22:04:22.496Z Reads: 95

```
Your first claim was with the may tech hub motors. 
<img src="/uploads/db1493/original/3X/3/9/390c26495f579a4a4c118b209afde0a8285498dc.png" width="690" height="196">

Now your showing us a board with belt drive. 
And your claiming no voltage sag.
<img src="/uploads/db1493/original/3X/4/5/455c0f05221de745443a9755b8c59110eaaf6c79.png" width="313" height="165">
There is always some voltage sag even with the highest output batteries.
And Samsung 25r's are known for voltage sag that's whey the diy builders in this forum are have been switching to 30Q cells.
This is just another case of deceptive advertising.
```

---
## \#46 Posted by: boramiNYC Posted at: 2017-09-30T22:07:13.083Z Reads: 94

```
Good move, I think the OP's pack is also LG MF1 cells and partly he's experiencing voltage sag. OP's motor should be run by VESC like Pulse Echo it seem. 

A question, on Echo you are running the one piece dual VESC or two separate VESCs?
```

---
## \#47 Posted by: boramiNYC Posted at: 2017-09-30T22:10:03.074Z Reads: 93

```
No, I think Pulse has been very open about their evolution over at Reddit.
```

---
## \#48 Posted by: goldrabe Posted at: 2017-09-30T22:12:20.217Z Reads: 92

```
Thank's for your time again!!

The battery was labeled on the outside, together with the companys name i will take the board apart and see if i can get more information. The battery is originally made for e-scooters and so far i like the bms, i have brakes avaiable even at 100% charged. So if i could bypass the discharge there might be hope. But i really consider going for a refund and start from scratch again. I would have loved to get the Raptor, but it is outside of what i can afford. How much are the @Hummie Hubs when avaiable?
```

---
## \#49 Posted by: Namasaki Posted at: 2017-09-30T22:13:55.418Z Reads: 91

```
[quote="boramiNYC, post:47, topic:34345, full:true"]
No, I think Pulse has been very open about their evolution over at Reddit.
[/quote]

I say they are making impossible claims about their product.
Those of us who have been around a while building and testing various setups know this.
```

---
## \#50 Posted by: Esk8HubsUS Posted at: 2017-09-30T22:14:44.752Z Reads: 89

```
The belt setup isn’t  what we’re selling today.  The echo is selling with dual Maytech 800w’s .  I was just showing that we’re testing multiple motor options for future upgrades as were designing it to be modular for easy upgrades.  

The hill climb test on instagram was running the Samsung 25r’s and the Maytech 800 hubs (not the belt setup) 

We’re running dual Maytech VESC and working on an app that will allow you to run a quick motor detection when changing motors (that or have a predefined motor configs that we can push on demand via the app)
```

---
## \#51 Posted by: Namasaki Posted at: 2017-09-30T22:21:12.302Z Reads: 83

```
I'm guessing the test rider in your Instagram video weighs about 120 lbs
And you should not claim "no sag" because that is impossible especially with 25r's
```

---
## \#52 Posted by: boramiNYC Posted at: 2017-09-30T22:21:29.237Z Reads: 81

```
Nice. Dual VESC. I was always curious about that one. So little information on those with successful implementation.
```

---
## \#53 Posted by: evoheyax Posted at: 2017-09-30T22:24:46.562Z Reads: 84

```
Everything comes down to rider style and weight. If you like to ride slow most of the time, weight 120 lb, and go fast every once in a while, hubs like that wlill be fine. But the stator is tinny. They are not tested to my standards. 20% hills for a 2 miles, is what needs to be done. Tell me how hot you are, and I bet you'll blow you board up in the first mile. Get good components, speed 2-3k, and build your self a board that will do what we all expect from our electric skateboards, which is to just work, and work well.
```

---
## \#54 Posted by: Esk8HubsUS Posted at: 2017-09-30T22:28:01.553Z Reads: 86

```
Haha yeah 150 , however I’ve done 20% grade myself running the LG’s and I’m 200Lbs and no issues at mid throttle (full throttle was topping out the BMS max amperage output , hence why we moved to the 25r’s plus better BMS ) .. I agree , technically we shouldn’t say “no voltage sag” ,  maybe we’ll re-word  that one .
```

---
## \#55 Posted by: Namasaki Posted at: 2017-09-30T22:50:43.146Z Reads: 89

```
I think you should stick with belt drive and forget about hub motors.
Cheap hub motors like those from Maytech are known to be unreliable.
The issues associated with those types of motors like high current draw and overheating, urethane getting loose and comping off.
When your making boards to sell and warranty, you need dependability.
That is my friendly advice to you.
```

---
## \#56 Posted by: Hummie Posted at: 2017-10-01T06:51:05.634Z Reads: 90

```
wound motors for 11 hours today, never left the house.   getting better at it     i don't have a price or time when they will be done sorry
```

---
## \#57 Posted by: goldrabe Posted at: 2017-10-01T14:20:02.212Z Reads: 88

```
The time you have a price and are willing to sell your motors please let me know it, here in Japan electric vehicles are prohibited, having a nearly stealth motor like the hub motors is a big advantage!
Thanks for your time and dedication anyways!
```

---
## \#58 Posted by: composites_r_awesome Posted at: 2018-07-11T16:07:02.081Z Reads: 45

```
Hi, How are the Maytechs been so far?

> in Japan electric vehicles are prohibited

I so hoped modern urban areas in Japan would be heavens for esk8ers :hushed:
```

---
## \#59 Posted by: goldrabe Posted at: 2018-07-12T04:42:46.912Z Reads: 41

```
I did not had a good experience with them. Urethane is not good and chips easily, they develop a lot of heat. First I had them running with the ebay esc which was not a good match. Then I tried them with VESC'S and more amps, with the VESC'S they are more torquey and can drag me uphill but they get really battery hungry then. Another side effect was even more heat and that slowed the ride down after maybe 5-7 km. At the moment there is no good option for Hub motors, maybe that might change with @Hummie Hubs. If I had the money i would go for the Carvon torque drives which are similar specked to the Maytech's. But i have really hope in @torqueboards direct drives, which will hopefully come at an affordable price.
```

---
