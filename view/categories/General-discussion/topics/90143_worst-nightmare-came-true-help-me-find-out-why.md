# Worst nightmare came true. Help me find out why…

### Replies: 48 Views: 1476

## \#1 Posted by: davidbonde Posted at: 2019-04-11T13:04:18.806Z Reads: 478

```
My biggest fear when going around on an eskate are a sudden electronic failure or something similarly, throwing me of the board out of the blue. That happen tp me today and I can’t figure out what the hell happened. 

I was doing my speed runs I just launched for the one where I really would give it all. Slightly downhill and the wind in my back. But I didn’t get very far before the board threw me off. It kinda felt like that the board just stopped / blocked or something. Luckily it was in the beginning of my acceleration so I was not going very fast (20 mph), but it was enough speed to launch me forward. Reflectively I took a long step and landed first on one foot and then down on my stomach and hands sliding. I sled long enough to think “hey now I am sliding. Wonder how my shirt will hold up. Kinda nice feeling sliding when I think of it :) I was wearing knee pads, hillbilly crash pants, kvelar shirt, elbow pads, and slide gloves. So I am fine and nothing seriously happened.  

The thing is that after the board worked fine. No sign of things that were wrong. I only took the board to 17 mph on my way back. But no issues. 

I had the metr app running when I crashed and the only thing that stands out are the motor current that did go all the way to 118 two sec before the crash (I did start the acceleration from standing and slightly up hill). That might be the reason. But would that block the motors and then afterwards work fine again? When I look that other vesc data I have I see that the 118 motor amps are the highest I have seen yet. Normally its around 80a when It’s the most. I haven’t been close to 118 before. 

Anyone have any suggestions on what might have happened. I know you don’t have much info to guess from. But Anyway. 

This is the metr data: https://metr.at/r/LEFou
```

---
## \#2 Posted by: chaka Posted at: 2019-04-11T13:24:18.112Z Reads: 448

```
Motor amp spike caused your motor controller to shut down. The sudden loss in accelleration feels like the board is braking but it is not.  What is your motor max set at and gear ratio/top speed?  The taller the gear ratio the more susceptible the system becomes to current spikes when pushing the throttle.
```

---
## \#3 Posted by: davidbonde Posted at: 2019-04-11T13:57:01.176Z Reads: 436

```
If the Vesc short down wouldn't we see that the Voltage would drop very low in the metr data? It only drops to 35V. Or would the short down be so short that it wouldn't be caught in the data? 
I have tried to short the board down while giving full throttle and the V drops tp 9V And sometimes, but not every time, the metr app gives a warning saying "Under Voltage". That didn't happen with my crash. 

My motor max is set at 80a and my gear ratio are 16/40 and I hit 37 mph as max speed.

Crash data:
![image|281x500](upload://eOv3UBsIFpofLrrwjVPgBXPMuoe.png) 

Under Voltage Warning when testing shirtinget of the board. But that warning only came once, and I turn off the board multible times:
![image|281x500](upload://4IcNODKrYJCf2Sz4bbBhLZ6RL44.png)
```

---
## \#4 Posted by: davidbonde Posted at: 2019-04-11T14:07:20.703Z Reads: 355

```
I am really surprised about that spike in motor amps. I haven't seen that before. Normally I am around 80 when it is highest. And I didn't feel I was accelerating that hard. Strange.
```

---
## \#5 Posted by: BooYA Posted at: 2019-04-11T14:21:44.328Z Reads: 350

```
Sounds like motor desync due to hard throttle input that can't be followed and then resulting in cogging at high speed felt like locked motor. 
Huge amp spikes also indicate that your esc had a super hard time driving the motor and/or the current ripple from the desync overflow the current management loop
Do a better detection and try again 
Also hardware side is extremely important, make crazy strong soldering job and ensure electricity can flow with no bottleneck. Use ton of tin, big cables, and be sure vibrations can't loosen connection
```

---
## \#6 Posted by: davidbonde Posted at: 2019-04-11T14:26:21.597Z Reads: 337

```
Would you do the detection with or without wheels on?
```

---
## \#7 Posted by: chaka Posted at: 2019-04-11T14:30:56.954Z Reads: 328

