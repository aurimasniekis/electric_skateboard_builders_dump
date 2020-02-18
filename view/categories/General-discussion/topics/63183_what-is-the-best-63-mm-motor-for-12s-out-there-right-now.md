# What is the best 63 mm motor for 12s out there right now?

### Replies: 48 Views: 1124

## \#1 Posted by: dareno Posted at: 2018-07-28T22:56:07.182Z Reads: 221

```
So this time instead of just opening up a new topic I have spent all morning scrolling and researching and  there doesn't seem to be anything recent so I still am none the wiser.

What is the best motor on the market right now for a dual belt set up running 12s?
I currently have twin SK8 6374 192 kv on a steet set up with 218 trucks and apart from a dead hall sensor on one they are performing well and have been for 4 months on 10s but I am upgrading my battery to an @TinnieSinker 12s 4p and I thought in for a penny in for a pound and in the spirit of builds everywhere why stop there?
  What about 6380  from @torqueboards or the 6384 monsters that @Eboosted used on a build?

Thoughts please
```

---
## \#2 Posted by: kalebludlow Posted at: 2018-07-28T23:06:05.326Z Reads: 212

```
You have managed to fit two SK8 6374 on TB218? I was under the impression that they were far longer than 74mm so they didn't fit. I'm also doing the same as you with using a battery from @TinnieSinker
```

---
## \#3 Posted by: Skunk Posted at: 2018-07-28T23:11:41.660Z Reads: 208

```
I think you want a higher kv on 12s. 
I'm not sure on that,  I'm very new to all this.  But I feel like I just read a conversation about this topic in the last 48 hours.
```

---
## \#4 Posted by: Colson003 Posted at: 2018-07-28T23:16:28.502Z Reads: 204

```
Stick with the motors you have currently if you’re looking for a higher top speed. Get around 170kv if you’re looking for more torque.
```

---
## \#5 Posted by: pat.speed Posted at: 2018-07-28T23:25:49.896Z Reads: 201

```
Generally the higher the voltage, the lower your kV should be

I personally like 12s on 190kv as that gets you upto about 60km/h with ease
```

---
## \#6 Posted by: kalebludlow Posted at: 2018-07-28T23:28:18.237Z Reads: 195

```
What sort of gearing and wheel size to achieve this?
```

---
## \#7 Posted by: dareno Posted at: 2018-07-28T23:33:27.373Z Reads: 186

```
@kalebludlow 

[quote="kalebludlow, post:2, topic:63183"]
You have managed to fit two SK8 6374 on TB218?
[/quote]

Yeah they are a very tight fit but doable.  The rear bearing is outside of the can which makes them longer than 74 but the stator size is the same.  It leaves about 5mm between them and with the longer reverse mount plates they do flex a bit so i'm currently fabricating some braces for them to keep them solid
```

---
## \#8 Posted by: Skunk Posted at: 2018-07-28T23:35:59.075Z Reads: 176

```
Good to know I've been reading too much and I must have had it backwards
```

---
## \#9 Posted by: pat.speed Posted at: 2018-07-28T23:42:35.581Z Reads: 179

```
I running 12s, 195kv 6355, 97mm wheels and 2.7:1 gear ratio. Top speed ~55km/h but it could easily be more if I lowered my gearing.

Build threads here


https://www.electric-skateboard.builders/t/re-re-rebuild-my-boards-thread/50805
```

---
## \#10 Posted by: uigiroux Posted at: 2018-07-29T01:54:31.801Z Reads: 155

```
This tells you what the ideal kv is for the type of battery you have.

https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125?u=uigiroux


It says in the link that for 12s, 170kv is the most ideal, any higher and you lose to end performance.   As for which is the best brand, well that's likely different for many people.  I recently got the Torque Boards 6380's  @170kv and they are amazing.  They actually are 6384's, but they were able to save some space and make them more compact.  Hope that helps :smile:
```

---
## \#11 Posted by: dareno Posted at: 2018-07-29T02:56:51.677Z Reads: 146

```
Just what I was after with this thanks  Real world experience with the different options.. must admit I am leaning toward the tb 6380 as the whole point of the upgrade is to achieve the performance I want without having the settings at potentially damaging levels as I have to with the 10s.
I want torque and speed but primarily torque as the board will hit 50kmh now and that really is the limit with how I like my trucks set up.   It will be nice to have the option to fly though......
```

