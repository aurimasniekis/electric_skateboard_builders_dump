# Custom VESC for drop-in replacement of Onan ESC (Any interest?)

### Replies: 44 Views: 494

## \#1 Posted by: bluegreen Posted at: 2019-05-10T21:25:15.709Z Reads: 130

```
How many of you out there have an Onan or Nuff booster? And of that group, how many are interested in modding the ESC?

I am considering having a go at taking the VESC 4.12 hardware design and fitting it to a PCB that will be a direct drop-in replacement for the ESC that comes from the factory.

This is interesting to myself as a project for the following reasons:
* Learn about designing BLDC medium voltage PCB topology.
* First time designing a 4 layer board
* Fist time using KiCad (used eagle for 6 years)

If it worked, it might be economical to have a few or maybe a dozen completed ESC made. I have no idea what they would cost, but maybe $150 to $200 which includes dual vesc and antispark.

The open end for me right now would be to decide on an anti-spark design as this seems to be an area of much contention. So maybe if anyone thinks this is of interest could recommend an anti-spark design to use with this project, thanks!
```

---
## \#2 Posted by: RedBaron Posted at: 2019-05-11T04:40:53.881Z Reads: 117

```
We could always use more options and creativity!
```

---
## \#3 Posted by: mynamesmatt Posted at: 2019-05-11T06:20:39.128Z Reads: 108

```
@City-Blade-101 this sounds like you!
```

---
## \#4 Posted by: City-Blade-101 Posted at: 2019-05-11T10:09:54.319Z Reads: 87

```
Yeah Matt, thats right. ATm the mini v-esc x could be the only not onan esc that will fit on dual setup with the onan booster, because of space and this would be a nice option for a change,
```

---
## \#5 Posted by: City-Blade-101 Posted at: 2019-05-11T10:12:50.134Z Reads: 84

```
Im in when it works and when the mod beats the original new Foc mode  onan x2 esc ( what could be very hard, because the new onan escs are b pretty good)
```

---
## \#6 Posted by: bluegreen Posted at: 2019-05-11T10:14:44.312Z Reads: 83

```
This would be most interesting to me if I could get a bunch of blank enclosures super cheap. That way could sell the enclosure and customer can buy their own motors/hubs and just order onan batteries.

Has anyone ever talked to customer support or anyone at onan? I have sent a few emails no responses.
```

---
## \#7 Posted by: City-Blade-101 Posted at: 2019-05-11T10:15:21.989Z Reads: 73

```
![20190510_130208|690x388](upload://nE36z498J84HeAF6BMo2sGbnZQQ.jpeg) 

mock up of two mini v- esc in an onan.
```

---
## \#8 Posted by: City-Blade-101 Posted at: 2019-05-11T10:17:38.204Z Reads: 70

```
yeah its not easy to get in touch with someone at onan. Maybe try out from alibaba platform, because sellers will lead you to the onan labs if you ask for it.
```

---
## \#9 Posted by: bluegreen Posted at: 2019-05-11T10:17:52.444Z Reads: 66

```
Then again I'm not sure I really want to support these so much. I hate that you can't get to the charge port while it is installed.

Actually, if you've got the x2 or 3, and want to rewire them, it would be possible to split the plug, so 2 prongs are charging and 2 are for power. Then put a barrel connector on the enclosure.
```

---
## \#10 Posted by: City-Blade-101 Posted at: 2019-05-11T10:22:20.038Z Reads: 59

```
chargeport never were an issue to me, but for many people it is.
Dont understand the second part. which plug you want to split?
edit: ahh i got it, you mean so you have two charge ports, one underneath like the original and a second one from were you can charge without taking the battery off, right?
```

---
## \#11 Posted by: bluegreen Posted at: 2019-05-11T10:30:44.396Z Reads: 52

```
The battery<->esc connection has 4 pins, 2 in paralel. You could split them so that you can pass the charge connector through the internal connector... and then add a barrel jack to the esc enclosure. That way you could charge it while it was plugged in.
```

