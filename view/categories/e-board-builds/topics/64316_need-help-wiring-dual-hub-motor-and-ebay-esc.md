# Need Help Wiring Dual Hub Motor and Ebay ESC

### Replies: 26 Views: 1787

## \#1 Posted by: trinidad Posted at: 2018-08-09T04:46:50.467Z Reads: 127

```
My first build. Just got my motors and esc and the motors come with 5 small wires which i assume connect to the hall sensor connection on the ESC.
But the wires are individually crimped and not in a connector that can just fit into the hall sensor connectors on the ESC. I have no idea what sequence the wires go.

![My%20Snapshot|666x500](upload://xd0MEuCM1VGV28yzys4ABzzXAkV.jpg)![My%20Snapshot_1|666x500](upload://culMuoQKEd01aUG2bERAy06ryvs.jpg)![My%20Snapshot_2|690x388](upload://4rhmuKYdBA0gR6wt2FlZpKDiskx.jpg)

Edit: Board finished just need to go buy a planter box for my enclosure
![My%20Snapshot_3|690x388](upload://77w5nTkXtiMnZOyoETpM67PvvGr.jpg)
```

---
## \#2 Posted by: dareno Posted at: 2018-08-09T05:01:30.366Z Reads: 114

```
Hey mate is that a complete motor and esc package?  I'm only saying because they usually come with connectors attached and are mostly plug and play so someone stuffed up.
If its the sine wave esc then it actually works fine without sensors, just make sure you insulate the wires.  You get a bit more torque too but if you want the sensors to work you need a motor guru like @Hummie
```

---
## \#3 Posted by: Hummie Posted at: 2018-08-09T05:03:46.462Z Reads: 113

```
ive never made a motor with sensors and probably was only on such a thing for max five minutes.  Id cut them off and kick the motor amps way up and forget about it!  to each their own.
```

---
## \#4 Posted by: dareno Posted at: 2018-08-09T05:07:19.729Z Reads: 109

```
:joy::joy:
And I called you a guru and everything.  Let me down man but I'm with you on the whole sensor thing just something else to go fucking wrong!!
```

---
## \#5 Posted by: Hummie Posted at: 2018-08-09T05:15:44.551Z Reads: 103

```
lately im freaked and next board i put together has to be super reliable.  escs are awesome but suck and break.  hoping on the 6.6.   i dont know what happens when sensor wires fail and maybe its not too bad but im feeling really lucky at this point.  even when running two escs if youre hard on the throttle or brake and one esc breaks..im lucky many times now.   i kind of enjoy the challenge..like when the brakes die and im forced to pancake onto a car for a moment, gives me a thrill, but completely other than when that happens its a nightmare.  And then youre freaked and dont trust your stuff.  receivers have sent me with stuck-on throttle...that was one painful event.  and once had my main battery wires break while going down a steep hill with 3 lanes of traffic didnt feel good either.  everything has happend to me at this point i think. I can trust myself to do dangerous stuff, that's skateboarding and electric skateboarding for sure, but when things are out of my control game over.
```

---
## \#6 Posted by: trinidad Posted at: 2018-08-09T05:17:52.865Z Reads: 99

```
nah it wasn't a package I bought them separately. No idea if its a sine wave esc or not. I don't know too much about electronics so I just thought if it has wires it should be connected :stuck_out_tongue: 

 https://www.ebay.com.au/itm/6364-90mm-Dual-Hub-Electric-Skateboard-Longboard-Motors-Drive-Parts-Brushless-AU/152832782374?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2648

https://www.ebay.com.au/itm/Dual-Motors-Electric-Longboard-Skateboard-Controller-w-Remote-ESC-Substitute-AU/282979522572?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649
```

---
## \#7 Posted by: dareno Posted at: 2018-08-09T05:19:51.342Z Reads: 96

```
I think its the difference between eboarders and longboarders.  I would never think of not pushing off to start, its just not in my wiring.  Feels weird standing there and relying on the remote to move me.  I kind of use my board like a snowboarder uses a ski lift.  Its for uphill shit.
```

---
## \#8 Posted by: Hummie Posted at: 2018-08-09T05:20:30.708Z Reads: 91

```
im also cheap.  that's why i give a push.  partially true.  when im not riding powered board like now im pushing the long board around many miles with an empty hole.  its a nice board.  huge.  relaxing.
```

---
## \#9 Posted by: dareno Posted at: 2018-08-09T05:23:17.821Z Reads: 92

```
I would be trying it without sensors and if you get major stuttering from a standstill then work out how to connect them.  I don't personally use sensors at all as they can lock your motor when they go bad and there is too many other things that can do that.  I'm a push start kind of guy.  Saying that all my boards will start from a complete stop just fine and one has that chinese esc thing that looks very similar to yours.
```

---
## \#10 Posted by: trinidad Posted at: 2018-08-09T05:31:07.651Z Reads: 89

```
Awesome cheers for the info will let you know how it works out, pushing to start isn't a problem for me so things should be fine.
```

---
## \#11 Posted by: Silverline Posted at: 2018-08-09T05:52:16.059Z Reads: 83

```
Isn't the sensors just for the startup from stand still. Then why can they lock Up the motor if they fail ?
```

---
## \#12 Posted by: trinidad Posted at: 2018-08-09T06:18:54.757Z Reads: 79

```
Hmmm I've connected up 2x 3s in series for a 6s battery, its completely charged and when I plug it into the esc, the ESC starts beeping and the low battery indicator on the remote is flashing and wheels don't turn. The 6s and 7s pads on the ESC are not connected. Do I need to connect the 6s pads with solder for it to work on 6s?


image is not my ESC but shows a picture of the pads that aren't connected on my ESC 

![s-l1600|374x499](upload://v37TXtI5Iu19CC9Jrtx2gKJfQmQ.jpg)
```