---
## \#12 Posted by: Eboosted Posted at: 2018-07-29T03:27:44.651Z Reads: 138

```
To be honest if you want to feel more torque even a big ass 6380 won't be much different than a 6355 as long as you ride on flat surface. From my experience bigger motors won't give you faster acceleration, they will give more torque only so I'd be noticeable when riding up a hill, launching from a really bad terrain or launch better when off roading, I'd also help if you are a big buy 120kg or so. Bigger motors also have the disadvantage of more weight. 

If you are looking for faster acceleration then upgrade to 12S, that's is really an amazing upgrade, cheaper than a set of new motors.

You should try to get 60km/hr final speed on your boards, use the esk8 calculator and select from you hardware from there. 

Once upon a time I wanted the board with the highest torque ever, I went down to a really torquey pulley setup and a reeaaaaly low final speed, 200kv 6384 motors, 12T motor pulley, 72T wheel pulley on 12S battery and 200mm pneumatics, I though it was going to be a fun board, the launch from a dead stop was a little better but the overall riding experience sucked balls, the peak torque was too narrow on the powerband, just a glitch of full torque, the top speed uncontrollable when lifting the throttle, top much drag up top, the small motor pulley skipped like mad. 

So my final word on it would be to look for 60km/hr final speed, use 14T wheel pullies minimum, choose the correct motor size not for the acceleration but for the battery discharge current capability and consider weight, 12s has a bad reputation but gives you plenty of power to play with, all my electronics have been working fine on 12s for a really long time in everyday abuse. 

Hope I could be of some help to people around here trying to choose their hardware
```

---
## \#13 Posted by: Wraith Posted at: 2018-07-29T03:33:37.147Z Reads: 127

```
Thanks @Eboosted! Speaking of 12s, do you have a discharge bms in use with your setups? What would you say is a safe setting for vescs as I’ve read thats usually what blows due to the 12s batteries haha
```

---
## \#14 Posted by: Eboosted Posted at: 2018-07-29T04:11:58.633Z Reads: 125

```
No. Only one of my 12s builds has a BMS for discharge, the others have bms for chaging only. I had too many close calls because of the BMS shutting power down braking on full battery no matter if it's runing a 10s or 12s. The one with bms for discharging is charged up to 50v not 50.4v and does not trigger power shot down.
```

---
## \#15 Posted by: Wraith Posted at: 2018-07-29T04:14:26.348Z Reads: 120

```
Oh so the bms cutting power off the the vescs is a reaponse to over charging? What bms do you use? Can that be programmed not to happen?
```

---
## \#16 Posted by: dareno Posted at: 2018-07-29T04:20:06.025Z Reads: 124

```
Thanks man real helpful,  I am using 6374 now so not much point in the upgrade then?  The new battery is 12s 4p 30Q and my goal was to get some good hill climbing ability with my fat ass 110kg without running everything as high as I can go therefore risking blowing components.  
Also if I go buying new motors then I will have two spare laying around and with the two vescs I have laying around and the 10s battery from the original board I could effectively build ............you see where I'm going with this lol
Thanks again
```

---
## \#17 Posted by: dareno Posted at: 2018-07-29T04:21:09.824Z Reads: 123

```
Now really is that in the spirit of the building ethos?  Encouraging me not to buy new stuff? :wink:
```

---
## \#18 Posted by: torqueboards Posted at: 2018-07-29T04:25:24.564Z Reads: 118

```
@dareno - No need.. In San Francisco, I would typically only ride with Dual 6355 190KV with 12mm belts on 12S.. Climbs everything except for hills with stairs (those ones you don't even want to go up).
```

---
## \#19 Posted by: dareno Posted at: 2018-07-29T04:36:36.569Z Reads: 112

```
@torqueboards considering it was your motors I was going to go for that is valued information indeed!!
I do live in a very hilly area too so hence the 12s
```

---
## \#20 Posted by: Skunk Posted at: 2018-07-29T04:39:08.894Z Reads: 112