---
## \#12 Posted by: City-Blade-101 Posted at: 2019-05-11T10:33:54.046Z Reads: 50

```
ah okey,but not necessary for me, because you can swap batteries that easy and i always got some extra batteries with me. But nice idea anyways
```

---
## \#13 Posted by: bluegreen Posted at: 2019-05-11T10:34:42.306Z Reads: 51

```
Would make life easier just popping a dc jack in instead of having to wrestle the damn battery out getting hands all dirty.
```

---
## \#14 Posted by: City-Blade-101 Posted at: 2019-05-11T10:35:09.332Z Reads: 52

```
I like it dirty hahahahahaha
why wrestle? don't glue the batteries in the enclosure man hahahahaha
```

---
## \#15 Posted by: City-Blade-101 Posted at: 2019-05-11T10:39:05.278Z Reads: 49

```
What do you think about the mini v-esc (foc) for dual setup in the enclosure.
For me best choice atm and enough space at all. Good to go imo because they do FOC like the new onans, and performance on them is pretty cool.
```

---
## \#16 Posted by: bluegreen Posted at: 2019-05-11T10:43:24.555Z Reads: 53

```
With the same hubs or different? I'm not sure what is worth it for the stock hubs really. X2 probably better. I think its important to keep it cheap for this build unless you plan on putting some real high power motors there. I think 2 vesc 4.12 would fit if you stack the capacitors on top or maybe in between. Would be tight.

If I knew how to use KiCad like I do eagle it wouldn't take me much time at all to move the parts around. The advantage to doing it this way is that you can use the heatsink the same way as the stock pcb.

But... again at these power levels, doesn't matter. Using the heatsink like that would be good if you want to run more power, but then, the battery can't really put out too much anyways.

The main reason I want to do this is because the ramp rate on the controller is so dumb, and I don't have FOC so it's quite loud.

Probably better to just leave it alone and ride it into the ground, get a cooler board.
```

---
## \#17 Posted by: City-Blade-101 Posted at: 2019-05-11T10:55:50.556Z Reads: 42

```
im talking about X2...X3 motors are to small and weak.
Don't know the problems anyone has with these hubs, im totally happy with them.
In 4WD after treating them hard they don't even get warm, and im talking about steep hills up and down all the time in my area(like SF). Always hitting the sidewalks hard and never had any issues like loosing magnets or something.
It would be great to be able to change between motors with another esc( i heard onan is not open source) and i would try that. The battery would need another hack for more power, switching the cells to 30Q instead of 22P would be much betters i guess.
@faust got a 10s3p configuration in one battery pack...
I got an idea: It would be nice, if we were able to use a second battery pack (via serial connection i think it must be) with only a 2WD onan X2. So theres more power and more range and with maybe fausts battery hack you got 60 cells underneath.
You know what im talking about? there only has to be a connection method between the packs, and another add on enclosure to fix the second one, WHOOOOHOOO!
```

---
## \#18 Posted by: Mazda_bater Posted at: 2019-05-11T12:01:11.299Z Reads: 41

```
I had Onan esc issues and managed to squeeze a fsesc 4.2 dual in there
```

---
## \#19 Posted by: City-Blade-101 Posted at: 2019-05-11T12:20:39.409Z Reads: 39

```
great, do you have taken any pictures you can show up here and maybe a video running them motors on them flipskys?
```

---
## \#20 Posted by: Mazda_bater Posted at: 2019-05-11T19:30:21.477Z Reads: 40

```
![IMG_2633|375x500](upload://sR2b5GWU7yveXnFmKYUW8L6CBSs.jpeg) I took a little video it cogs a bit because I've set it up unsensored after just doing the resistor swap on the fsesc not sure how to add a vid to the forum though. No room for a power switch it turns on when I connect a battery and off when I disconnect.
```

