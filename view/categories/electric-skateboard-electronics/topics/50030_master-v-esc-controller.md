# Master (V)ESC Controller

### Replies: 57 Views: 1255

## \#1 Posted by: uigiroux Posted at: 2018-03-24T19:37:14.452Z Reads: 184

```
So I think I briefly mentioned this idea the other day, but it was poorly thought out, and I got some time to think about it more and drew up a schematic of things, and hopefully this will be something we can theorize over.

Anway's, I am not a fan of the way we have to connect our VESC's if were going a 2WD, and ESPECIALLY for a 4WD, so I was thinking about better ways we could connect them.

What I've thought of, I basically call a Master (V)ESC Controller.  So assume you are building a 4WD setup.  You connect your battery to all the VESC's, but then you have to connect all the VESC's to one another so they work in sync.  What I talked about the other day was essentially you develop a bit of hardware that has a OS that allows you too designate each VESC to it's corresponding spot.  That's about as far as my mind took me, lol.  That was a bad idea cause I essentially wanted to run all the power through this Master Controller (MC), but that would create a whole bunch of unnecessary issues.  Rather, I thought about it some more today and I wondered if you could just connect your battery to each VESC as you would normally.  Then, setup a 5V UBEC so you can run some extra electronics without blowing them up, lol.  From there, connect the MC, and basically, I imagine something similar to a VESC Tool or similar would be set-up for you to assign each VESC accordingly.  To connect the MC to the VESC's, you would simply connect them all via the "canbus."  So typically when you connect multiple VESC's, you designate one "Master" and the rest the "slave."  What I'm essentially proposing is that this MC be designated as "Master" and all the VESC's be designated as the "slave."  Additionally, from the MC you would also connect your remotes transmitter/receiver so all the VESC's get the signal at the same time from the same source.  It just seems like a must simplier way to control the VESC's in my opinion.  I made a little drawing of this.  It's my first so I am sure I missed a few things, but the overall gist of things can clearly be seen.  So, does anyone this think is something that would be doable, or would it require way too much programming and coding, etc...?

![20180324_141333|384x500](upload://ri1bqzEfVUbi12IIxfJKYFsB59k.jpg)
```

---
## \#2 Posted by: uigiroux Posted at: 2018-03-24T19:45:26.183Z Reads: 159

```
This would work with both 2WD and 4WD since all it would require between the two is having just inputs for each canbus.  For 2WD, just use the rear left and rear right inputs.
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-03-24T20:00:35.339Z Reads: 156

```
I am trying to understand your much "simpler way". You connect a receiver to any of vesc set it as master and use canbus to sync all of them. This is already dead simple. Now you want to introduce another component to do exactly that?
```

---
## \#4 Posted by: b264 Posted at: 2018-03-24T20:00:41.866Z Reads: 152

```
Are you talking about the master VESC controller being a VESC with just the MCU and CAN and a few other components populated on the board?
```

---
## \#5 Posted by: uigiroux Posted at: 2018-03-24T20:05:37.592Z Reads: 141

```
No not a whole seperate VESC, just like some tech that allows you to easily connect to 4 VESC's (this really should just be for 4WD as connecting 2 VESC's is easy as pointed out by @Kug3lis) through the canbus and the remote is connected to this as well, so all the VESC's get the signal at the exact same time and instead of having one master and 3 slaves you could designate front left, front right, rear left, rear right, and maybe that would make the whole traction control thing work better, I dunno.  I just think connecting 4 VESC's the normal way is a hassle is all and I like the idea of them specifically being designated to exactly the position they are at.
```

---
## \#6 Posted by: Ixf Posted at: 2018-03-24T20:10:56.063Z Reads: 122

```
won't a simple 4 way splitter for your remote receiver accomplish that?
```

---
## \#7 Posted by: b264 Posted at: 2018-03-24T20:12:28.419Z Reads: 116

```
Just use 4 receivers.  That way, a failure doesn't bring down your braking ability.  Unless your hand controller fails :stuck_out_tongue:
```

---
## \#8 Posted by: uigiroux Posted at: 2018-03-24T20:14:38.507Z Reads: 112

```
I don't think so.  I've asked about that before and basically was told you are supposed to connect them via the canbus.  easy enough for just 2, but if you have for  then you having to split a bunch...  And what if your master VESC goes out?  All your VESC's would stop working.  If it was set up the way I'm proposing, I think the three other wheels would still keep going, but you would probably notice the difference, so you could stop and check it out, as opposed to getting flung from your board cause they all stopped working.
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-03-24T20:16:13.303Z Reads: 102

