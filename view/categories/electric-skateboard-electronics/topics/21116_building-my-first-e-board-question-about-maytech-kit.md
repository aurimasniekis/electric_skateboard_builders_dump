# Building my first e-board, question about maytech kit

### Replies: 22 Views: 1767

## \#1 Posted by: yarinasher Posted at: 2017-04-16T02:27:52.685Z Reads: 188

```
im planning on building my first e-board, single drive 10s4P li-ion battery, which can give about 60 amps.
I've read a few days in this forums, and got impressed by maytech motors, which everyone rebrand and sell with their logo.
did a bit of search, and met with this kit: https://www.aliexpress.com/item/Maytech-11pcs-belt-drive-electric-skateboard-6365-rc-outrunner-brushless-motor-for-electric-skateboard-with-hall/32777186977.html?spm=2114.10010108.1000023.12.nXhhff
sounds that it includes everything, all the parts should fit each other with matching connectors, only need a deck and a battery.

sombody can recommend? opinions?
what kv motor should i choose? and size? tought about 190kv 6374. im like 85kg, mainly flatland terrain, few hills. reminding li-ion 10s4p. want top speed of like 40km/h.
im very exited about it because e-boarding is a really small scene here in israel. i hope this will help to spread the word!
```

---
## \#2 Posted by: pennyboard Posted at: 2017-04-16T02:57:21.536Z Reads: 182

```
First off welcome to the community, you made a create choice asking for help on here about building your board, it'll save you a lot of future problems stress. 

The kit looks to include everything except a battery, as you said. I personally do not have any experience with Maytech VESCs, but what I've heard is that they're fine, as long as you set them up correctly, same as any other VESC. You're correct in assuming you need only a battery and a deck. 

Since you're going to be running a 10s battery, I would deffinetly go with a 190kv motor because you do not want to exceed the e-rpm limit of the VESC. With 190kv, 10s, and the 83mm wheels the kit comes with, you should expect a realistic top speed of 40km/h, with plenty of torque for climbing hills if you ever need to. Also, if you ever decide you want to go faster, you can always swap out the pulley the kit comes with for a 16T pulley and get closer to 48km/h top speed.
```

---
## \#3 Posted by: Hummie Posted at: 2017-04-16T03:20:00.103Z Reads: 165

```
I think u could get a better vesc that would do the foc program and good rubber wheels and all the rest of that stuff for that price from other vendors here.
```

---
## \#4 Posted by: yarinasher Posted at: 2017-04-16T03:46:55.234Z Reads: 162

```
pennyboard, thanks alot! i tought about it and maybe better with 6355 motor? for keeping the option to put another one in rear... (if ill get bored)
and im almost sure i will upgrade the wheels to 97mm flywheels, but for the price of the 83's that comes with the trucks - why not check them out first? anyway - would it still be optimistic with 190kv motor? i guess i can change the gearing ratio to balance that, no?

hummie, thanks for the info about the foc.
just found this:
http://www.michobby.com/product/electric-skateboard-2pcs-trucks1pcs-motor-mount1set-pulleysbelt4pcs-wheels-with-bearings/?attribute_pa_color=blue
+
http://www.michobby.com/product/hot-combo-6355-190kv-sensored-motorremote-for-electric-skateboard/

that seems to include all components but vesc (and ofcourse deck and battery) in just less than 300$. 330 including shipping with TNT express. (first time i hear about this service. its fine?) which vesc is recommended so? i can order seperate.
```

---
## \#5 Posted by: landonkun Posted at: 2017-04-16T04:58:23.502Z Reads: 142

```
Ollin vescs are pricey, but seem to be very popular due to their high reliability.

http://www.ollinboardcompany.com/product/vedder-s-speed-controller

I'm personally starting out with the Maytech VESC (literally setting it up for the first time this moment), so I can't give my opinion on it, but I figured I'd start with a cheap one for now and upgrade someday if I really feel the need to use FOC mode. I've heard Maytech's run BLDC mode just fine.
```

---
## \#6 Posted by: yarinasher Posted at: 2017-04-16T05:13:40.264Z Reads: 136

```
how's enertion vesc-x? or diy's? diy's almost half price than ollin... if it work in foc and no problems so...
and good luck with your vesc!
```

---
## \#7 Posted by: landonkun Posted at: 2017-04-16T05:18:22.532Z Reads: 135

```
I have no experience with them, but here's my two cents:
From what I've heard, the vesc-x is also pretty solid, but pricey as well. The DIY one isn't a bad vesc either, but isn't _quite_ as robust as ollin's. There are also a couple users on here (I'd have to look up who, I forgot) that have the Maytech vesc's running FOC mode without any issues, despite Maytech saying they aren't designed for it. So whether it works or not could depend on user error.

Bottom line: you get what you pay for.
```

---
## \#8 Posted by: PDXroses Posted at: 2017-04-16T06:10:51.526Z Reads: 122

```
Ollin VESC quality is no better than Maytech. Prove me wrong, anyone?  The owner, Chaka, is very active on this site and did a good job branding his merchandise.
```