---
## \#13 Posted by: pat.speed Posted at: 2018-08-09T06:44:25.506Z Reads: 77

```
Yes, if no pads are connected it means it’s set for 10s, just connect the 6s pad and you’ll be on your way
```

---
## \#14 Posted by: trinidad Posted at: 2018-08-09T06:45:54.049Z Reads: 77

```
excellent cheers :slight_smile:
```

---
## \#15 Posted by: trinidad Posted at: 2018-08-09T07:32:12.746Z Reads: 80

```
@Hummie @dareno @pat.speed

Cheers for your help guys, you helped me put this together i just need to find some enclosures :smiley:  

![My%20Snapshot_3|690x388](upload://77w5nTkXtiMnZOyoETpM67PvvGr.jpg)
```

---
## \#16 Posted by: pat.speed Posted at: 2018-08-09T07:34:17.329Z Reads: 78

```
I’m guessing your in Aus too by that awol deck. If you can get down to a Bunnings they have some rectangular plant potters that have served me well, and you too until you get another case. I think they were $4
```

---
## \#17 Posted by: trinidad Posted at: 2018-08-09T07:36:19.210Z Reads: 75

```
Yeah I am in Aus, was planning on going down to Bunnings cheers will go straight to the garden section, might wait till Saturday though, sausage sizzle :P
```

---
## \#18 Posted by: pat.speed Posted at: 2018-08-09T07:39:04.822Z Reads: 73

```
Bunnings snags are the best 😋
```

---
## \#19 Posted by: dareno Posted at: 2018-08-09T08:08:22.246Z Reads: 72

```
The hall sensors tell the vesc where the stator is and when one goes it confuses the poor soul and in the case of my HK sk8 very recently it locked it solid. Luckily I was on the flat and ran it off.  I think that if I was travelling a bit more it would have continued to run but I'm not game to test that theory. :expressionless: Disconnected and reprogrammed and haven't noticed the difference at all with the way I ride it so all good.  Still going to squeeze a new one out of hobbyking though lol
```

---
## \#20 Posted by: dareno Posted at: 2018-08-09T08:25:34.574Z Reads: 64

```
@pat.speed @trinidad saturday morning ritual.  always find a reason for a bunnings trip. double saus and onions and wander round the shop dropping it all over the floor.  Just bought a small planter for my vescs because the @TinnieSinker new battery has maxed out my enclosure.  Function over form but hell whatever works while you're waiting for machined version!
```

---
## \#21 Posted by: trinidad Posted at: 2018-08-09T08:45:19.611Z Reads: 59

```
haha the dropping shit all over the floor is so me. I had a Masters down the road from me and when they closed their business they built a Bunnings. I make the most of it when I head down there now :smiley:
```

---
## \#22 Posted by: Silverline Posted at: 2018-08-09T10:12:38.823Z Reads: 57

```
Make nok sence. Because the hall sensors is only used from 0km/h to about 3km/h.... You sure it was not and DRV or FET error ?
```

---
## \#23 Posted by: dareno Posted at: 2018-08-09T10:29:54.255Z Reads: 60

```
  Scenario was riding slowly and motor locked.  Picked up board and left side motor not rotating.  Took back to man shed and plugged in to computer.  Did motor detection on vesc tool and got hall error 255.  Unplugged sensor cable and changed my settings accordingly and now it works fine.  Whether it makes sense or not this was a real world situation that happened to me personally.
  You will find with me my friend that I only comment on things that actually happen to me when I'm riding or building or whatever.  I never pull shit out of my arse because that is misleading and frankly detrimental to anyone reading and needing help.  If you can come up with a different theory then please do as I am far from an expert and always open to advice but my opinion is always based on experience.
In theory is just that......a theory.

Edit @Silverline
```

---
## \#24 Posted by: TheGreekGuy Posted at: 2018-09-07T00:37:15.174Z Reads: 45

```
Hi I got the dual hub motor esc from ebay https://www.ebay.com/itm/123329058317?ViewItem=&item=123329058317 
doesanyone has a wiring diagram or assembly instructions? i am intrested on what connector types are used basicaly
```

---
## \#25 Posted by: goldrabe Posted at: 2018-09-07T02:35:00.355Z Reads: 46

```
Which hubs are you using with it?
Usually the colors of the phase wires are matching the colors from the esc if you got them as a set.
If you want to replace the connectors 3.5mm bullet connectors are standard. Those ESC's don't draw that much amps so 3.5 is fine. Make sure you tape the connectors after wiring the vibrations from riding can wiggle them loose.
```

---
## \#26 Posted by: TheGreekGuy Posted at: 2018-09-07T21:54:52.730Z Reads: 40

```
Hi 
So here is the story and my questions.
I got the ESC from ebay https://www.ebay.com/itm/123329058317?ViewItem=&item=123329058317
I want to use it to drive 2 scooter hub motors (https://www.ebay.com/p/Ninebot-Segway-Es2-Hub-Motor-Assembly-l30/22018623336?iid=332633565806&chn=ps) they are rated 300W with a maximum of 700W. I will drive them with a 36V 10S battery (as nominal) with a future upgrade to 48V (or 54V).

Q1. what do you think about that? I believe it should work
Q2. the hall connectors on the ESC and the motors are different types so I need to make the harnesses for those and with the ESC I didn't got any instructions. what type of connectors are on these boards? JST PH I think but not sure! also there is a 7pin connector that goes to the battery display I guess? 
Q3. the 2 blue capacitors are rated 470uF @ 63V If I get and solder 2 470uF 100V capacitors is this going to upgrade the security of the ESC?

Thank you in advance for all the help that you can give me.
```

---
