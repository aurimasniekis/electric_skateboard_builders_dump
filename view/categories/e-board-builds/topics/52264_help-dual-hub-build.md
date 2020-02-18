# HELP! dual hub build

### Replies: 35 Views: 1327

## \#1 Posted by: admiralackbar Posted at: 2018-04-14T19:47:35.781Z Reads: 135

```
I have these hub motors... 36volt 1000 watt

https://www.aliexpress.com/item/100W-36V-electric-scooter-motor-electric-skateboard-conversion-kit-electric-scooter-motor-kit/1000003336521.html?spm=2114.10010108.1000013.4.6d9e4a6bLDPY4B&traffic_analysisId=recommend_2088_2_90158_iswistore&scm=1007.13339.90158.0&pvid=eadad467-68a3-486d-8bb8-cc50a3e70f90&tpp=1

![HTB1wvSzNVXXXXaEaXXXq6xXFXXXr|690x387](upload://7FixV5XK3sjY1FVZh3Ne574uca9.jpg)

I am looking to build a diy board from these and have NO IDEA what ESC or BATTERY TO GET... i am not sure what is compatible... its very hard to figure out and looking for a point in the right direction... or a simple answer of just what to buy... JUST IN TERMS OF COMPATIBILITY... range can be ANYTHING... but note the deck will be very long and can fit a larger battery... I have no idea if size of battery even corresponds with range or speed at this point... 


battery MUST be able to plug directly into wall with AC adapter cable... no balance chargers allowed

thanks
```

---
## \#2 Posted by: linsus Posted at: 2018-04-14T20:13:21.239Z Reads: 119

```
[quote="admiralackbar, post:1, topic:52264"]
battery MUST be able to plug directly into wall with AC adapter cable… no balance chargers allowed
[/quote]

*reaches into magic hat and pulls out ready made battery and charger suited for e-skate*

Think you have some reading to do. Dont get me wrong, you can get what you ask for. But may I ask what your budget is for said battery and esc?
```

---
## \#3 Posted by: ZackoryCramer Posted at: 2018-04-14T20:20:09.799Z Reads: 112

```
[quote="admiralackbar, post:1, topic:52264"]
NO IDEA what ESC
[/quote]

When in doubt, FocBox or Vesc 6.
```

---
## \#4 Posted by: SeanHacker Posted at: 2018-04-14T20:23:45.908Z Reads: 104

```
Stick to butt boarding dude. ;)
```

---
## \#5 Posted by: SeanHacker Posted at: 2018-04-14T20:23:58.113Z Reads: 101

```
ESC-
http://www.electric-skateboard.builders/t/hw6-4-based-esc-escape/37579

BATTERY (If you're US based)-
http://chibatterysystems.com
```

---
## \#6 Posted by: admiralackbar Posted at: 2018-04-14T20:25:10.263Z Reads: 96

```
no budget... just need compatibility... or options of what is compatible and the pros and cons... 

also... what is the minimum diameter of the hub motor that would be acceptable... AS IN JUST THE HUB MOTOR NOT INCLUDING THE PU WHEEL
```

---
## \#7 Posted by: admiralackbar Posted at: 2018-04-14T20:28:39.557Z Reads: 91

```
TBH i have done much research but havent gotten a clear answer... like the two hub motors specs read 36v and 1000watts.... what kind of battery is suitable for this???
```

---
## \#8 Posted by: admiralackbar Posted at: 2018-04-14T20:31:43.427Z Reads: 89

```
will these esc's work for the specs of the motors?

i am not really looking to program a VESC so will FOCBOX be better?
```

---
## \#9 Posted by: Exiledd_Top Posted at: 2018-04-14T20:32:57.482Z Reads: 87

```
[quote="admiralackbar, post:7, topic:52264"]
36v
[/quote]

Exactly what it says 36v as in 10s, the motors are good for 10s
```

---
## \#10 Posted by: admiralackbar Posted at: 2018-04-14T20:41:46.899Z Reads: 85

```
[quote="Exiledd_Top, post:9, topic:52264"]
the motors are good for 10s
[/quote]

even though its a dual hub system... does that just mean it draws twice the amps?

the P number isnt just a difference in how the batteries are linked together though? it literally implied a bigger battery... a similar sized batter with a higher P number would mean a smaller S number? 

i ask because i have been hearing that anything below 1P is bad news for some reason? and 2 P is better... any thoughts on this?
```

---
## \#11 Posted by: Exiledd_Top Posted at: 2018-04-14T20:46:48.700Z Reads: 83