---
## \#9 Posted by: Eboosted Posted at: 2017-04-16T06:40:30.115Z Reads: 122

```
I've heard Maytech VESC do not have bootloader installed, so you can't install a new firmware without installing the bootloader first.
```

---
## \#10 Posted by: SirDiff Posted at: 2017-04-16T07:44:38.687Z Reads: 119

```
[quote="PDXroses, post:8, topic:21116"]
Prove me wrong, anyone
[/quote]

Okay. You can ask him a list of the improved components, he has no problem sharing that. He also has a direct fet version, with added heatsinks. He also provides warranty for any problem, which nobody else does. I have never bought from him, I'm not a fanboy, but what you said is just ridiculous
```

---
## \#11 Posted by: PDXroses Posted at: 2017-04-16T08:06:03.829Z Reads: 111

```
Sure, Chaka adds more shit on his VESC and jacks up the price. You still haven't proven why it's BETTER. If there's stats showing better reliability and performance than Maytech's, I'll concede. Til then, you're the ridiculous one. :slight_smile:
```

---
## \#12 Posted by: SirDiff Posted at: 2017-04-16T08:16:32.449Z Reads: 112

```
First off, I've seen many people using foc on chaka's vescs, but only a couple of guys were able to get it running on maytech's. Second, construction quality is clearly better (you can check @Karen_Vanda's photos of the circuits of standard Chinese vescs) 
Many people with chaka's vescs with heatsinks were able to climb Hills that overheated their previous vescs, I see that pretty often. 
Even if they worked the same, I've never seen anyone complaining about chaka's warranty. So, if you have any problem he will replace your vesc in a question of days. Maytech will take months, IF they admit it's their fault. 
Now, who are you? You joined the forum yesterday and you're already talking shit about a producer nobody ever had to complain about. Troll?
```

---
## \#13 Posted by: Wubbalubbadubdub Posted at: 2017-04-16T11:06:02.555Z Reads: 108

```
I just found this out, and thought I would share: a lot of maytech VESCs (maybe all?) don't have a boot loader installed, so if you decide to use one of the cool apps floating around the forum, you will have to get a programmer and install it yourself.
```

---
## \#14 Posted by: yarinasher Posted at: 2017-04-16T12:19:56.290Z Reads: 107

```
thanks for that info.
anyway - i just realised i need on/off switch switch as well.. (vedder anti spark switch). ollin sells them assembled together so maybe thats a good idea.
i like the idea of foc so i guess ill go with that combination.
how's maytechs trucks? they are 50 degrees? i guess all trucks have the same performance.. but didnt found any info about their angle.
and motor mount? sombody that have this trucks can approve it works?
```

---
## \#15 Posted by: PDXroses Posted at: 2017-04-16T16:30:04.571Z Reads: 92

```
@SirDiff
Now now calm down. This is just skateboarding after all. No need to call someone a troll because they disagree with you. I'm glad you love Ollin, but my point stands. You have anecdotes. Well one fact is that his VESCS have been shipping late and email responsee are slow. He's probably too busy with his late board shipments. That's a fact so warranty or not, I call bs on "immediate  response."  My Maytech VESCs are working very well and so are the other thousands sold over the months. Saving my $ for other components.  Have a great day.
```

---
## \#16 Posted by: SirDiff Posted at: 2017-04-16T17:02:08.612Z Reads: 92

```
I just find it strange that you come here saying "he just added some shit and jacked up the price" 
I don't have neither of those vescs, I'm waiting for a custom made one from Denmark, so this conversation doesn't concern me at all. I wouldn't pay 170 dollars for a vesc, knowing it costs less than a half for the components, and I know maytech vescs are probably good enough if set up the right way. But at the end, the quality in chaka's one is just superior. Maytech's are not even rated for foc. Not saying chaka's it's a must buy, but if you are a beginner and you are not completely sure about what you're doing, the warranty, heat dissipation and foc capability MIGHT be worth the extra cost. That said, I think everybody should give 2 years warranty (stuff sold from EU automatically has that)  and a vesc should cost 110€. Try @zmoney's axle vesc, it should be right in the middle
```

---
## \#17 Posted by: flatsp0t Posted at: 2017-04-16T17:41:18.374Z Reads: 92

```
Maytech VESCS are crap, they remove shit and production steps needed for Complete functionality and jack the price down.
They are also not doing proper QC.
[quote="PDXroses, post:8, topic:21116"]
Prove me wrong, anyone?
[/quote]

I can play that game.


But to get on topic:
Maytech does some good motors.
Diy Vescs are good and their customer service is ok, but they have much to do in the moment and can be slow.
If you are from europe, you can also check out esk8.de.
VescX also seems to be reliable, but their customer service was bad when i dealt with them last time, but they got better since then.

Ollin vescs are super reliable and he will repair them no questions asked iven if it was your fault. But you dont really need them if you are not doing some high power or FOC stuff.
Same goes for VescX. if you dont need the extra current/ FOC, it is not worth the difference.

It is also worth checking out Axle, it is @longhairedboy s goto at the moment (for Applications that dont need ollin/vescX) and if they survive the stuff he builds they cant be that bad.

190kv motors are good at 10s.

To play around with different gearings, cou can check out this nice calculator: http://calc.esk8.it/

Here is a complete list of VESC sellers.
https://www.electric-skateboard.builders/t/worldwide-vesc-directory/16764
```