```
What if your main controller goes out? You lose all controls :D
```

---
## \#10 Posted by: uigiroux Posted at: 2018-03-24T20:17:08.022Z Reads: 93

```
But that would happen regardless of how you set things up no matter what.
```

---
## \#11 Posted by: b264 Posted at: 2018-03-24T20:17:54.976Z Reads: 89

```
If you wire them so the only wires connecting them are the + and - power wires, there is no main controller to go out.  It's redundancy.
```

---
## \#12 Posted by: uigiroux Posted at: 2018-03-24T20:18:01.165Z Reads: 89

```
Oh you mean the Master Controller?  Yes well that is true.  I guess I'm just thinking that it's such a simple piece of tech that it should be foolproof hopefully..?  lol
```

---
## \#13 Posted by: uigiroux Posted at: 2018-03-24T20:19:16.082Z Reads: 86

```
I'm not suggesting plugging the MC into the main power, just power it off the 5V UBEC and then connect them to the canbus of the VESC.  Where's the redundancy?
```

---
## \#14 Posted by: b264 Posted at: 2018-03-24T20:19:54.924Z Reads: 83

```
What you are describing has none and one failure will bring down everything.
```

---
## \#15 Posted by: uigiroux Posted at: 2018-03-24T20:21:00.807Z Reads: 80

```
Yes but so would the failure of the master VESC.  This is just a way to better manage them IMO.
```

---
## \#16 Posted by: Der6FingerJo Posted at: 2018-03-24T20:21:20.786Z Reads: 80

```
So basically a 1 in x out splitter for PPM and Serial Data for the VESCs? Just use an Arduino for that, it could be done with a bit of coding. But i don't see any immediate benefits over CAN. You're just moving the failure point, not eliminating it.
```

---
## \#17 Posted by: uigiroux Posted at: 2018-03-24T20:24:15.922Z Reads: 77

```
True, but I think the ease of setting things up and potential improvement in any traction control, along with the simplicity of the HW/SW i'm suggesting is more beneficial then just keeping the potential failure point.  I feel like this would be less likely to fail, and as I said, I think it also has some benefits as well, so to me at least it seems worth it.
```

---
## \#18 Posted by: uigiroux Posted at: 2018-03-24T20:25:09.277Z Reads: 78

```
Granted, I can't make anything like this on my own I'd need help, and it doesn't seem like anyone thinks this is a great idea, lol, but I figured it was worth discussing.
```

---
## \#19 Posted by: Kug3lis Posted at: 2018-03-24T20:26:53.596Z Reads: 75

```
I mean I am planning to do this with my boards, to have main control unit but it will not be only splitting signal, but also collecting data, recording to sd/card, communicating with my own remote, telephone maybe some kind of linux board for wifi data sync and etc.
```

---
## \#20 Posted by: uigiroux Posted at: 2018-03-24T20:28:50.143Z Reads: 76

```
Really..?  Are you planning on selling any?  Would this connect the VESC's via canbus as well?
```

---
## \#21 Posted by: Kug3lis Posted at: 2018-03-24T20:33:43.465Z Reads: 65

```
For selling, I don't know it would be too expensive for the general public, as it would have way too much thing for simple people ;) I going to connect each vesc via uart/ppm/usb to the main board. Also there will be usb hub on board so I would only need to plug one usb to the board for BMS, Vesc's and main controller ;)
```

