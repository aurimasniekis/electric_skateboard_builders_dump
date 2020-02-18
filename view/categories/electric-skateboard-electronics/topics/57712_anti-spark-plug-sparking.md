# Anti-spark plug sparking?

### Replies: 32 Views: 993

## \#1 Posted by: Fafu Posted at: 2018-06-03T21:24:15.462Z Reads: 212

```
Hi!
Very new here :slight_smile: glad to be part of this colective
I recently built my electric longboard, this is unfortunate because i feel I dont need a girlfriend now, as I spend tones of time in it…

As a first question in the forum, I have a problem with the antispark plug wich I could not find the answer in the other posts: **it sparks anyway!** is this normal?

some info prio to the spark:

this is a 12S 1VESC 
- motor longboard , postive cable going to VESC has the antispark female in the middle, and close the circuit a male with a fuse.
- when i plug it half way ,precharge circuit with the resistor, the VESC blinks (I understand here capacitors are charged and i can go all way in)
- when i go all way in after some second(s) a spark sounds in the XT90 antispark, then VESC turns ON and works fine --for the moment…
- after that, nothing broke, resistor in place, no magic fumes and stuff like that…
in any case im afraid to plug all the times as the spark actually happens despite the setup!

thinking now on using an extra antispark I have from DIYelectricskateboard

Best regards!
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-06-03T21:30:37.795Z Reads: 204

```
i ve use 90s countless time but never had that issue before. may be u need new 90s. 
btw spark won't kill anything. it just eat away ur plug everytime it sparks.
```

---
## \#3 Posted by: b264 Posted at: 2018-06-03T21:31:28.923Z Reads: 199

```
Please post a photo of it
```

---
## \#4 Posted by: Fafu Posted at: 2018-06-03T21:40:48.859Z Reads: 194

```
Hey Thanks for the answers!, 

