# Do I need 2 anti spark switches?

### Replies: 13 Views: 433

## \#1 Posted by: B_in_tha_OZ Posted at: 2019-03-26T12:15:17.508Z Reads: 153

```
Please forgive my ignorance if this is a stupid question but I'm still pretty new and on my first rebuild. I've searched everywhere and can't find anything on any of the other topics

I have 2 flipsky vesc's each running a motor connected via can bus with 2 X 7s3p Li-ion batteries. The original plan was each battery would feed a single vesc/motor. The batteries are rated 24v at 40A continuous working load 60A peak. My question is if I want each vesc to put up to 30A into the motors do I need each battery to have its own anti spark switches and keep them totally seperate? Or can I connect the batteries through a parallel connector, through a single anti spark switch then split them again to go to the vesc's? Or will that drop the usable amps I can get to each vesc/motor? Sorry for the noob question
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-26T12:21:58.839Z Reads: 148

```
If you want to have a separate battery for each vesc you need two anti spark switches.
If no, than just wire the packs in parallel and split them up after the switch than.
All current run than through the switch but divided through the parallel packs.
```

---
## \#3 Posted by: B_in_tha_OZ Posted at: 2019-03-26T13:16:01.401Z Reads: 125

```
How does it effect the amps I can get to the motors though? If I join them can I still get 30 amps continuous to each motor safely (in regard to the batteries each is rated to 40A continuous output). Or will it mean it mean I will only be able to get 20A continuous to each max workable? Sorry For the dumb question i'm just not sure fully how amps work, if they split or stay the same down each cable when split
```

---
## \#4 Posted by: danielz Posted at: 2019-03-26T13:30:33.847Z Reads: 105

```
2 parallel will provide the same current as having one battery connected to each motor. If you want even more current, the batteries to be less stressed or longer range, connect even more in parallel.
```

---
## \#5 Posted by: Andy87 Posted at: 2019-03-26T13:32:59.242Z Reads: 97

```
what @danielz :point_up: said
```

---
## \#6 Posted by: B_in_tha_OZ Posted at: 2019-03-26T13:34:25.184Z Reads: 87

```
Thanks @danielz that helps a lot. That means it won't negatively effect the current to motors if I pass both batteries through the same switch. Thanks guys been a massive help and save me money and work 🤙
```

---
## \#7 Posted by: Eboosted Posted at: 2019-03-26T14:12:51.855Z Reads: 72

```
Why have you wire two batteries one for each vesc? You will need two switches, you won't be able to sync botch VESCs for each motor, you won't be able to use traction control, you will not be able to keep both batteries at the same level, you won't be able to make telemetry unless you buy two dongles, you will have to charge 2 batteries with two chargers

It's just a bad idea
```

---
## \#9 Posted by: L3chef Posted at: 2019-03-26T14:52:23.613Z Reads: 64

```
[quote="Eboosted, post:7, topic:88358"]
you won’t be able to sync botch VESCs for each motor,
[/quote]

Are you sure about that? With CAN connected you should be able to sync 2 or more motors even tho you have a seperate battery. Right?
```

---
## \#10 Posted by: linsus Posted at: 2019-03-26T14:54:41.835Z Reads: 60

```
Pretty sure its just misscommunication here.

TL:DR

Original question: 
Can I put my batteries in parallell to feed both VESC or will something bad happen? Will I need one or two anti sparks?

Answer:
Yes, you can parallell your batteries and have one antispark, given everything is wired correctly and aslong as the antispark can handle your top current(which I assume is 120A in this case)
```

---
## \#11 Posted by: olestra Posted at: 2019-03-26T16:09:18.576Z Reads: 51

```
It's really bad idea to connect even data lines across separate systems when they don't have a common ground.

if you wanted to make the separate batteries for each vesc work, you would need to connect the negative of each battery together -- that would _mostly_ solve the floating ground issue. Then you would need to tie the negative off of each ESC that goes to the receiver, to get the 5v common ground. 

Of course this only will work as long as you don't get any transient voltage spikes that cause one side or the other to drift too far apart in voltage... 

Then you're only left with the problem of one battery draining before the other (one motor more efficient, more/ less drag on one side or route has more left or right turns).

I don't think it's worth the effort to separate the power per drive system, even though the advantage of being able to continue with one side inoperable is really seductive
```

---
## \#12 Posted by: L3chef Posted at: 2019-03-26T17:01:12.646Z Reads: 41

```
Thanks, I can see the problem with seperate battery packs now
```

---
## \#13 Posted by: B_in_tha_OZ Posted at: 2019-03-26T22:42:00.281Z Reads: 30

```
Good thing I'll be running them parallel now with one flysky 280A anti spark switch then, thanks to all the info you guys have given me. The only reason I was thinking to run one battery each was because I didn't know how amps work I thought it may devide the amps in half so I would only get 15-20 amps to each motor but thanks to you all, you cleared that up for me, thank you 😁🤙
```

---
## \#14 Posted by: Eboosted Posted at: 2019-03-27T02:59:07.334Z Reads: 22

```
Maximum current will be restricted on the ESC programming
```

---