---
## \#22 Posted by: uigiroux Posted at: 2018-03-24T20:34:48.121Z Reads: 62

```
Sounds much more complicated then what I'm thinking of, lol!
```

---
## \#23 Posted by: Kug3lis Posted at: 2018-03-24T20:36:42.662Z Reads: 67

```
Well, I have idea of controlling each motor individually so I could accomplish really tight turns on my eMtb by braking one wheel and spinning another that way I could make decent 90º turns with ease. Of course only on low speed and it also would require CH2 or as I will use my own remote some kind of button/thumb control to make it work.
```

---
## \#24 Posted by: Deckoz Posted at: 2018-03-24T20:46:56.402Z Reads: 67

```
Look if you want a simple solution, setup all of the escs as Masters and slaves.

For example use "multiple esc over can" on every esc, and "send status" on every esc. As well setup ppm on every esc.. hook all esc up to a canbus chain.

For 4wd install a 4 way switch, wire the ppm from each esc to the 4 way switch. If your main master dies switch to a different position. Or setup the 4 way switch as channel 2 on the remote so you can switch masters by remote.

It's already simple....alot of your suggestions seem overcomplicating something simple...
```

---
## \#25 Posted by: uigiroux Posted at: 2018-03-24T20:51:28.274Z Reads: 60

```
What would be a 4 way switch?  Is a canbus chain just 4 of the wires where there all spliced in series?  I don't know that seems like it could fail easily too, plus, the signal is not being received at the same time but each one gets it after the preceeding.  LOL sorry don't mean to over-complicate things, though I know I tend to do that :blush:
```

---
## \#26 Posted by: Deckoz Posted at: 2018-03-24T20:52:23.649Z Reads: 60

```
Canbus is a bus. The escs are wired in parallel. Just like two batteries would be...

You know what a 2 way and 3 way switch are? ..you can get 4 way 5 way and ,6 way switches ...
```

---
## \#27 Posted by: scepterr Posted at: 2018-03-24T20:57:50.148Z Reads: 61

```
From the 4WD Master

[quote="BigBoyToys, post:60, topic:34656"]
4wd CAN: Same as 2wd CAN setting but with additional slaves. All are connected by a daisy chain can harness, and with different CAN ID’s.

It works, but doesnt seem robust. Ive tried 4wd CAN,  4wd split PPM, 4WD communication/tuning via CAN but control via ppm and front CAN with rear CAN connected via PPM. Still seemed to be plauged with random CAN tranceiver failures.  I gave up on CAN and split ppm for 4wd setups. It was suggested that connecting 4 vescs in parallel lowers the resistance on the can bus circuit too much, but I don’t know if this was confirmed. I just run 4 receivers now and havent had a single vesc failure since.
[/quote]
```

---
## \#28 Posted by: uigiroux Posted at: 2018-03-24T20:58:00.788Z Reads: 62

```
I don't know why but I can't think of what you mean by a 4 way switch...?

Canbus would be so much easier for 4WD if they had a canbus in, and canbus out you could plug into, rather then having to splice wires.
```

---
## \#29 Posted by: scepterr Posted at: 2018-03-24T21:01:44.616Z Reads: 60

```
It's just a 1-3 parallel Y splitter
You could make a small PCB with 4 parallel ports that all vesc plug into
```

---
## \#30 Posted by: Kug3lis Posted at: 2018-03-24T21:02:14.801Z Reads: 60

```
He meant to use 1 to 4 output switch so you can select which vesc gets PPM in
```

---
## \#31 Posted by: uigiroux Posted at: 2018-03-24T21:04:17.096Z Reads: 59

```
I like the idea of just using 4 receivers, lol.  Then wouldn't have to connect any of them..
```

---
## \#32 Posted by: uigiroux Posted at: 2018-03-24T21:06:17.894Z Reads: 62