---
## \#21 Posted by: City-Blade-101 Posted at: 2019-05-11T22:02:23.473Z Reads: 35

```
hahahaha...i meant a photo from the inside of the enclosure to see how you managed to fit in a dual flip sky esc hahahahahah but thank you anyways...vids you can upload to youtube and then put the link in here.
And yeah, the powerswitch is a problem with such a big esc, for that reason i think two mini v-esc are the better choice, so you can leave the powerswitch where it is or move it to the side of the booster. Thats what i will do if space is a problem with the minis, but i think it will all fit perfect. I can't swap resistors or things like that, because this means high math to me and im not able to change them with my crappy knowledge obout pcbs and stuff like that.
```

---
## \#22 Posted by: bluegreen Posted at: 2019-05-11T22:07:46.114Z Reads: 33

```
Does X2/X3 have the problem of the remote throttle delay? I push full throttle it takes like a full 6 seconds to actually give full power.

I almost wish I would have got the x2/3 for $500 but I got my x1 for $229 complete with the deck so kinda hard to say. No sensors means I can't push from a start but after building my own board and riding it for a while, I realize that is saving a lot of battery power. FOC would be nice so it's not so loud. Mine sounds like a powerdrill sometimes!

Maybe I will travel to china and meet with onan to convince them to make a dual vesc and 30Q setup and it will actually be quite nice.
```

---
## \#23 Posted by: City-Blade-101 Posted at: 2019-05-11T22:15:55.963Z Reads: 34

```
I got dual X2 in bldc and 4WD in foc and the remote works perfect for both of them.Never had any issues or delay or something. Maybe its because you have the earliest model of the x1. I bet this is the reason because Onan did lots of updates on their esc and remotes so far.
I bought an X3 for my sisters 14 year old son and even this model works pretty well for him(he is a lightweight).No remote issues, nothing.
I would not recommend an X1 or X3 for people above 50kg, because then its too weak. But its esc got damaged by water, because the plastics underneath the electrics had cracked because of vibration and deep concave of the deck, so there got a little bit water in there. Shit happens, but i will change the esc and all should be fine again.
```

---
## \#24 Posted by: bluegreen Posted at: 2019-05-11T22:33:48.502Z Reads: 33

```
Ya my plastic cover cracked too.

Its weird the pcb has a place to attach sensor motors on mine, so it's like they were planning on adding the feature later.
```

---
## \#25 Posted by: City-Blade-101 Posted at: 2019-05-11T23:11:42.603Z Reads: 33

```
yeah, the x2 and x3 models i own are censored.Seems like you got an old dinosaur at hand:joy:
I attached some foam rubber on the plastics and underpinned the concave of the deck with it, since then everything is fine.
```

---
## \#26 Posted by: Mazda_bater Posted at: 2019-05-12T12:40:05.483Z Reads: 33

```
![IMG_2634|666x500](upload://rmyreKmySiXFWCU0Fx0IussAcJZ.jpeg) ![IMG_2635|666x500](upload://lBOUwvoPDoJPAqV4man5bJ4lLa6.jpeg)
```

---
## \#27 Posted by: Mazda_bater Posted at: 2019-05-12T12:42:56.090Z Reads: 30

```
You can likely see that I removed 2 screw posts. I didn't want to waste too much time manually machining the enclosure to fit the vesc I also wanted to be able to screw the old speed controller in if I can work out what's wrong. I just drilled them from the top Of the post down
```

---
## \#28 Posted by: City-Blade-101 Posted at: 2019-05-12T16:06:05.640Z Reads: 29

```
Awesome, cannot believe that it fits. I measured the case and even with drilling the screw posts i couldn't get the flip sky dual in there( using a mock up flip sky i cut out from paper)...were you able to add more power to the motors for more top speed?
Edit: Why do you want to replace the flip sky again with the original esc? Was it better with the original or what is the reason? Because I want to change them to add a bit more power to my dual Onan drive using the vesc tool.
```