```
The vesc has a hard cutoff at 120 amps and in your app data you hit a peak of 120.7 amps. This only cuts throttle and does not shut the whole system down. It looks like your board is set up with a top speed just under 40 mph, this is high enough to start triggering these spikes when throttling hard at 50% duty cycle.

If you lower your max motor amps down to 50 or 60 amps it will give the soft cut off more time to engage and prevent the hard cutoff.

Motor detection should be with the motor free to spin, no belt or gears should be attached.
```

---
## \#8 Posted by: rsalmon Posted at: 2019-04-11T14:36:30.257Z Reads: 299

```
What kind of VESC are you using, if you don't mind me asking?
```

---
## \#9 Posted by: davidbonde Posted at: 2019-04-11T14:37:52.525Z Reads: 295

```
Ahh that makes sense... Thanks Chaka. 

Would lowering the motor amps make the the top speed less? 

It sunds like I need to upgrade my setup to handle more strain if I want keep doing these speed runs.  What would you suggest I look at?
```

---
## \#10 Posted by: davidbonde Posted at: 2019-04-11T14:38:22.066Z Reads: 285

```
I don't mind... two focboxes.
```

---
## \#11 Posted by: chaka Posted at: 2019-04-11T14:42:30.990Z Reads: 285

```
It will not lower the top speed but it will lower the torque you feel during acceleration. Looking again at your app data and it looks like your motors are being driven very hard, you can see the temp rise when the board stopped moving. They could have picked up some resistance from heavy use so It might be worth while to recalibrate to help prevent another hard cut-off.
```

---
## \#12 Posted by: chaka Posted at: 2019-04-11T14:52:29.482Z Reads: 284

```
I think it is time for all of us to move on to a more robust MOSFET like the to-247 package in order to get the power we need from a dual motor setup.
```

---
## \#13 Posted by: davidbonde Posted at: 2019-04-11T15:00:01.987Z Reads: 278

```
"recalibrate" now we are entering unknown territory for me. 

You are right. I properly drive my motors to hard. they are 6365 200kv. I run pneumatics 150mm.  

I did adjust the belts a little before this run. Made them a little tighter. And one motor are saying a noise. But thats not in the motor when there is belt on. I think its from a loose motor pulley, where the scrub screw is funck and cant be tighten anymore. So the bully sit loose and makes a noise. 

But I will check everything again. 

What would be a reasonable temp to have. When I see other data I have the temp hit 60 degrees C.
```

---
## \#14 Posted by: chaka Posted at: 2019-04-11T15:04:06.109Z Reads: 255

```
When a say recalibrate I mean run motor detection again. 😉

I also recommend taking a mental note on how much torque you were feeling when the cutout happened. You most likely hit the maximum power you can pull out of a vesc based on v4.12
```

---
## \#15 Posted by: davidbonde Posted at: 2019-04-11T15:53:31.884Z Reads: 243

```
Thanks Jeramiah. You helped me find a plausible reason why this happened. That takes away the unknown. I was afraid of the unknown. Now I feel ok comfortable hitting the speed track again tomorrow.
```

---
## \#16 Posted by: deucesdown Posted at: 2019-04-11T17:39:32.663Z Reads: 230

```
Photos of the shirt plz!
```

---
## \#17 Posted by: Pedrodemio Posted at: 2019-04-11T18:21:54.897Z Reads: 224

```
Could also be that the motor saturated and the observer lost track of it

You could a bit with saturation compensation, but only way to test would be induce the problem again, not sure if you are up to it
```

---
## \#18 Posted by: Arzamenable Posted at: 2019-04-11T18:36:20.155Z Reads: 226

```
Looks like the experts are finishing up this case 👍. I recently had a scary fall. I was not so composed in the aftermath. I put the remote in a vice and crushed it. 

I think I’m going to add Metr Pro to my essential  riding gear right after helmet... and pants . Heal up bro 🤙
```

---
## \#19 Posted by: myreala Posted at: 2019-04-11T19:13:18.383Z Reads: 219