```
http://www.electric-skateboard.builders/t/master-v-esc-controller/50030/29?u=uigiroux

That's an interesting idea... It's essentially what I was thinking of just without any complicated software to potentially fail!

And I could probably figure out a way to connect the receiver to that also...
```

---
## \#33 Posted by: scepterr Posted at: 2018-03-24T21:07:37.000Z Reads: 55

```
Yeah...there's really nothing to do..4wd can works as-is, you can have fwd and rwd traction control even
```

---
## \#34 Posted by: uigiroux Posted at: 2018-03-24T21:09:32.372Z Reads: 56

```
To do that would I keep the front and rear VESC's separate?

Would that be better than left side and right side traction control?
```

---
## \#35 Posted by: scepterr Posted at: 2018-03-24T21:12:06.691Z Reads: 55

```
You would still have left/right just independent front/rear too
The vescs can be physically anywhere
```

---
## \#36 Posted by: uigiroux Posted at: 2018-03-24T21:16:12.006Z Reads: 56

```
Ok..  Man I'm so ready to get my build going.  The one thing I just not super confident about is properly setting up my VESC's, and since I'm getting 4 ESCape's, I really don't want to risk frying one of those beauty's...
```

---
## \#37 Posted by: scepterr Posted at: 2018-03-24T21:23:42.740Z Reads: 58

```
Gotta pop that cherry one day 

https://giphy.com/gifs/ui1hpJSyBDWlG?utm_source=media-link&utm_medium=landing&utm_campaign=Media%20Links&utm_term=
```

---
## \#38 Posted by: deucesdown Posted at: 2018-03-24T23:18:14.531Z Reads: 55

```
If you look at quadcopters typically there's an esc for each motor, and a flight controller sends control signals to them via digital protocol.

The interesting idea being the brainbox and dumb escs talking via some protocol.
```

---
## \#39 Posted by: Deckoz Posted at: 2018-03-24T23:28:49.978Z Reads: 56

```
See..

That works for quadcopters because the flight controller is centralized has a gyroscope and is sending signals to each esc to keep it stabilized at x angle. So it can fly. They are synchronous based on the gyroscope. In skateboards there is no gyroscope. But traction of all four wheels

Then benefits of having a "brain" are already implemented into the vesc, canbus allows the 2 wire communication, and provides the traction control. Any vesc can be the brain. If we are asking for a smarter traction control, where canbus IDs = motor corner location. You could implement torque vectoring. But again, each vesc Is already a brain in it's own right. I setup all my vesc as Masters and slaves, if something ever arises in the field, just swap ppm or uart pins and keep riding.
```

---
## \#40 Posted by: wolffoxx Posted at: 2018-03-24T23:41:52.478Z Reads: 56

```
I have a 4WD with 4 Vescs, and I use this to split the remote signal:

![IMG_0570|375x500](upload://eo4krFz1kYNxYOQf6mfcuPJuM5Q.jpg)

That has been very reliable.  I've not messed with telemetry so far, but I'm planning on putting an HM-10 on every VESC, as well.  That might be overkill, but I never had any luck with the CAN back when I was trying.
```

---
## \#41 Posted by: deucesdown Posted at: 2018-03-25T01:27:16.461Z Reads: 50

```
I hear what you're saying, but I can see benefits of splitting it up the control from the escs.

- lower unit cost per esc (and per motor)
- one receiver, no debate about split ppm or self frying canbus (especially with 3 or more vesc?)
- with one brain, easier to get logging/telemetry
- again, with one brain, there's one source of truth for things like brake lights
- less chance to fumble finger and put different configs on control units

I'm leaving traction control out of this, as at least with canbus, I've not liked it at all. if one vesc is cogging, the other one stops hard, etc.

Oh and I'm just thinking out loud, not really advocating anything.
```

---
## \#42 Posted by: Kug3lis Posted at: 2018-03-25T01:31:02.913Z Reads: 49

```
You talking about running all 4 motors from single MCU? Because VESC MCU spends 90% of time working on controlling motor and just fraction of checking can/ppm/uart/usb.

So there is not much way to split control from VESC to single mcu
```