Well before not using an antyspark plug it actually burned a capacitor and lifted a track out of the VESC.. wich I had to resolder :( 

If this helps, I only hear the spark with 12S, when i am plugging 9S, 6S or 3S there is no spark. 

I will replace the antispark and lets see... THX!
![5e0b6d0b-0709-43cd-9db0-ab1725e8b548|375x500](upload://ujezYpdJpaLjKJTM7zPSLxF6Jah.jpg)
```

---
## \#5 Posted by: Hummie Posted at: 2018-06-03T22:00:51.331Z Reads: 176

```
youll need to replace the plug with the green.  it has a resistor in it and that makes the circuit first for a split second reducing the current and that stops the spark.  ive gotten sparks out of my xt90s after they finally burn out.  its not the worst thing and will just damage your connectors and increase the resistance there, and make a scary spark.    weird how you say it wont happen with the lower voltage
@Fafu interesting you burned a capacitor out without the antispark. was it one of the big ones going to the battery or on the board.  I imagine with a huge current spike charging the capacitor it could be more rough on them but never heard of it being the case
```

---
## \#6 Posted by: Fafu Posted at: 2018-06-03T22:20:24.538Z Reads: 169

```
Hi!,

Regarding the first comment on the green plug, that the one I actually use! it works making vesc blink when is pre-inserted, but sparks when I finish to put it in.. so lets say it does not fully work as expected, like capacitors have time to discharge before i fully plug and then Sparks? Will replace the antispark tomorrow and let you know!

Regarding the capacitor, was the c51 form positive to floor, the track taking that current shorted,![Capture|149x140](upload://n4Whrbgu9pVXre7Hs7GAQ2dlhPZ.PNG)

the track to that capacitor shorted, (that track has 2 or 3 paralel tracks underneath but rewelded it anyway because 12S might take too much current and that extra track might be needed...
![Capture2|273x443](upload://oDTOvGqgIifEioPCqLIdYhY83qE.PNG)

What I think regarding the capacitor and the track, I never used antispark with 3S at the begining and something broke. plugging one day the 3S this happened. I cant tell 100% if it is related **But now with new capacitor, track in place and antispark (sparking :S) it works fine**

Thanks!!
```

---
## \#7 Posted by: koralle Posted at: 2018-06-03T23:02:51.191Z Reads: 147

```
Mate, get a Vedder antispark! They are not expensive and *very nice*
```

---
## \#8 Posted by: Fafu Posted at: 2018-06-04T21:45:21.924Z Reads: 131

```
Guys!! Just replaced the antispark... IT WORKS! well that is strange, maybe it was dirt and current didnt flow fully when half plugged: vesc didnt turn On 100%, only blinking, but now it does! 

I did a super small fuse with 2*20A car fuse :slight_smile:![IMG_20180604_212107|666x500](upload://nLIrB4JNIgQSi3lgkdDK4SWfXvQ.jpg)
```

---
## \#9 Posted by: Hummie Posted at: 2018-06-04T22:21:36.184Z Reads: 127

```
can you tell me what you did because I'm confused.   Are those two 20amp car fuses you used to make antispark loop key?   40a max?  that's not much and would likely be high resistance.    and you didn't replace the green side just this side?  I'm confused as to what your problem was originally now since you didn't replace the green side with the resistor connection
```

---
## \#10 Posted by: E1Allen Posted at: 2018-06-04T22:46:50.678Z Reads: 122

```
Bridge that connection with large gauge wire or copper.  I don't know where that idea came from but don't do it.  Like hummie said, more resistance and wait till you blow that going uphill or accelerating fast = streetface.  A fuse like that isn't a good idea.
```

---
## \#11 Posted by: Fafu Posted at: 2018-06-04T22:57:32.172Z Reads: 115

```
Hi! Sorry i understand it is confusing, i replaced the green part, and also the male as both looked very dirty/burned

So the male is the fuse I did it new, using 2x20A car fuses, removing enclosue and welding it. 

Regarding the fuse value, well, i will try 40 and limit with vesc slightly below that value. When i get more experienced i could increase, what do you think? FYI i had the chance to try it only a couple of times before something broke... But now things look promising!
```

---
## \#12 Posted by: E1Allen Posted at: 2018-06-04T22:59:48.130Z Reads: 111

```
I think you should not do a fuse like that.  I think you should bridge the gap with wire, not a fuse whatsoever.
```

---
## \#13 Posted by: Fafu Posted at: 2018-06-04T23:03:26.710Z Reads: 105

```
I see.. so maybe the question is, why do we need a fuse?
```

---
## \#14 Posted by: E1Allen Posted at: 2018-06-04T23:13:45.875Z Reads: 102

```
You don't.
```

---
## \#15 Posted by: onepunchboard Posted at: 2018-06-04T23:20:08.486Z Reads: 100

```
yeah fuse is over-protective. why people even use it? maybe for fet switch ( even this is questionable)

anyways, it may have been the solder part of old 90s is nearly touching, and on 12s was arcing through the air gap.
```

---
## \#16 Posted by: Fafu Posted at: 2018-06-05T06:18:53.262Z Reads: 86

```
Understood!! Thanks to all
```

---
## \#17 Posted by: Slak Posted at: 2018-06-05T12:00:31.238Z Reads: 81

```
How do you protect your ESC if there is short-circuit ?
```

---
## \#18 Posted by: Fafu Posted at: 2018-06-05T14:27:28.485Z Reads: 74

```
At the end i decided to keep the 40A fuse, monitor current in a normal ride, see how far I am, cover the fuse with isolating tape, and vesc limit battery current to 35A. In any case 12s and 35A is a >1.5kW wich i doubt i will use... I read a bit, if vesc shorts, i dont to set the longboard on fire so the fuse i think is important!
```

---
## \#19 Posted by: Hummie Posted at: 2018-06-05T14:50:11.058Z Reads: 69

```
Is that how a fuse is supposed to work?  ive never used one so don't know and never think about them but is it simply putting a super thin and high resistant part in your circuit that will melt at a certain amperage because in doing that you will be making the system more inefficient and more likely to have voltage sag.  Id think youd want a fuse that would still do a lot more current to keep the system efficient and if you did have a short it would be a lot more amperage than 40.
```

---
## \#20 Posted by: DeathCookies Posted at: 2018-06-05T14:55:55.170Z Reads: 65

```
The fuse only holds a certain amount of time the rated max load. But if we use a 40A fuse and will get over that amount on every ride for a second. Will the fuse last Long?
```

---
## \#21 Posted by: Hummie Posted at: 2018-06-05T15:02:55.988Z Reads: 61

```
i think if he sets his battery amp limit to 35 he will never hit the 40 unless he shorts but if he shorts it'd be more like 200 amps or something so no point doing so low a fuse as 40 and getting less efficiency and voltage sag always
```

---
## \#22 Posted by: E1Allen Posted at: 2018-06-05T16:27:36.688Z Reads: 55

```
If you look at some of the issues people have short circuiting batteries, the failure stays at the battery.  A fuse downline of that isn't going to help anything. Now if they catch fire and burn the ESC that stupid fuse isn't going to help one way or the other.  This is not cell level fusing like Tesla and some users have done.

Basically the only thing you have done by adding a tiny fuse/any is punish yourself.  
1. Created a weak point for no reason
2. Added a high resistance/high heat spot
3. Created the failure point at the most dangerous scenario on your board, that being high current draw.
4. Maybe save your board instead of your face.  (Pointless maybe)
5. Created a board likely unsafe to ride


Your ESC has limits.  Which include high transient limits.  Which means you could briefly pull over 150a on most of the ESC we use before they overhear.


But keep the little fuse... Maybe wear lots of protective gear.
```

---
## \#23 Posted by: Hummie Posted at: 2018-06-05T19:08:40.465Z Reads: 50

```
[quote="E1Allen, post:22, topic:57712"]
Your ESC has limits. Which include high transient limits. Which means you could briefly pull over 150a on most of the ESC we use before they overhear.
[/quote]
why you say150a when the battery amp limit is maybe 100 on vescs

[quote="E1Allen, post:22, topic:57712"]
If you look at some of the issues people have short circuiting batteries, the failure stays at the battery. A fuse downline of that isn’t going to help anything
[/quote]

If this loopkey were in circuit with the battery and esc as I think they mostly are used, to turn the board on and off, then it would work if the esc broke and shorted and a huge current were to come from the battery.  I kinda like the idea of an integrated fuse but it needs to be capable of way more amps and ultimately Id rather have the battery and esc circuit with no resistance and enjoy those benefits.
```

---
## \#24 Posted by: E1Allen Posted at: 2018-06-05T19:28:16.437Z Reads: 42

```
[quote="Hummie, post:23, topic:57712"]
why you say150a when the battery amp limit is maybe 100 on vescs
[/quote]

It was a arbitrary number since all ESC are different
![image|281x500](upload://6vKA2ayOqWItPVT1W1Gp2PPe6gn.jpg)![image|281x500](upload://mJqO3r2iVUs3FUgS9q2TMlUl8n4.jpg)![image|281x500](upload://lvTeTPYFNQFtbbIv2m1U5mmoLh0.jpg)


Anti spark switch is only meant to not spark.  After that you still want maximum current flow.  I've read enough on this forum to know a fuse isn't necessary.
```

---
## \#25 Posted by: Hummie Posted at: 2018-06-05T19:44:55.089Z Reads: 36

```
i agree and i think if the esc were to somehow short it would probably blow apart and break the circuit and the fuse wouldnt help. 
  the shorts Ive heard of that ended up causing a fire were in the battery cell connections to each other and not the main battery to esc circuit
```

---
## \#26 Posted by: Fatglottis Posted at: 2018-06-05T22:26:38.903Z Reads: 36

```
I’ve put a 100A fuse only to prevent the battery being on fire ”if” the vesc for some reason gets shorted/ welded (Probably/hopefully not). I did not intend to save the VESC itself.
Peronally I will never ever reach that high amount of current on my dual to be even close to breaking the fuse while riding, so I have ruled out the face to ground scenario due to that :slight_smile:

I found a fuse chart and it looked “more or less linear” For a 100A fuse, there would be a voltage drop of 50mV across the fuse at 100A. (Please correct me if I’m wrong)

Is this voltage drop of 50mV really noticeable in performance?

If the fault is inside the battery, the fuse of course won’t help.. but then there must have been something else that was severely overlooked in the design or choosing of material. 

If your board will never fail, you don’t need the fuse. However, I don’t plan to crash on my head either but I wear a helmet anyway :)
```

---
## \#27 Posted by: Fafu Posted at: 2018-06-05T23:25:50.817Z Reads: 32

```
Hi again.. so if we asume losses are irrelevant, maybe the question is, 
- _**does a fuse protects something in any case?, What are the scenarios?**  Is there a failure mode where current is waterfalling due to a short somewhere? How probable is that? we would save in this case batteries?
- **If it saves something... As was mentioned before fuse breaks while riding... Is guaranteed to be launched out of the board?**  Lets take it this way, if i do a electric scooter, does the fuse make sense?

Regardsss!
```

---
## \#28 Posted by: Hummie Posted at: 2018-06-05T23:39:48.830Z Reads: 30

```
can you post the fuse chart please? 50mv isn't anything but what resistance is the 100a fuse and what is a 40 amp fuse's resistance?   how much voltage drop would you have gotten with the 40 amp fuse we can figure it with ohms law
current going through anything is non-linear I think. be nice to visualize what size wire will melt at what current and don't want to do it at home



If you weren't going to fall if it fused sounds like a good idea but I don't think the escs create an open short when they fail and the fuse wont save a battery internal short so there's no point
```

---
## \#29 Posted by: J.Marshall Posted at: 2018-06-06T01:21:15.429Z Reads: 28

```
Fuse won't cause any issues as mentioned previously as far as heat build up, adding any significant resistance, or voltage sag.  While the fuse must have higher resistance than the wire that it is protecting in order to function, a 40amp fuse is still low resistance.

[Fuse Datasheet](http://www.littelfuse.com/~/media/automotive/datasheets/fuses/passenger-car-and-commercial-vehicle/blade-fuses/littelfuse_atof_datasheet.pdf)

From that datasheet you can see that a 40amp fuse has a resistance of 0.00144ohms. If we pump 40amps through it, which can be done for 360,000 seconds before blowing, we would have a voltage drop of 0.0576V!  You will not notice that sag in voltage. You can also check out the graph for current versus time to see how high a load it can handle for how long.  As you can see, a 40amp fuse will never blow due to a 40amp draw on an esk8, something that may seem counter-intuitive.

I'm fairly new to the hobby of esk8 so I don't have too much knowledge of the typical failures.  The fuse would most likely help you in the event of a short between your battery wires (after the fuse that is).  As long as the fuse was sized properly, I think you are going to face plant no matter what the failure is if it is bad enough that it would blow a fuse.  

I guess the only thing to think about is that just about every commercially designed power circuit that I have seen employs the use of fuses.
```

---
## \#30 Posted by: Hummie Posted at: 2018-06-06T02:16:10.704Z Reads: 26

```
so how many amps does a 40amp fuse protect against?!    why the hell would they call it a 40amp fuse if it takes 40 amps for 100 hours? 
so tiny voltage drop thanks for doing the math.
I don't think the fuse on a loopkey is going to be any help if theres a short in the battery still and i haven't heard of an esc breaking into a permanent short.
```

---
## \#31 Posted by: J.Marshall Posted at: 2018-06-06T03:07:03.948Z Reads: 26

```
A 40amp fuse will protect your circuit from any current above 40amps technically speaking. My understanding of fuse ratings is that the rating of the fuse is the minimum current it takes to blow the fuse ... eventually.   When sizing fuses, it is common to select a fuse rated for 125-200% of your normal operating current. It really depends on what current you want to protect against. In our case we would want to protect against a dead short which would result in a huge current draw in the 300-600amp range or maybe more. Taking the 40amp fuse, at 500amps the fuse will blow in 2 hundreths of a second. 

In summary, in order to size a fuse, you really need to understand the dynamics of the system to know the length of time and magnatude of the currents your protecting against. 

But I agree, the fuse will not protect you from any issues with your battery pack. It will only protect the battery wires that go from the fuse to the VECS. I don't think it is a bad idea to have a fuse given all the stories I've read of issues cause by all of the vibrations.
```

---
## \#32 Posted by: Fafu Posted at: 2018-06-06T15:44:32.180Z Reads: 23

```
Ok so this is getting interesting... Do we know from this forum a case where the fuse saved his battery pack and did not die on the event? We will never know i guess haha. My conclusion is, if does not fit to a realistic short scenario, and u risk of blowing the fuse while riding and fly off the longboard,adding the potential tradeoffs on performance.. **then there is no point at all** arguments against? :D
```

---