```
10s means 10 cells now the "P" means how many in parallel so a 10s2p means 10cells and 2 pack so in total its 20 cells total. Now the reason u want to stack them in parallel is for one u get more range and 2 u pull more amps , also depending on the motor watts u go fast, u also want to have more amps so that u don't voltage sag as much is u have a 10s1p depending on your cells let's say 30q u can only pull 20amps and your going to have a lot of voltage sag typical motors single drives can pull 60amps (not really good at explaining the technicality sorry )
```

---
## \#12 Posted by: linsus Posted at: 2018-04-14T20:49:38.820Z Reads: 81

```
Not sure where you did this "much research" but sounds like you just went out and bought some motors and are now just assuming things will work out :p always plan a build. Especially if you're unfamiliar with what you're doing.

And sorry if i sound like a douche, thats not my intent
```

---
## \#13 Posted by: admiralackbar Posted at: 2018-04-14T20:51:46.498Z Reads: 76

```
Ok.. i didnt buy the motors exactly... but these motors are the only ones that will fit my trucks... ALSO PLEASE NO ALTERNATIVE MECHANICAL SUGGESTIONS... THAT COULD BE A SEPERATE BUILD... I MUST USE THIS MOUNTING STYLE FOR REASONS.... didnt even want to make it a mechanical / truck mold thread...
```

---
## \#14 Posted by: SeanHacker Posted at: 2018-04-14T20:53:09.465Z Reads: 79

```
FOCBoxes are vescs. You'll need to program either of them. 

36v means you can use a 10S like any of the 10S batteries here for example http://chibatterysystems.com/shop/10s2p-37v-5ah-samsung-25r-e-board-pack-9wsfb

P.S- Wear a f$cking helmet dude. You're going to need it. ;)
```

---
## \#15 Posted by: admiralackbar Posted at: 2018-04-14T21:11:34.995Z Reads: 74

```
what is the advantage of 36 volt motors over 24 volt

what would be the range i would get from these 2 motors... with 10s2p

are FOCBOX or VESCs basically compatible with ANY spec motor... or are theres different ones for different specs
```

---
## \#16 Posted by: pennyboard Posted at: 2018-04-14T21:24:05.246Z Reads: 72

```
You're not the first person to ask these questions. All these answers can be found by SEARCHING and READING. Serisiously. Devote like an hour or two to solid reading of posts on here and you'll have your answers
```

---
## \#17 Posted by: Acidfie Posted at: 2018-04-14T21:28:19.730Z Reads: 72

```
the VESC will power every sychronous motor.

[quote="admiralackbar, post:15, topic:52264"]
what would be the range i would get from these 2 motors… with 10s2p
[/quote]

depends on your used cells, ride style, weight, motors but about 10km

[quote="admiralackbar, post:15, topic:52264"]
what is the advantage of 36 volt motors over 24 volt
[/quote]
 more voltage = efficient usage of current

24V * 10A = 240W
36V * 10A = 360W
```

---
## \#18 Posted by: pat.speed Posted at: 2018-04-14T21:40:05.535Z Reads: 66

```
That range calculation would be correct if he was using 20wh/km but I doubt it. It’s usually around 10Wh/km so he will get somewhere around 20km
```

---
## \#19 Posted by: Acidfie Posted at: 2018-04-14T21:45:39.217Z Reads: 62

```
i am using 10S3P and getting about 12-15km.. so..
```

---
## \#20 Posted by: admiralackbar Posted at: 2018-04-14T21:59:21.414Z Reads: 60

```
is there a special trick to hooking up 2 esc's to the battery pack? 

what would be the draw for these two 36 volt batteries from the battery... if theyre 1000watts each... 

are batteries with integrated BMS systems for wall charging readily sold?
```

---
## \#21 Posted by: pat.speed Posted at: 2018-04-14T22:04:57.909Z Reads: 48

```
Yes they are readily sold, somebody already linked you to a website to buy from a forum member
```

---
## \#22 Posted by: ATLesk8 Posted at: 2018-04-14T22:06:23.437Z Reads: 52

```
Dude this is at least the second thread you've started like this..."solve my problem using these shitty components and nothing else, also I know better so no suggestions!" 

Use the search function
```

---
## \#23 Posted by: admiralackbar Posted at: 2018-04-14T22:19:01.369Z Reads: 55

```
its not that im not open to sugestions.. i just cant deal with people telling me to "just buy a meepo"... also one of those threads got zero responses and the other was for single hub build which i took the advice not to do
```

---
## \#24 Posted by: pat.speed Posted at: 2018-04-14T22:27:46.264Z Reads: 56