---
## \#29 Posted by: Mazda_bater Posted at: 2019-05-12T18:56:29.783Z Reads: 24

```
I actually found it quite good on the original esc and remote. I only changed to the flipsky because I lost confidence that I could order replacement parts for the Onan and have a reliable setup,
This vesc hasn't been without its issues it would cut out over a certain motor amp level. It's working well now after doing a repair and certainly has more power. Running in sensored foc is great
```

---
## \#30 Posted by: City-Blade-101 Posted at: 2019-05-12T18:59:53.759Z Reads: 21

```
you mean the original onan esc has cutouts or the flip sky? sorry im a bit confused because my dual x2 on sensored bldc shuts down when going up to steep hills.
The 4WD X2 is sensored, too and in foc which is amazing-climbing every hill full speed without getting the motors hot.
I was totally happy at first with my dual but now, if you say its better with flip sky or another esc like the mini v-esc i want to try, then i will do the same. which remote do you use now?
```

---
## \#31 Posted by: bluegreen Posted at: 2019-05-12T19:14:53.029Z Reads: 22

```
I'm afraid the shutdown is actually the battery controller shutting down on max amps so changing the controller might not even fix it youd have to change the BMS too.
```

---
## \#32 Posted by: City-Blade-101 Posted at: 2019-05-12T19:17:29.049Z Reads: 21

```
Ah okey thank you. if im doing the battery mod one day i will skip the bms anyways to get more cells in there, but this is future time project. At first i would be happy if everything is fixed and it performs the way it did before, because i got some more Onan boosters at hand, but this one is from my sisters son.Still waiting on parts from china. If you need a the email address of my seller i will send it to you. From there you can get any part for the onan you need
```

---
## \#33 Posted by: Mazda_bater Posted at: 2019-05-12T20:02:42.813Z Reads: 21

```
The fsesc dual 4.2 had a known issue with cutouts, this has been solved recently and corrected at a manufacturing level.
My ivoryboards. Is a bldc model and it would cog from a standstill changing to a configurable speed controller where I could set up sensored foc was an amazing change. I tested these motors at 50 motor amps and it dragged my fat ass up a decent incline.
I was using the original ivory(Onan)setup and one day randomly I turned the board off and when I went to turn it back on to use it, it wouldn't pair.
I struggled to get in touch with the manufacturer to order gear so went with the flipsky. By rights after going to a separate speed controller and remote receiver setup I've never had a connection issue and I've always had the board running
```

---
## \#34 Posted by: City-Blade-101 Posted at: 2019-05-12T20:12:16.750Z Reads: 22

```
mhhh, i will think about my plans again. maybe use the original esc for the kids booster.
don't want to do experiments on the neck of the boy. Will order the onan esc right now:laughing: he has got the X3 booster and the main units are available atm...
Like i mentioned before i never ever had any connection issues or something and i bought 7 boosters last year. Two x2 4WDs in FOC(which is 4 boosters), Two x2 Dual in bldc and one x3 in bldc. All of them are pretty fine except the mainboard of the x3 now.

Go for a X2 4WD  and you will see how much power is into them.I have seen them these days on alibaba for under 700 dollars complete with 2 chargers, 2 remotes, 2 battery packs and a deck. And you are from australia, so shipping should be under 150 dollars.
```

---
## \#35 Posted by: Mazda_bater Posted at: 2019-05-12T22:31:24.758Z Reads: 17

```
![IMG_2638|375x500](upload://mzpjff1J0c9hosXTQkFogQoWms4.jpeg) this is the way the enclosure looks sorry it was 4 posts
```

---
## \#36 Posted by: bluegreen Posted at: 2019-05-12T22:42:12.290Z Reads: 17

```
Lol one of my battery packs stops charging at 40 volts, so I'm probably looking at building a new pack. But it's the high capacity pack that is actually dead, so maybe I should make 2 10s2p 30q packs...
```