---
## \#18 Posted by: pennyboard Posted at: 2017-04-16T18:13:29.185Z Reads: 83

```
I think you've made some interesting points, in saying that there's not necessarily proof that ollin vescs are any better. While it's true that there's no hard facts proving that, I think the general feeling in the community is that because most people report no problems with it, and those that do are usually user error and fixed for free under the warranty, it is the better VESC, if not for its construction quality, then for its warranty when things break.
```

---
## \#19 Posted by: dimnsionofsound Posted at: 2017-04-16T18:16:53.800Z Reads: 88

```
IIRC Ollin adds a couple capacitors or resistors that most of the other manufacturers have removed, though which are present in Vedder's schematic. They also apply a conformal coating to the board so hopefully if you get it a little wet, it won't just die?
```

---
## \#20 Posted by: longhairedboy Posted at: 2017-04-17T11:56:13.248Z Reads: 84

```
[quote="flatsp0t, post:17, topic:21116"]
Maytech does some good motors.
[/quote]

indeed they do. I bought a bunch of them with my name on them. I have some extras for sale on my site. 
https://longhairedboy.com/products/totally-bitchin-190kvs-6355-electric-skateboard-motor

Also, Maytech VESCs are indeed crap. But maybe only for now. I burned up the sample they sent me in approximately 8 hours. However, i believe they are taking input from venders and builders so if you tell them they are crap, they will improve them. Maytech has a way of listening to people like us over time. 

As an example, I bought so many steeze remotes that now they're giving me dealer discounts. But they are also taking me seriously when i tell them the A and B buttons need work as those tiny SMD switches keep popping off on impact. They're dead easy to fix, and dead easy to reinforce to prevent the issue, but they are actively trying to improve things. I love those remotes for man many reasons, and if that issue can be resolved then there will not really be any issues with that remote at all. I'm probably going to have some extras of those too soon. 

Maytech is getting better, and they aren't the worst people to work with. I recall they had a bad spell with their motors at first too. But i feel like they're on the right path. 

[quote="flatsp0t, post:17, topic:21116"]
It is also worth checking out Axle, it is @longhairedboy s goto at the moment (for Applications that dont need ollin/vescX) and if they survive the stuff he builds they cant be that bad.
[/quote]

I'm having a difficult time telling the VESC-X and the AXLE 4.12s apart on the street. The VESC-X is slightly smoother and more polished and more efficient but with the price difference its hard to ignore AXLE. I just shipped a board with AXLE vescs that were replacements for the older Enertion 4.12s that were in there. We'll see how they hold up for the customer. 

Both are are a pleasure to work with and ride on.
```

---
## \#21 Posted by: torqueboards Posted at: 2017-04-17T16:07:17.363Z Reads: 74

```
@yarinasher - Our parts come out to $451.97 compared to the setup which you posted. Just FYI. We're also USA based if it helps.
```

---
## \#22 Posted by: yarinasher Posted at: 2017-04-17T17:10:34.646Z Reads: 70

```
I live in Israel, well looked into your stuff and thinking maybe ill get most of my setup including 10s4p battery & enclosure..
you can deliver this to Israel? specificly the battery? 
I saw you have 12mm pulley system... im leaning towards 15mm.. you have those also?

another thing is, i read here on some threads about all the li-ion batteries limit of low amp output against lipo's, and got confused so much, as it seems 30a continuous Amp output from the battery is less than the vesc can handle (upto 40-50a continuous without warming up too much if im not mistaken), and a 6374 or even 6355 motor that can draw up to more amps than the battery can deliver. but it also seems that 30amps is enough in the real world, which in stress situations can spike more for a few seconds without hurting the battery. but i dont fully understand this, as i imagine a 1km hill that can stress the motor , which will benefit of more than 30amps in reasonable speed, and this stress sounds like unhealthy for the battery. (and vesc maybe also), for more than a few seconds.
but then again, from the other side everybody uses this kind of power packs and it seems to work well also in dual motor setups.
so now im trying to decide which single motor will be the most efficient way to go with 30amps continuous 10s4p power pack. i guess 190kv.
6374? 6355? seems like the 6355 since its weaker, but maybe stronger motor will be more efficient under load? (85kg rider)
also foc sounds awsome, as a smoother, quieter and more efficient ride. but also very dangerous to the vesc. still undecided about that, and if i go with bldc mode maybe better save like 70$ and go with a DIY's vesc for example.
i hate decisions. :slight_smile:
any help will be greatly appreciated.
sorry about the length of this!
```

---