```
So I had the exact same fall and I figured out the reason eventually by doing a bench test. Accelerate the board by pulling the full throttle on a bench, does one of the motors stall? 
In my case the motor was stalling only when accelerating too quickly. The reason was bad motor detection. That fall fucked me up real good.
To avoid this do a bench test every time you do any changes to the drive train. If there is cogging, time to re do the motor detection.
```

---
## \#20 Posted by: davidbonde Posted at: 2019-04-11T19:41:28.954Z Reads: 208

```
I did a lot of bench throttling afterwards including full throttle for 5 min. Nothing really happened. Everything seemed fine. I will try again.
```

---
## \#21 Posted by: myreala Posted at: 2019-04-11T19:44:52.511Z Reads: 197

```
Look for cogging while accelerating quickly.
```

---
## \#22 Posted by: davidbonde Posted at: 2019-04-11T19:53:46.983Z Reads: 200

```
Weirdly nothing happened to the shirt but at the end of the sleeve. Think I might have taken most on the pressure with my gloves. One hand did get caught between my chest and the road which ripped the side of the glove. And just now I see that the jaw part of my helmet took a hit as well. The only thing I feel now is the heel on the foot that took the first impact (can’t stand on it. Need to be on my toes). And on the dorsal side of the hand that got caught. 

![image|375x500](upload://wnkMpAb3zah7aUcugfNiFTYdplY.jpeg) ![image|375x500](upload://ipMmju44sn9btkO4o0LpsGFry0U.jpeg) ![image|375x500](upload://iveoiGATzrlAFN4yriA2AO1eWiu.jpeg) ![image|666x500](upload://1OH9Y72zYybIBDA4iOfzFbsxe6K.jpeg)
```

---
## \#23 Posted by: deucesdown Posted at: 2019-04-11T19:58:21.317Z Reads: 191

```
Nice and clean!

Do you lean forward when grabbing the throttle? I'm always afraid of this, so rather than lean forward, I bend my knees and sit down. Gives me a fighting chance at staying on if throttle cuts. Not sure if I can stay on if it cogs though.
```

---
## \#24 Posted by: davidbonde Posted at: 2019-04-11T20:10:23.345Z Reads: 189

```
Yeah.. I do lean forward. I lean forward all the time mostly when going fast. Practicing the tuck. But I have the feeling that when something happens as it did to day I have no chance saving the fall. 
I think this is the significant main different between going fast on a eboard and going fast down hill on a gravity driving board. We have have the possibility of a electronic failure coming out of the blue giving us no time to react and work with the crash. In DH they often can anticipate the crash, giving them options to control the crash better.
```

---
## \#25 Posted by: Chase Posted at: 2019-04-11T22:18:41.736Z Reads: 176

```
I’m having similar problems with my 4wd. I’m pretty sure all 4 motors go out together when I accelerate hard from still and it’s on a 4way split ppm with 4 separate foc boxes. It would be odd if all four motors had a bad detection. I was under the impression it had something to do with the enertion nano remote since all four died together. I’m not getting any errors in the app. I know it’s hard to give input without me showing any settings
```

---
## \#26 Posted by: Mobutusan Posted at: 2019-04-12T01:22:48.223Z Reads: 173

```
Open up your Nano-x and have a look at the battery. I had two that I never fully got around to using, so they were brand new, although had been sitting in a box for a while. One would not hold a charge, and the other would, but seemed to need a charge everytime I picked it up. Opened them both up and found this. Those suckers were ready to pop, and didn't even have a ride on them. Interestingly, I got these during Enertions notorious 2017 Black Friday deal along with some "in stock" FOCBOX's that showed up around Feb, 2018. So, according to the date on the batteries, they were almost 1 year old before I got them brand new, and neither seemed to hold a charge very well even then. 
![20190201_155329|690x335](upload://vl5K9BfNkGmvj3kL0V7vq6Frl54.jpeg)
![20190131_220407|690x335](upload://M6qnwLhcN8YmHlnBaHlxw9CRkV.jpeg)
```

---
## \#27 Posted by: b264 Posted at: 2019-04-12T01:31:46.334Z Reads: 165

```
@davidbonde What firmware version are you using?
```

---
## \#28 Posted by: louwii Posted at: 2019-04-12T01:37:22.081Z Reads: 168