```
Man this thread has me going back and forth again on whether to go 10 or 12s for my build.....
I thought I decided 10s because I'm really not in a situation where replacing parts world be easy for me if my focbox was to blow running 12s.
But at the same time I don't wanna put $1500+ into a board that doesn't satisfy me....
I've got 190kv 6374 motors and am 200lb with my pack. Pretty flat town.
```

---
## \#21 Posted by: torqueboards Posted at: 2018-07-29T04:48:01.733Z Reads: 106

```
Just depends on what you need. If you want a commuter, you probably don't want 6374s. If you don't ever have to carry it. I'd opt for the bigger motors but the difference won't be insanely better unless you're running a huge battery.

I like 12S.. most of the final decisions are a few bucks more $10-50. If you decide less but want more later you end up spending more because you still bought the first item.
```

---
## \#22 Posted by: Wraith Posted at: 2018-07-29T04:48:46.935Z Reads: 102

```
I was in the same spot as I’ve read that 12s was to be avoided due to its risk to the vescs but I wanted something that wouldn’t lack in supplying the power needed in future upgrades to motors so I switched from ordering a 10s to a 12s from @tinniesinker lol
```

---
## \#23 Posted by: Wraith Posted at: 2018-07-29T04:49:56.927Z Reads: 100

```
Exactly why I changed my mind on 10s haha
```

---
## \#24 Posted by: Skunk Posted at: 2018-07-29T04:52:32.836Z Reads: 101

```
It is a commuter but I wouldn't have to carry it at any point. Most of my commutes are about 5 miles round-trip.
I've also got a smaller board (kick tail) I'm building that I'd like to get 2 6355 for.
I'd like to be able to go on fairly long rides and maintain somewhere in the 30 miles per hour.
```

---
## \#25 Posted by: torqueboards Posted at: 2018-07-29T04:59:22.663Z Reads: 101

```
@Skunk lol... it's hard choosing.. but choose the best one you think you'd prefer. Dual 6355 is capable of 30mph.
```

---
## \#26 Posted by: Skunk Posted at: 2018-07-29T05:01:38.394Z Reads: 101

```
I'll probably be picking up 6355 from you if the direct drives aren't available in the next few months for my classic kick tail board.  I've already got the 6374 for the hummie  deck.
```

---
## \#27 Posted by: torqueboards Posted at: 2018-07-29T05:03:40.189Z Reads: 99

```
Yeah, still a while out unfortunately..
```

---
## \#28 Posted by: Wraith Posted at: 2018-07-29T05:04:10.353Z Reads: 97

```
Waiting on @torqueboards direct drives for my hummie deck as well! While I want to be optimistic on the carvon drives, the price and availability is really making it difficult to decide on them sadly
```

---
## \#29 Posted by: Skunk Posted at: 2018-07-29T05:13:06.023Z Reads: 97

```
[quote="torqueboards, post:21, topic:63183"]
unless you’re running a huge battery
[/quote]

Looking at a 10s7p or a 12s6
```

---
## \#30 Posted by: Wraith Posted at: 2018-07-29T05:15:28.461Z Reads: 97

```
You gonna fit that onto your hummie deck? That would be massive and interested on how you’d make your enclosure!
```

---
## \#31 Posted by: Sender Posted at: 2018-07-29T05:15:57.284Z Reads: 99

```
@torqueboards are you still thinking about doing some motors in raw or something else? Mmmm
```

---
## \#32 Posted by: torqueboards Posted at: 2018-07-29T05:20:47.827Z Reads: 96

```
@Sender Only for 6380s. Shiny Black and Shiny Silver. Separate color options.
```

---
## \#33 Posted by: Sender Posted at: 2018-07-29T05:21:21.601Z Reads: 99

```
Nice!!

10char
```

---
## \#34 Posted by: Skunk Posted at: 2018-07-29T05:28:43.425Z Reads: 98

```
10s5p and 12s4 fit single stack, plan on going double stack. Enclosure difference will be less than an inch bigger than psychotillers hummie enclosure .  I should be fine on clearance with running 107s or six shooters.
```

---
## \#35 Posted by: Narnash Posted at: 2018-07-29T05:57:59.053Z Reads: 96