---
## \#43 Posted by: uigiroux Posted at: 2018-03-25T01:51:04.975Z Reads: 47

```
Does this mean you agree with me?  Lol
```

---
## \#44 Posted by: deucesdown Posted at: 2018-03-25T01:52:38.242Z Reads: 48

```
I think the "dumb" escs for quads have an MCU, after all they talk to the flight controller via some control protocol (newer ones use a digital protocol). So it's like the motor control is offloaded to the escs.

So the "master" MCU decides what to do, and the "dumb" MCUs on the ESCs execute the commands.

[quote="uigiroux, post:43, topic:50030, full:true"]
Does this mean you agree with me?  Lol
[/quote]

Lol I'm not sure if I agree with you. But I think it's an idea with merit, and probably not for the BV vesc. Are you gonna make it happen? ;)

EDIT I think dshot is the popular FC -> ESC digital protocol. From a 30 second read, it seems like a 11 bit throttle value with a 4 bit checksum. Not bidirectional, and not that fancy.

https://www.rcgroups.com/forums/showthread.php?2756129-Dshot-testing-a-new-digital-parallel-ESC-throttle-signal
```

---
## \#45 Posted by: deucesdown Posted at: 2018-03-25T02:05:51.339Z Reads: 45

```
Okay this got my brain going a little.

I'm not familiar with the space, but 30A dshot ESCs seem to be around $15. 4 x 30a is 120a, so I guess that's plenty for typical use.

VESC is 50A so the power section would have to scale up, but the control section would probably remain the same? The quads are running way higher KV motors, so I'd guess they have much higher sampling rates, etc?

If the ESCs are separate from the brains, there's less risk of one of the common failure modes of VESC -- something like frying the DRV chip.

Eh, I like the idea of this more and more.
```

---
## \#46 Posted by: uigiroux Posted at: 2018-03-25T02:54:57.595Z Reads: 41

```
How would I go about doing this if I don't know anything about programming or circuit boards...  I'd love to be in on the development, but I'm probably not the one to head this project...  I think it would greatly simplify things especially for 4WD, and reduce esc failures.
```

---
## \#47 Posted by: Sender Posted at: 2018-03-25T03:21:14.709Z Reads: 43

```
@uigiroux no offense, but why are you making multiple topics everyday...?  Most of the things you make NEW topics about are covered somewhere (there is tons of stuff on board security, one of your new topics from yesterday for example).

Might I suggest starting a build thread so you can put these thoughts there instead of spamming new topics?  I mean I know its exciting and all, but you don't need to recreate the wheel quite yet... 

Once again, not to offend, but it is a little annoying.  Maybe just try a different tactic. Like finding a similar thread and posting your thoughts/ideas there.  The more new redundant topics we have the more all this knowledge and insight gets spread out and difficult to search.

I dunno, maybe I am just in a bad mood.
```

---
## \#48 Posted by: uigiroux Posted at: 2018-03-25T03:30:48.835Z Reads: 45

```
Ok well I guess the board security one I could have added to another thread, but I think I've made I'm total over the past year less then 20 posts.  I don't know what thread I could have added this too so I think this one is fine, and aside from the board security one, the last topic I made was a hub motor in a pneumatic tire, which I didn't see any when I made the thread.  I do typically look first before adding a new topic.  Sorry about the board security if that upset you... but as for the majority of my new posts I think I have been good about either adding too an existing topic, and if one can't be found then I'll make a new post.

As for making a build thread I think that would be pointless, mainly because I still waiting on the things I've ordered so I can hardly start one of those, and a lot of the times, a topic I bring up would have nothing to do with a build thread, but more to do with learning about certain things that I didn't find a sufficient answer in the current threads when searched.

Also, a thread should have one topic to be discussed.  If I was to make a thread and just start throwing new topics in there it would be very confusing and I'd probably have an admin come and tell me to stay on topic.  So I don't know what is so annoying about this, as it's a place for learning.   I'll be sure to be extra vigilant in the future and make sure only to post new topics if not a single thing else can be found, if that will make you happy... :wink:
```