```
Oh look! They put balloons in the remotes to make them lighter!
```

---
## \#29 Posted by: Chase Posted at: 2019-04-12T01:39:59.897Z Reads: 168

```
I guess 2.18. I’m using the bdlc tool. Probably should switch over to ackmaniac.

Opened up the remote and luckily did not have the same issue with the battery.
```

---
## \#30 Posted by: ervinelin Posted at: 2019-04-12T03:22:02.398Z Reads: 160

```
Hope you find the root cause of your problems. I do think however that full throttling on the bench is hardly a comparable test to full throttling on the road. You won't be able to ramp up enough amps to trigger the supposed fault.

Glad to know you were well protected... out of curiosity, what Kevlar shirt (or is it a t-shirt) is that?
```

---
## \#31 Posted by: Sender Posted at: 2019-04-12T12:32:08.148Z Reads: 152

```
@chaka thanks for the investigative journalism!  I always love to learn a bit more about why cutouts happen and what can be done to mitigate these instances.
```

---
## \#32 Posted by: chaka Posted at: 2019-04-12T13:23:16.976Z Reads: 150

```
A bench top dyno is on the to do list. Nothing fancy just a couple of drums heavy enough to draw a lot of power while spooling them up. Testing a board that tops out at 40+mph on the road is not that big of a deal but my last build doesn't hit its power band till roughly 30 mph and has a therotical top speed of 66mph.
```

---
## \#33 Posted by: davidbonde Posted at: 2019-04-13T20:20:53.985Z Reads: 141

```
[quote="b264, post:27, topic:90143, full:true"]
@davidbonde What firmware version are you using?
[/quote]
3.40. Now updated to 3.54 as I ran a new motor detection today. What your thoughts @b264? 

[quote="ervinelin, post:30, topic:90143"]
You won’t be able to ramp up enough amps to trigger the supposed fault.

Glad to know you were well protected… out of curiosity, what Kevlar shirt (or is it a t-shirt) is that?
[/quote]

Think you are right. I need the protection. I am to afraid of crashes not to wear them. Seriously considering some leathers. I wore this kvelar sweat shirt: https://www.xlmoto.dk/troje-xlmoto-fuld-aramid-sortsolv#?p Just saw that they also have it without the reflex writing now. Would have chosen that if they had it back when I ordered.
```

---
## \#34 Posted by: davidbonde Posted at: 2019-04-16T13:03:57.408Z Reads: 124

```
I am back doing my speed runs. If I kick push to start and don’t hit the throttle to hard, I am not close to the 120 motor amps spikes. 

To be hornets... When I look at my VESC data I don’t really know if they are normal or at values where I should be concerned. Especially I am thinking of the motor amps and temp. Is it normal that they are this high? If someone with more knowledge about this than me have time to take a look I would appreciate it. I want to understand better. 

It seems that my setup max out at 37 mph. I can’t seem to get it going faster. 

I run 10s - 6365 200kv - 16/42 - 150mm pneumatics - focboxes

Vesc data:



[https://metr.at/r/UaZY4](https://metr.at/r/UaZY4)
```

---
## \#37 Posted by: sebaszz Posted at: 2019-04-16T14:49:47.210Z Reads: 109

```
Ì can fully agree on this. My first build with no experience brought me around town for 2 years/ 2000km without a single hickup or issue. Only wearing a helmet. 

6 month ago after building my 2nd board 2nd ride it tossed me off quite hard on the asphalt during acceleration wearing thin clothes, just came out of the gym. BMS cutoff on cell voltage because of unbalance almost full discharged pack.

1 week ago rebuilt my 2nd board, it tossed me off again. Wearing motor jeans en hoodie with kevlar lining? builtin protectors wirst guards. It protected me actually quite good besides the road rash on the hip above my pants. (MBS crashpants laying in the closet....). This time mosfet of the antispark burnt probably due to insufficient cooling/issue cooling block.

I'm now looking for even more and better protective gear inspired by @Deckoz. I really appreciate your effort trying to convince people to wear proper safety gear. Somehow it is still little bit ignored.
Wearing proper protective gear is essential part of our hobby.
```

