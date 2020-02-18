# I Submarined my esk8

### Replies: 17 Views: 1009

## \#1 Posted by: ThermalM16 Posted at: 2018-03-20T00:22:48.343Z Reads: 270

```
So I was headed home from class and it started to downpour. I figured my board would be fine since I conformal coated my FOCBOXes and had a foam neoprene seal around my enclosure. Turns out the neoprene seal around the enclosure didn't help all that much. 

The trip from my apartment to class is about 1 mile. I was probably about 3/4 of the way home when my board began to feel sluggish. I let off the throttle immediately and picked the board up only to be greeted with a small waterfall pouring out of my enclosure. The first thing I did was turn my board off to prevent any further damage. One thing to keep in mind is if your antispark switch is shorted, or if water found its way into the switch on your board, it will not turn off until you disconnect the battery. Fortunately, my antispark switch wasn't shorted from the water and my board actually turned off.

My board is sitting on my floor in pieces at the moment while I assess the damage. Before powering either VESC, I thoroughly dried them off, then blew them off with canned air. After doing that, I blew air under each direct FET to make sure there wasn't any water shorting the gate, drain, or source on them. Once I was sure there was no chance of further damage due to water, I tested various resistors connected to the DRV to see if it was blown of if any needed replacing. I then tested each FET for a short. After all that, I hooked them up to my lab power supply and powered them with a max of 12v and just enough amps to get them to turn on. Realistically in this situation, a shorted FET shouldn't self destruct with somewhere around 6 watts of power going into it. 

So far, both FOCBOXes are powering on with my power supply and do not give any odd reading in VESC Tool or throw any faults. I'll be running them on my test setup shortly to see if they're both still running at 100%. With any luck I managed to avoid any damage to my electronics.

Hopefully for anyone else that has been caught in this situation will get something out of this and be able to avoid having to send me their VESCs haha

TLDR; Submarined the board, powered it off before anything appears to have been damaged
```

---
## \#2 Posted by: lrdesigns Posted at: 2018-03-20T00:42:27.943Z Reads: 251

```
Good luck on the dry out. The loss of power is concerning though.

I submarined my board once, rode though a 4 inch deep puddle. It was dark I couldn't see how bad it was until i was in it. Board was fine no damage, I did do extensive water proofing though because it rains a lot in my area.
```

---
## \#3 Posted by: onepunchboard Posted at: 2018-03-20T00:46:31.326Z Reads: 236

```
I think your battery maybe was leaking power not vesc. 
if vesc got water damage look for green rust.this is very clear sign of water damage. even little as 5v with water make greenish rust.
```

---
## \#4 Posted by: Jedi Posted at: 2018-03-20T00:55:26.204Z Reads: 218

```
bag of rice it
```

---
## \#5 Posted by: trancejunkiexxl Posted at: 2018-03-20T01:03:39.359Z Reads: 201

```
 i used isopropyl alchohol to clean up laptop pcb, it works quite well. im very scared of erosion must be likwe 98% tho
```

---
## \#6 Posted by: LunarKim Posted at: 2018-03-20T03:19:08.479Z Reads: 175

```
I have never dried it for two days.
```

---
## \#7 Posted by: Jebe Posted at: 2018-03-20T03:25:20.400Z Reads: 164

```
My friends son submarined my evolve GT. Opened it up and it was bone dry. Started straight up again.
I wouldn't try that with my builds.
```

---
## \#8 Posted by: ThermalM16 Posted at: 2018-03-20T04:00:46.952Z Reads: 153

```
@onepunchboard I know that you silly goose, I have a customer that managed to submerge 5 of them lol

@Jedi :joy: 

@trancejunkiexxl I use denatured alcohol, its just cheaper and in larger quantities, same end effect though

 @Jebe Well I kind of figured I'd find out if my waterproofing was working one way or the other today, and I got my answer haha

Fortunately my apartment is equipped for almost any VESC repair, so if I blow a FOCBOX up I can repair it pretty quickly. I'll just get it up and running again, tweak my seals and go for round 2 haha
```

---
## \#9 Posted by: b264 Posted at: 2018-03-20T04:01:37.081Z Reads: 144

```
[quote="Jebe, post:7, topic:49568"]
My friends son submarined my evolve GT. Opened it up and it was bone dry. Started straight up again.
[/quote]

That's unbelievable because I had a little bit of damp sand on top of mine from my shoe and it destroyed the entire ESC
```

---
## \#10 Posted by: Jebe Posted at: 2018-03-20T04:07:06.469Z Reads: 144

```
it was totally submerged..... If I wasn't too busy laughing at the poor kid and trying the get video I could have stopped it. He panicked, holding the remote and was squeezing the throttle while chasing it.
```

---
## \#11 Posted by: ThermalM16 Posted at: 2018-03-23T02:41:44.136Z Reads: 94

```
Okay, so I got everything working again, nothing needs to be replaced. I touched up some of the conformal coating on my antispark switch, as well as one of my FOCBOXes. Some wires were corroded, so I replaced them and ended up using marine grade heat shrink on all of my connections (since it comes with an adhesive lining to keep water out). My battery is encased in closed cell foam which is sealed by silicone. In addition I now have a much thicker closed cell foam gasket around my enclosure. 

The only real damage my board suffered was to the sensors in my motors. Those cheap racerstar motors must not have any coating on their sensors...they're dead. I'll just run sensorless FOC until I can upgrade to some 63mm motors.
```

---
## \#12 Posted by: Apolo Posted at: 2018-03-23T03:39:58.995Z Reads: 77

```
I'd imagine the bearings and grip tape would need some extra emergency aid?
```

---
## \#13 Posted by: Acido Posted at: 2018-03-23T06:07:57.520Z Reads: 67

```
Put them in a oven at 100celsius lol to make sure all water is gone
```

---
## \#14 Posted by: lrdesigns Posted at: 2018-03-23T06:59:02.808Z Reads: 65

```
[quote="ThermalM16, post:11, topic:49568"]
Those cheap racerstar motors must not have any coating on their sensors…they’re dead.
[/quote]

Sorry to hear that. I took my racestars apart and applied epoxy over all the sensor PCB for this reason. Before I even used them. Now I feel good that it was actually worth the effort after seeing this result. And knowing mine have been underwater.
```

---
## \#15 Posted by: ThermalM16 Posted at: 2018-03-23T15:37:54.419Z Reads: 56

```
@Acido Won’t high temperatures like that kill the magnets? I might take them apart at some point and see if I can resurrect the sensor boards in them. 

@lrdesigns that was definitely a good call. I just assumed they’d be fine, but I was definitely wrong. Either way they seem to run almost the same without sensors, so I’m not too worried about it right now.
```

---
## \#16 Posted by: Acido Posted at: 2018-03-23T15:59:24.094Z Reads: 53

```
do not put the motor in lol just the vescs
```

---
## \#17 Posted by: ThermalM16 Posted at: 2018-03-23T17:59:32.551Z Reads: 46

```
The VESCs are fine haha. They were conformal coated, no corrosion formed under the FETs. Usually for chips like that you can put some flux around them, heat them up with hot air, and it will blow any corrosion that formed under them out. There was no corrosion though. I conformal coated the FETs this time as well though and cut the conformal coating off the top center of the FETs to help thermal transfer.
```

---