```
I just looked at the item you want to buy and it’s only 100w not 1000w. 100w will barely get you moving. 

If your budget is very low and you want to use hubs I would suggest to get on the @PredatorBoards group buy for ownboard parts. That includes the hubs, esc and remote I think. 

Then get a decent 10s battery. Either a 10s2p from a forum member like the one linked, a 10s2p lipo setup with bms or if you really have to a meepo style 10s2p battery
```

---
## \#25 Posted by: KTMinni Posted at: 2018-04-14T22:34:12.501Z Reads: 59

```
[quote="ZackoryCramer, post:3, topic:52264"]
Vesc 6
[/quote]

Lol like anyone can afford it
```

---
## \#26 Posted by: KTMinni Posted at: 2018-04-14T23:02:27.426Z Reads: 53

```
@pennyboard is right, you can find all of these answers by searching but just to get you started I'll tell you, no there aren't different versions of the VESC, same tech just varying levels of quality (FOCBOXES seem to be the highest quality iteration)
```

---
## \#27 Posted by: linsus Posted at: 2018-04-15T11:49:52.943Z Reads: 50

```
[quote="KTMinni, post:26, topic:52264"]
no there aren’t different versions of the VESC
[/quote]

well thats just not true. There are different verisions of the vesc i have Three different ones on my desk as i type this, 4.10, 4.12 and 6. Then again i dont know what you imply by saying "same tech". 
I'm not even going to start on the FOCbox part.
```

---
## \#28 Posted by: KTMinni Posted at: 2018-04-15T14:05:38.173Z Reads: 44

```
Yes you are right in the sense there has been different versions. But there are many  _iterations_  of the 4.12(the most recent VESC before vedder teamed up with trampa), and those include basically all of the new VESCs you can buy right now including the focbox, and TB VESC.
```

---
## \#29 Posted by: admiralackbar Posted at: 2018-04-15T14:18:53.186Z Reads: 42

```
so the same vesc that will work with a 24v 200w motor...

will also work with a 36v 1000w volt motor... 

it just depends how you program it?

what about an ESC... those must be pre-spec-ed if you will? im looking at the maytech super esc or the new maytech dual esc...  because the cables are thick and theyre just overall less sketchy...

it seems like maytech only sells one version so same question... does it work the same with a 24v motor as it would with a 36 volt motor.. or do i have to buy a specific version of the ESC... not really talking about iterations of quality
```

---
## \#30 Posted by: linsus Posted at: 2018-04-15T14:48:41.771Z Reads: 37

```
The vesc has motor detection to suit the motor you use it for. Again, read up on the VESC. Its all written Before.

My impression is that Maytech is know around here as one of the lesser brandnames. Alot of failures it seems.

Personally never used any of thier products
```

---
## \#31 Posted by: admiralackbar Posted at: 2018-04-15T14:59:46.037Z Reads: 37

```
yes but theyre more readily available than R-SPEC... and seem decent
```

---
## \#32 Posted by: admiralackbar Posted at: 2018-04-15T15:03:09.459Z Reads: 39

```
im wondering if anyone has any experience getting truck hanger molds made... i would like to make an R-SPEC style truck but one that is about 330mm wide axle width and one that is extremely narrow where the wheels are almost touching the king pin...  gotta have that square piece that locks into the stator... 

Basically im wondering if theres any 3d models floating around... or if people know of the cheapest way to get it done... it seems liek the cheapest i could find is about 800 to get the mold made...
```

---
## \#33 Posted by: Hummie Posted at: 2018-04-15T15:09:37.978Z Reads: 43

```
Lost wax mold maybe. Cheap n easy.  Lost pla maybe
```

---
## \#34 Posted by: Deckoz Posted at: 2018-04-15T15:13:24.189Z Reads: 45

```
[quote="SeanHacker, post:4, topic:52264"]
butt boarding
[/quote]

You should try it... It's actually pretty fun lol...
```

---
## \#35 Posted by: admiralackbar Posted at: 2018-04-15T16:20:01.828Z Reads: 42

```
im seeing these batteries for sale... 

https://wholesaler.alibaba.com/product-detail/Chinese-brand-cell-10s2p-18650-i_60750160852.html?spm=a2700.7782932.1998700997.8.25d21e7a335ZfY

are there any downsides to going with these?

im seeing others for about $80... 

trying to keep the entire build under $500... but also i have an investor/partner skateboard builder who wants to mass produce them... so im sure the price could go down... just trying to figure out a good design... from standard parts... 

we will probably figure something out for the electronics casing.... 

once again... if hummies or R-spec were readily available.. i would totally use them but theyre not...  and i dont know the first thing about designing my own hub motor... If anyone has any solidworks or inventor files theyd like to send me i wont stop you
```

---