---
## \#39 Posted by: davidbonde Posted at: 2019-04-17T06:03:59.617Z Reads: 103

```
@Deckoz Have you ever considered a leather suit. And what are your thoughts pro / con?
```

---
## \#40 Posted by: klaus79856 Posted at: 2019-04-17T08:32:03.530Z Reads: 102

```
I use my 25+ year old leather pants from a motorcycle suit.
Very good padding all aroud and as they have already some "scratches" I don´t care if there will be a few more.
```

---
## \#41 Posted by: Andy87 Posted at: 2019-04-17T10:20:50.745Z Reads: 98

```
I´m totally with you in gearing up to the max. As I come from the MTB part of esk8, falling is just a part of it. To achieve falling as save as possible is never bad. Save you more time on the board in future.

But I also think that maintenance of our boards is pretty much underrated. 

[quote="sebaszz, post:37, topic:90143"]
BMS cutoff on cell voltage because of unbalance almost full discharged pack
[/quote]
That´s just one of the things that can happen. 
Lose motor mounts, idlers, scratched cables, water in the enclosure and what not ever. Once the enclosure is mounted it´s good and closed for ever for some of us. I think as min a weekly inspection should be part of a save ride. Just open up the enclosure, check the voltage of your packs, check if all cables still in place and connected, check motor mounts and screws. That's a 15min job for the most people and can prevent a lot of troubles later.

Or maybe get a smart bms which give you to monitor the individual pack voltage. Stay up to date with things who went wrong at other peoples builds and think about it and if that could happen with your build as well. One of the reasons why I for example never used my push to start switches was that just too much of this anti spark switches burned up and that was not worth the risk for me.
```

---
## \#43 Posted by: banjaxxed Posted at: 2019-04-20T21:14:15.626Z Reads: 74

```
I’m looking at these crash pants, I value what’s left of my svelte lines 😜

Anyone tried them?

Leatt 3DF 5.0 Impact Shorts-L https://www.amazon.co.uk/dp/B07DYHJ5H8/ref=cm_sw_r_cp_api_i_uR4UCbEHZ3XC4
```

---
## \#44 Posted by: Mobutusan Posted at: 2019-04-20T23:28:14.052Z Reads: 68

```
I've got the Hillbilly impact shorts, and the Triple 8 Bumsavers. Either one is better than none, but I would definitely go with the Hillbilly shorts since they feel like they fit more comfortably, protect more area and have better padding. Those look pretty nice though.
```

---
## \#45 Posted by: davidbonde Posted at: 2019-04-21T11:29:07.089Z Reads: 60

```
I crashed again today this time my own misstake. Was practicing cornering at high speed. Felt good. Nice feeling did a lot of them progressively faster. Until it became to fast :) And then I stupidly tried to run it off. But I had no change and ended up on my chest / stomach. Ended up in the dirt / crass. I wore everything I had but no impact protection other than the kvelar shirt on the chest and I think some rock gave me the two scrapes through the kvelar. But it's not the scrapes that's the worst. It's the feeling after the impact. But hey I am ok nothing seriously and I will be out again when the board is charged back up. 

It become more and more clear to me that I want the impact protection from my safety gear. That will be bulky and limit mobility and freedom, but hopefully not too much. A couple of days ago I ordered this piece. Could have used that today :) 

I am still considering some leathers, but as that can not be returned I will test other stuff first. And BTR doesn't do impact protection on shoulders, and I want it everywhere :) 

@banjaxxed Those look nice. I have seen some good looking crash pants form the MC world with hard protection on the sides as the one you link to. I think that's the way to go. 

I have the hillbilly short. they are ok. I ware the outside my trousers. Not the most sexy looking. But inside the trousers the limit mobility way too much. On the outside I don't notice them. They have a lot of padding BUT the hip crest and the hip padding are located so my trochanter major (the most protruding bone in the hip and where you will hit the ground) are right between the padding. Should not be possible whit all that padding, but it is :) I think I will ad some g-form pants for everyday riding and then the hillbilly pants when I am pushing my limits. 

![IMG_9212|666x500](upload://49Inf77KkpYIDG2L64mAnvAYGgO.jpeg)




Alpinestars bionic tech:

https://www.fc-moto.de/epages/fcm.sf/?ObjectPath=/Shops/10207048/Products/Alpinestars-Bionic-Tech-Jacket/SubProducts/Alpinestars-Bionic-Tech-Jacket-0003&Currency=DKK&Locale=da_DK&gclid=CjwKCAjwqfDlBRBDEiwAigXUaHYneAwqoi6ft3OKo0ASWE_gAgcSbj6EnYo_KCRK7l10jjOvq7sVCxoCLrAQAvD_BwE


I ended up here and the remote there :) ![IMG_9211|666x500](upload://3fo33ZGEhCCu7wPGYuU3CibkrH.jpeg)
```