---
## \#49 Posted by: Sender Posted at: 2018-03-25T03:42:23.366Z Reads: 40

```
Like I said, I am probably just in a bad mood because  I am sick.... you do you.  But you did just put up 4 debatably not necessary topics in 2 days.  Just wanted to point out there maybe other ways to research/discuss something than putting up a new topic.  I have learned on here that I am hardly ever in a position to where I need to create a new topic for something... especially 4 in two days thatare pretty meh...  sorry tgisis dickish, just wanted to point it out 👬
```

---
## \#50 Posted by: pakue Posted at: 2018-03-25T03:46:46.762Z Reads: 40

```
Has anyone tried getting rid of R401 for 4WD builds on the VESC? The CAN network is usually terminated with 120 Ohm resistors. On the VESC schematic CANH and CANL are already connected with 100 Ohm so for a 2WD it's therefore to spec, but 4WD has now 2 resistors too many.
```

---
## \#51 Posted by: uigiroux Posted at: 2018-03-25T11:39:50.196Z Reads: 38

```
Ok well maybe next time you want to point something like this out it would be more appropriate to PM someone instead of changing the forum topic and disrupting discussion.

Also, just because you say 'not to be a dick' doesn't mean you can then go ahead and be a dick.  You made the issue known, I acknowledged it, the end.  You don't need to keep posting or in the last case,  adding a huge edit to one of your posts.
```

---
## \#52 Posted by: Nordle Posted at: 2018-03-25T12:45:33.489Z Reads: 36

```
But @sender is totally right... you should read much much more before trying to reinvent the wheel...
In hummies thread 4example you ask for hall sensors and 3 posts later you dont know even what they do-.-
```

---
## \#53 Posted by: Sender Posted at: 2018-03-25T12:57:31.779Z Reads: 36

```
Sorry for the edit, I was drunkish and it was literally littered with typos.... well, still is TBH. Sent you a PM. Also, sorry for the derail gents.
```

---
## \#54 Posted by: uigiroux Posted at: 2018-03-25T14:21:14.415Z Reads: 35

```
Ok, I have heard the issue raised.  I will take it into consideration now before I make any new threads.  Can we move the discussion back to the topic at hand?
```

---
## \#55 Posted by: trampa Posted at: 2018-03-25T18:07:52.110Z Reads: 30

```
The first VESC Six design Benjamin made had two CAN bus ports, so that you could have plugged in two cables, forwarding the CAN signal to the next VESC. We skipped that design, since you don't really need that feature in reality. Soldering an external parallel Y-Splitter for CAN is simple enough.... 

A brain, controlling all the attached ESCs is somehow nonsense for this kind of application, since each VESC is a brain already. The MCU is needed on each device anyway and it has plenty computational resources left to handle some other tasks in addition. This is why there is an App section in the software.

On a 4WD you have 4brains already, why implement a 5ths? If that device fails, you would be struggling to get home. If the master ESC fails, you could simply re-configure another ESC to be master and ride home on 3 driven wheels. If you build your board in a way, so that you can plug in your receiver into one of the other devices you will have fall back strategy. 

If the Hardware is made to a nice spec, it usually doesn't fail during a ride and there is no problem that needs to be addressed by making things more complicated than needed. The likelihood that your 5ths brain fails is as high as the likelihood that your master ESC fails.
```

---
## \#56 Posted by: Sender Posted at: 2018-03-25T18:18:01.519Z Reads: 31

```
![20180325_131739|398x500](upload://ymyCNAmfTL79EZCIfG8pyZ8ZuTq.jpg)
```

---
## \#57 Posted by: uigiroux Posted at: 2018-03-25T18:20:47.337Z Reads: 30

```
Love is a beautiful thing...
```

---
