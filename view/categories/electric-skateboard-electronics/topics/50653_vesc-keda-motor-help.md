# VESC/ Keda Motor Help

### Replies: 20 Views: 771

## \#1 Posted by: AntiPusher Posted at: 2018-03-30T14:43:50.711Z Reads: 96

```
(Warning: This May Seem Stupid)

For my next esk8, i am using a keda 6364 190 kv motor. To figure out which wire goes where, I try each one, and see if the motor works. Problem is, I cannot connect the wires from the motor to vesc, without soldering. How do I figure out which wire goes where?
```

---
## \#2 Posted by: TheFluffiest Posted at: 2018-03-30T16:03:43.779Z Reads: 89

```
No such thing as a stupid question!

Solder some bullet connectors to the motor. It will save so many headaches! Just make sure you tape over the connections once you are done so they don't short. I have the same setup, that's all I did

If you MUST solder it, the way you do it depends on which side of the board the motor is.
```

---
## \#3 Posted by: Blitz Posted at: 2018-03-30T16:10:53.976Z Reads: 82

```
Can't you tap the wires together Use strong electrical tape and do a small test?
Bullets can be expensive if bought alone shipping costs etc.
```

---
## \#4 Posted by: TheFluffiest Posted at: 2018-03-30T16:13:24.328Z Reads: 77

```
@Blitz that works too, but it's a pretty worthwhile investment in my mind
```

---
## \#5 Posted by: Blitz Posted at: 2018-03-30T16:14:11.613Z Reads: 76

```
A direct solder connection can be stronger.
What Kind of investment @TheFluffiest?
```

---
## \#6 Posted by: Acido Posted at: 2018-03-30T16:15:46.633Z Reads: 71

```
the order of the wires does not matter, if it spins in the wrong direction just switch 2 wires
```

---
## \#7 Posted by: TheFluffiest Posted at: 2018-03-30T18:07:02.922Z Reads: 63

```
It's significantly easier to modify if you need to move motors. While it is stronger, I don't see why it needs to be more then a bullet connection and a piece of electrical tape. There should be little to no tension on the wires

That being said, there is something to be said about the strength of a single solder between wires. Much less opportunity for failure. I just prefer the customizability of the bullets
```

---
## \#8 Posted by: Blitz Posted at: 2018-03-30T18:08:33.567Z Reads: 57

```
@TheFluffiest Move motors how? and why would bullets make that easier? 
Customize what Mechanical reverse switch both bullets.. your a genius!
```

---
## \#9 Posted by: TheFluffiest Posted at: 2018-03-30T18:56:37.390Z Reads: 52

```
I've been to make repairs on a couple of occasions, and the ability to remove the motors completely is really helpful sometimes. Not sure what you meant by that last part
```

---
## \#10 Posted by: Blitz Posted at: 2018-03-30T18:57:41.400Z Reads: 56

```
If you have bullets and you change 2 wires your motor will spin the other way, Making a way to reverse without software change. Now back on topic you said.
[quote="TheFluffiest, post:4, topic:50653"]
it’s a pretty worthwhile investment
[/quote]

[quote="Blitz, post:5, topic:50653"]
What Kind of investment @TheFluffiest?
[/quote]

[quote="TheFluffiest, post:7, topic:50653"]
I just prefer the customizability of the bullets
[/quote]

All you came up with was "ability to remove the motors completely" because of repairs, well if something has broken I have bigger problems then unsoldering or cutting a wire. Is that all @TheFluffiest?
```

---
## \#11 Posted by: Blitz Posted at: 2018-03-30T19:12:54.008Z Reads: 48

```
@AntiPusher The answer to your question is Take the wires put them together Tape them with electrical tape and test it gently not pushing a lot of Amps through the wire If it spins in the right direction you're done if not Just switch 2 wires and test again. and don't forget to shave the enamel off the wire Its coated in something.
```

---
## \#12 Posted by: TheFluffiest Posted at: 2018-03-30T21:13:18.853Z Reads: 43

```
The other reason is being able to switch wires. It just makes life easier, and that's worth the extra $5 to me
```

---
## \#13 Posted by: Blitz Posted at: 2018-03-30T21:15:50.523Z Reads: 40

```
Switch wires? you get it right the first time label it and bam its done and 5 dollers where china?
```

---
## \#14 Posted by: TheFluffiest Posted at: 2018-03-30T21:21:40.695Z Reads: 41

```
I got it off hobby king in a large order. 

Neither of what we are saying is more correct than the other, it's a matter of opinion. I prefer the versatility of bullets, you prefer the security of a soldered connection. No need to provoke
```

---
## \#15 Posted by: Blitz Posted at: 2018-03-30T21:23:26.610Z Reads: 42

```
1- Big order from hobbyking yeah He already got his stuff so shipping costs ruin it.

2- I was not provoking you

[quote="TheFluffiest, post:14, topic:50653"]
Neither of what we are saying is more correct than the othe
[/quote]

I'm sorry you said bullets are a worth while investment Own up to it.
A guy is asking how to solder his Phase wires and your saying bullets are worth while investment and you don't give anything to back that up Just defense thats all.
```

---
## \#16 Posted by: TheFluffiest Posted at: 2018-03-30T21:37:50.096Z Reads: 39

```
Must be misreading your tone, I'm at a pretty high stress event. I think bullets are worth it so you don't ever have to worry about getting it right, just take a couple seconds to unplug and switch it over. Two different methods, both work. If he's on a tight budget, go your way, if not then bullets will save some pain later when he upgrades, repairs, or changes something.
```

---
## \#17 Posted by: Blitz Posted at: 2018-03-30T22:03:54.965Z Reads: 37

```
soldering wires is like The easiest thing you can do its easier than soldering connectors in my opinion. 
And It's worries free just tap all 3 wires tape them test it on low amperage not to overload a weak electrical connection if It spins the wrong way switch 2 wires and test again and then permanent solder it.
 In his situation its easier to do that then to go out and buy bullet connectors and wait for them to arrive.
```

---
## \#18 Posted by: TheFluffiest Posted at: 2018-03-30T23:15:41.524Z Reads: 35

```
To each his own. Certainly nothing wrong with strait connection at all!
```

---
## \#19 Posted by: amazingdave Posted at: 2018-03-31T07:13:58.223Z Reads: 32

```
No need to switch phase wires to reverse direction.... just reverse the spin direction in VESCtools... coming from a multi rotor background I’m not a fan of bullet connectors, they can increase resistance over time unless you get very good ones... solder and adhesive lined heatshrink every time for me!
```

---
## \#20 Posted by: ARetardedPillow Posted at: 2018-03-31T10:12:47.202Z Reads: 32

```
You come off looking like a dick here, almost everyone in the community uses bullets, if you think soldering is good then okay, you've expressed your opinion and nobody said anything about it. 

@TheFluffiest was trying to express his opinion and show his way of thinking. No need to bash his fucking face with all the "soldering is better omg why bullets." Let people do their shit okay?
```

---