```
12s +long cabels can easily kill a vesc
But you can fix that with some low ESR cspacitors near your VESC in parallel (to smooth out the ripple created by the switching and cable/connector inductance)

The RC rule of thumb is 10cm cable =  220µf cap (more small caps are better than a singke big one)
```

---
## \#36 Posted by: DAddYE Posted at: 2018-07-29T05:59:27.213Z Reads: 93

```
Why 12mm belts?
```

---
## \#37 Posted by: Skunk Posted at: 2018-07-29T06:02:31.876Z Reads: 89

```
Thank you.  These are the kinda things I need to know.
```

---
## \#38 Posted by: Wraith Posted at: 2018-07-29T06:09:10.505Z Reads: 94

```
Yeah I feel like I gotta double stack my 12s5p as well but unsure of what enclosure to use. I’d hate to get one that doesnt fit flush over the hole. Asking Hummie if he can still do an enclosure that can go with it for a 60cell pack like he mentions on the hummie deck thread but thats gonna be something he can do once the decks actually arrive which is about 3 weeks away according to Hummie
```

---
## \#39 Posted by: Wraith Posted at: 2018-07-29T06:13:22.550Z Reads: 94

```
Okay any chance you can point me to where I can read up and look at where I can buy those?

Honestly you lost me at ESR capacitors lol
```

---
## \#40 Posted by: DAddYE Posted at: 2018-07-29T06:31:29.529Z Reads: 92

```
Is there any substantial difference between a 6355 190kv and a 6355 170kv on a 12s2p setup? The latter cost substantially more.
```

---
## \#41 Posted by: Narnash Posted at: 2018-07-29T06:40:25.539Z Reads: 90

```
also @Skunk 

https://www.rcgroups.com/forums/showthread.php?952523-too-long-battery-wires-will-kill-ESC-over-time-precautions-solutions-workarounds
https://www.electric-skateboard.builders/t/how-many-additional-caps-for-12s-vesc-for-long-wires/22171

https://www.electric-skateboard.builders/t/vesc-faq-how-many-capacitors-what-uf/6125

The panasonic FR type capacitors are a example for a good low ESR caps, you will find them on ebay, mouser, digikey and any good store for bare electrical parts.
```

---
## \#42 Posted by: Wraith Posted at: 2018-07-29T06:41:48.254Z Reads: 79

```
Thanks! I nevertheless realized this could save the vescs. I was hoping to throttle discharge from the bms mostly haha
```

---
## \#43 Posted by: Narnash Posted at: 2018-07-29T06:44:16.212Z Reads: 77

```
Mind you that the orientation is important on electrolytic capacitors :D
```

---
## \#44 Posted by: dareno Posted at: 2018-07-29T06:44:48.088Z Reads: 77

```
@Narnash hey man, when you say long phase wiring are we talking board length?  With a dual and vescs beside them would that really be an issue if you keep your settings reasonable?
```

---
## \#45 Posted by: Wraith Posted at: 2018-07-29T06:51:05.472Z Reads: 78

```
Orientation in relation to the vesc you mean? I see a lengthy read ahead of me with the links you sent haha
```

---
## \#46 Posted by: Narnash Posted at: 2018-07-29T06:53:20.725Z Reads: 78

```
battery wire lenth is important the phase wires can be longer and don't need something to smooth ripple
```

---
## \#47 Posted by: dareno Posted at: 2018-07-29T06:56:51.460Z Reads: 81

```
That was my understanding but when I read your post i had a little panic lol  no my battery wiring will be fine the pack takes up the whole of the enclosure and the vescs sit on top in their own so the wiring can be standard.  Never used 12s before so I am a bit nervous about frying things  Thanks
```

---
## \#48 Posted by: Narnash Posted at: 2018-07-29T06:56:56.127Z Reads: 81

```
@dareno
Na, I wanted that you don't put them in reverse since electrolytic capacitors will likely break kinda violently when you put them in reverse polarity.

But it's important that you put them in parallel and not in serial to smooth the input.


With very short battery wires and a good quality VESC 12s isn't likely to cause any issues, but espacially under FOC the inductance of your battery wires (wich get's higher the longer they are) together with a full charged battery can spike your VESC to death pretty easily.
Added caps are a complete must have if you use  splitted battery and VESC, I would recommend them for anything with 20cm or longer cabels.
```

---