---
## \#46 Posted by: banjaxxed Posted at: 2019-04-21T13:06:55.712Z Reads: 53

```
The MX/MC world are very mature sports with products developed over decades, the same type of injuries occur, makes sense to piggyback their protection 

Asides from the insignificant looks, what appeals is the hip area above the short line, these have lips areas which protect that part which often gets rashed.

I’d you want real protection of that area you need zip together bottoms/jackets as a jacket will almost certainly ride up when you slide

[quote="davidbonde, post:45, topic:90143"]
hard protection on the sides
[/quote]
```

---
## \#47 Posted by: davidbonde Posted at: 2019-04-21T13:41:13.046Z Reads: 56

```
[quote="banjaxxed, post:46, topic:90143"]
The MX/MC world are very mature sports with products developed over decades, the same type of injuries occur, makes sense to piggyback their protection
[/quote]

Yes. I often come close to something that would be ideal for us but only close. At some point we need to develope something specific to eskating
```

---
## \#48 Posted by: Bataleon Posted at: 2019-04-21T14:19:34.469Z Reads: 54

```
[quote="davidbonde, post:47, topic:90143"]
Yes. I often come close to something that would be ideal for us but only close. At some point we need to develope something specific to eskating
[/quote]

A Swedish company called Lazy Rolling has developed a [Kevlar lined armored hoodie](https://www.lazyrolling.com/products/armored-hoodie-by-lazyrolling), specifically for the eskating community, which seems promising.
```

---
## \#49 Posted by: deucesdown Posted at: 2019-04-21T15:12:14.953Z Reads: 52

```
Most motorcycle gear is designed for one time use, ridht? At least the road bike style stuff. With the thought that hopefully you never make use of it. Nylon that shreds and is not repairable.

Race stuff (leathers) is different, and I don't know anything about dirt stuff, but I imaging you expect to fall in those disciplines and the gear is made for more than one get-off?
```

---
## \#50 Posted by: taz Posted at: 2019-04-21T16:01:46.167Z Reads: 59

```
Not really. It does take some damage but it is definitely not a one deal affair. I have taken quite a few spills and my motorcycle jacket is in perfect working order.

![20190421_185821|375x500](upload://wqOaniRGs5DSkSI3MDQoM8cGoNI.jpeg) 

![20190404_093617|666x500](upload://imySFqsIGoiioI1NB6Y0hwhHEUT.jpeg)
```

---
## \#51 Posted by: davidbonde Posted at: 2019-04-21T16:14:30.790Z Reads: 56

```
@Bataleon Yes Robin and Daniel has started to make something for us. It does look promising. Let's see what they can make of it in the future. I know they want to be here for a long time. 

@deucesdown It seems that the motor cross and mountain bike gear are the gear that come closest to what I want from safety gear when I push the limits. I little correction of the design and it will be perfect.

@taz Do you have a link to the jacket your are using?
```

---
## \#52 Posted by: taz Posted at: 2019-04-21T16:30:16.193Z Reads: 54

```
It is a Dainese Air Flux D1 and I have added a back protector. It is a motorcycle summer jacket so I can also use it during the summer. As long as I keep moving it is ok. During the winter I have to wear a down jacket underneath it since it does not provide any warmth or wind protection.

https://www.dainese.com/row/en/air-flux-d1-tex-jacket/201735163.html

I would love to also get a leather winter jacket but it is a lot of money and since I got this one to work, I don't really see a reason for it.
```

---