---
## \#37 Posted by: City-Blade-101 Posted at: 2019-05-13T01:03:42.118Z Reads: 18

```
At first I have to THANK YOU! for disassembling your board on my request.
That means a lot for me and again THANK YOU for that.

Edit: Yeah nicely done, I thought about the same enclosure mod by removing some parts which could change or are even irrelevant on this future fantasy project.
Most important for me is to keep the power switch where it is if it is possible, therefor I still have an eye on the minivescs, but I got lots of time with that, because Onan , believe it or not, still ROCKS!
About Foc mode on Onan you are totally right is more than awesome(doesn't matter if flip sky esc or original onan esc i guess)...the motors are super mega smooth while accelerating with kind of dynamic power transmission which makes this machine a true weapon.I love that. 
The only weakness of onan drives imo is the aluminium motor wheel inner part, where the slots are which were designed for air-cooling.This skeletal designs leads to weakness because they are very soft and will break soon by hitting the sidewalk sometimes(i always hit the sidewalk hahahah. But I got an idea about solving this issue...
@bluegreen  sorry for going so much out of topic. I am still interested in another esc option that would fit:grinning:
```

---
## \#38 Posted by: City-Blade-101 Posted at: 2019-05-13T01:08:00.193Z Reads: 16

```
I thought about something (don't laugh) similar to n.e.s.e(don't know the name, its an italian guy) or @Winfly modules to easily put into those original onan battery enclosures.
This way we are able to change capacity(which could be very flight friendly in separated mentioned modules)and we have access to every single cell at all time....
Sorry I can't live without edit! 
What also would be fantastic if we could choose between different wheel diameter! Ive seen some guys on here doing own HUB-SLEEVE-WHEELS! I think @visnu777 is one guy who is able to do things like that, because he is in practice with that hub sleeves.
```

---
## \#39 Posted by: bluegreen Posted at: 2019-05-13T01:49:25.578Z Reads: 17

```
Eh, the more I think about it as soon as you solve one problem there are so many more.

Thing I like the most is the deck and the weight balance, but I guess I could do that with another setup too.

Bummed out about the battery. I'll tear it apart, I'm really hoping I can revive the cell, I'm not sure it's worth trying to match the cells that are in there and replace it with a new one.
```

---
## \#40 Posted by: City-Blade-101 Posted at: 2019-05-13T01:59:16.565Z Reads: 17

```
Yeah good idea trying to switch the cells to 30Q.
Was planning the same but im not sure yet.
I got another idea to work out atm and must think about that a bit more.:cowboy_hat_face:
```

---
## \#41 Posted by: City-Blade-101 Posted at: 2019-05-13T02:00:51.979Z Reads: 17

```
yeah, hopefully its ok highjacking your own thread:joy::joy::joy:
```

---
## \#42 Posted by: bluegreen Posted at: 2019-05-13T02:24:52.665Z Reads: 15

```
I think if you are happy with your ESC, rebuilding a pack to 30Q if you already have several, I think that makes sense.

This X1 is a junker. For 229, if you lived somewhere totally flat and wanted to ride it on bike paths to the grocery store or give it to your nephew or something like that it's OK.

But it sounds like X2 doesn't have the problems with the throttle or sound like X1 does, so. No real point.
```

---
## \#43 Posted by: City-Blade-101 Posted at: 2019-05-13T02:26:28.760Z Reads: 14

```
yeah because one battery pack lost me already( it was a pretty old one) and im forced to do something.
You can't compare the x1 with the x2 and you can't compare it with new x2 foc and 4WD.
its another galaxy it is as powerful as evolve gtx. Battery may be may be not.
for 700 bucks.
```

---
## \#44 Posted by: Mazda_bater Posted at: 2019-05-13T21:04:48.825Z Reads: 14

```
I’ve had a battery issue related to a broken wire in the pack
```

---
