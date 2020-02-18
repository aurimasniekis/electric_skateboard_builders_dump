# Question on CAN vs split ppm

### Replies: 17 Views: 1047

## \#1 Posted by: onepunchboard Posted at: 2018-04-16T17:00:30.600Z Reads: 219

```
I'm going dual but since I'm using different 2 diff motor, 190 and 260kv, and gear ration is a bit different to compensate as well, 15/36 and 12/36.

I think 2 receiver may be better solution, What do you think?

And another one, Does Traction control helps on loose ground significantly?
```

---
## \#2 Posted by: skatardude10 Posted at: 2018-04-16T17:04:50.408Z Reads: 206

```
I wouldn't call traction control an essential feature, but it does help a bit if you hit sand, or gravel, etc.
```

---
## \#3 Posted by: Acido Posted at: 2018-04-16T17:22:03.674Z Reads: 193

```
split ppm, safest method as i know
```

---
## \#4 Posted by: Deckoz Posted at: 2018-04-16T17:38:33.775Z Reads: 185

```
I wouldn't run can on different KV motors... Stick to split ppm...

This is coming from a guy who runs sensored FOC over CanBus with traction control exclusively on my personal boards..
```

---
## \#5 Posted by: onepunchboard Posted at: 2018-04-16T17:40:37.479Z Reads: 183

```
That's what I thought. I saw many fired vesc even with experienced builders without any of my problem. Thanks
```

---
## \#6 Posted by: Da_gree Posted at: 2018-04-16T18:01:31.791Z Reads: 176

```
I fried several VESC's trying to make a CANBUS connection, stupidly without an antispark switch. Been running split ppm since then with no problems. I won't try another CAN connection until I'm more confident in my skillset, and the price of VESC'd comes down a bit more. I split out the ppm signal wire alone, and it works great.
```

---
## \#7 Posted by: bigben Posted at: 2018-04-16T19:59:58.621Z Reads: 167

```
I’ve always done split ppm or dual receiver. 
Always remove one positive wire from the splitter and you should be all good. 
A lot of people swear by canbus but it seems easier for it to go wrong.
```

---
## \#8 Posted by: fraannk Posted at: 2018-04-16T20:14:26.344Z Reads: 163

```
Don't you mean remove one +5v wire?
```

---
## \#9 Posted by: bigben Posted at: 2018-04-16T20:15:55.912Z Reads: 160

```
Doh, yep. that's the one.
My apologies for leading astray.. 
Will edit now.
```

---
## \#10 Posted by: onepunchboard Posted at: 2018-04-16T20:23:57.024Z Reads: 156

```
Thanks guys, Since I have 5 receivers because the seller sent me 2 times, I will use 2, cuz it's easier
```

---
## \#11 Posted by: bigben Posted at: 2018-04-16T21:24:50.527Z Reads: 154

```
And gives you some backup if parts fail. You can always get home if a vesc, motor or receiver blows. One half should always work.
```

---
## \#12 Posted by: tux-scooby Posted at: 2018-04-24T12:48:45.106Z Reads: 142

```
Is there tutorial how to configure dual focbox split ppm? Thank you in advance for help :slight_smile:
```

---
## \#13 Posted by: RedEagle Posted at: 2018-04-27T22:37:58.258Z Reads: 137

```
You have three wires of the receiver. 
+5v
Signal
Ground

Solder signal together. 
Solder ground together. 
You have two +5v wires. One on each vesc. 
Cut one +5v wire. You only need to connect one +5v wire to the receiver. 
So in the end you'll have one +5v wire, 2 signal wires and two ground wires connected to the receiver. 

Hope this helps.
```

---
## \#14 Posted by: tux-scooby Posted at: 2018-04-28T08:23:25.775Z Reads: 129

```
Thank you for clarifying that part for me, it is really helpful. I am just starting to assemble my emtb so I have couple of more questions : motor detection and configuration is done on each motor separately? Is there some recommendation regarding the motor and battery settings?
```

---
## \#15 Posted by: RedEagle Posted at: 2018-04-28T17:51:22.905Z Reads: 120

```
Motor detection and detection has to be done separately for each motor. There are a few emtb builds you can copy here on the forum.

Seriously, it seems to me that you only signed up yesterday. No hard feelings.
```

---
## \#16 Posted by: uigiroux Posted at: 2018-04-28T18:07:31.432Z Reads: 116

```
I've asked this before but I am still not totally understanding how to do this.  Could someone please explain how to set up 4 VESC's for 4WD?  Please if someone could draw a diagram that would be helpful.  I've heard to daisy chain a canbus, I was thinking about connecting 2 VESC together for a front and rear drive, and then connect those via ppm, or just using two receivers for the front and rear, but I've also heard that's bad...  Can I get a DETAILED explanation please???
```

---
## \#17 Posted by: tux-scooby Posted at: 2018-04-28T21:35:49.653Z Reads: 107

```
No reason for had feelings. I just started the assembly and I had difficulty finding the right answers on questions that concerned me :)
```

---
