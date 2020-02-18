# New APS 6355 HEV 190KV: weird noise

### Replies: 17 Views: 1840

## \#1 Posted by: whitepony Posted at: 2016-08-07T09:05:08.742Z Reads: 181

```
hey guys, Im currently running a brand new APS 6355 HEV 190KV on my vanguard and out of the box, it had a weird scraping noise at a certain rotor angle, which I thought was some leftover glue or whatever and I expected it to go away pretty much after the first kilometers. glued on the pulley and ran the board for about 100km now, but still that sound is there and the motor is incredibly noisy under load too - much louder than rspecc and sk6374.

I shot a quick video and maybe the motor experts have an idea what it could be right away. if I wiggle on the rotor, there is some clicking noise as if there is some slop ... and you can hear some pronounced reasonance noise in the video which is coming 100% from the motor, not the mount, the pulley or the truck!

would be nice if you take a look. worst case Ill have to remove that pulley somehow, which will really suck thanks to green loctite! :cold_sweat:

https://youtu.be/f_txfSjrJ44
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-08-07T09:44:06.651Z Reads: 164

```
Sounds like the bearings to me.... But I'm no expert
```

---
## \#3 Posted by: SimosMCmuffin Posted at: 2016-08-07T10:56:04.137Z Reads: 160

```
Bearings and maybe a bit unbalanced? Does it produce a lot of vibration when spinning?
```

---
## \#4 Posted by: whitepony Posted at: 2016-08-07T11:05:54.986Z Reads: 154

```
it seems very well balanced, no vibrations at all :confused:
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-08-07T11:11:42.380Z Reads: 151

```
And it's not the motor pulley rocking on the shaft?
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2016-08-07T11:13:13.578Z Reads: 149

```
I did not think that the balancing would be an issue, as that is a nice looking and sounding motor. There really aren't anything else that could create that noise other than a bearing. How does the loctite react to heat?
```

---
## \#7 Posted by: whitepony Posted at: 2016-08-07T12:30:29.465Z Reads: 146

```
[quote="Michaelinvegas, post:5, topic:7258, full:true"]
And it's not the motor pulley rocking on the shaft?
[/quote]

nah, same noise without pulley, I glued it on, expecting that after a few kilometer, this will be gone! :confused:

not sure about the loctite, but its the same that esk8.de are recommending for the same job!
```

---
## \#8 Posted by: SimosMCmuffin Posted at: 2016-08-07T21:15:20.237Z Reads: 130

```
Not saying they're the culprit here, but does that particular motor have integrated hall-sensors? And if it does, how is the build quality overall? I might be planning buying one the APS motors, so just wondering.
```

---
## \#9 Posted by: barajabali Posted at: 2016-08-07T21:52:26.951Z Reads: 128

```
Is the C clip biting the mount?
```

---
## \#10 Posted by: whitepony Posted at: 2016-08-08T04:50:49.979Z Reads: 121

```
nope, motor is sensoless, but starts up extremely good on the bench. my other motors in foc dont start that well. under load its stuttering from standstill though ... which doesnt really concern me cause im always giving it a push!

its not the clip either. im leaning towards the bearings, nothing would still do scraping sounds after 150km!
```

---
## \#11 Posted by: Pantologist Posted at: 2016-08-08T05:05:12.197Z Reads: 119

```
I was literally going to order one but now I am second guessing. 

Have you contacted APS yet?
```

---
## \#12 Posted by: whitepony Posted at: 2016-08-08T05:28:17.970Z Reads: 115

```
yea, he sent me this (thought a while if I wanted someone to insert my mail text on a public forum, but I think this text doesnt really put him or anyone else in a bad light):

_Hi, the motor noise is the noise that this particular motor makes. The HEV motors are made in a different way compared with the standard motors we sell. I used 2 different version of the 63mm to check and i got the same results. You can reduce the noise by using a lower timing setting. If that noise is something that annoys you i need to sent you the standard 6355._

I think he replied pretty much to the "resonance" phenomenon and not to the scratching sound - maybe thats also a FOC specific thing and it would sound better in BLDC. I recognize that screaming pattern under load from the sk6374, just that its even more pronounced for this HEV 6355 motor. 

we have sent a few mails back and forth and to be honest: it feels like bruno has to respond to a lot of mails - most often you feel that replies are rushed in some way, like he didnt read all details. I think Ill just run that motor until it fails and then go back to my SK6374 168KV ... or maybe Ill open it soon due to curiosity - just waiting for my gear puller tool to get that glued pulley of the shaft. 

to be fair: it was a very cheap motor for me. I had a 10% discount on my total order because bruno sent me a wrong wheel hub on my last order, so that motor only cost me 58€ - thats HALF of an rspecc and the rspecc is definitely not really better at anything.

I switched out my sk6374 168KV for the HEV and I feel like Im not really lacking torque, I have a slightly higher topspeed due to 15/36 with 190KV vs. 16/36 @ 168KV and the motor is much lighter @ only 508gr (think its the lightest motor around?). it comes stock with superflexible silicone wires (sadly only 14AWG), the closed body is kinda nice and it runs very cool, even under a lot of load (maybe due to the full aluminum mount, that seems to soak up a lot of heat unlike the CFK enertion mount). Ill try the 2nd HEV motor I got probably on my spud - that one has no scraping at least.
```

---
## \#13 Posted by: Pantologist Posted at: 2016-08-08T05:32:27.476Z Reads: 101

```
Weird how he has the same sound with two of his motors, but your second one doesn't...
He is definitely thinking of the wrong thing. 

The peeps in China told me they can just change the motor cans with closed ones. I don't think there is anything different between the closed ones and the opened ones.
```

---
## \#14 Posted by: Namasaki Posted at: 2016-08-08T06:50:31.455Z Reads: 101

```
I recently bought 4 of the APS HEV 6355 motors and out of the box there is no abnormal sound when spinning them by hand.
I openened up 2 of them today for cleaning( one got a rock stuck inside) and noticed that they put a thrust washer on the shaft that is much larger than 10mm. This seemed rather strange to me and I omitted it when putting them back together.
This thrust washer could very well be causing the scraping noise because it is apx the same dia as the ball bearing cover and would make contact between the inner and outer race of the bearing.
Not sure why you glued the pulleys on. If you use the key and set screw, it should stay on just fine.
Gotta be able to take the motors off to clean rocks out of them.

You could have got a motor with a bad bearing though it is unlikely.
The shafts are machined very close to the bearing inner race so they fit tight.
one of mine was so tight that I almost couldn't get it apart.
To check the motor, take it off and spin it by hand.
```

---
## \#15 Posted by: whitepony Posted at: 2016-08-08T07:21:46.634Z Reads: 99

```
[quote="Namasaki, post:14, topic:7258"]
Not sure why you glued the pulleys on.
[/quote]

the shaft is too short for the 15mm pulleys and the grub screw is in the outer smaller cylinder - which I now sunk into the motor mount shaft opening which is sufficiently large. I never ever cleaned my motors cause I dont have a way to put in that shaft clip, just using my vacuum cleaner to get rid of some dust every now and then. :yum:
```

---
## \#16 Posted by: Namasaki Posted at: 2016-08-08T11:32:19.245Z Reads: 95

```
The shafts are a bit short. I've got my set screws in between the belt teeth. The pulleys I got from APS had only one so I drilled and tapped 2 more so I have 3 equally spaced.
```

---
## \#17 Posted by: whitepony Posted at: 2016-08-10T16:12:17.742Z Reads: 79

```
I have probably put around 250km into that motor by now - my quick conclusion:

positive:
+ lightest 63mm outrunner available to my knowledge (508gr)
+ comes with silicone wires and 5.5mm gold bullet connectors
+ least resistance of all my motors in idle (= best coasting)
+ most silent motor I got when coasting - this thing is just dead somehow, I only hear the belt
+ most balanced motor I got - absolutely no vibration
+ comes with a keyway + key
+ cheapest of my motors
+ mostly closed body
+ runs coolest (but this is most likely due to the full aluminium APS mount)

negative:
- 1 out of 2 had that scratching thing, Ill assume its not intended but the motor still really runs well and well balanced at high rpms so Im still not sure what it is
- in FOC mode: noisiest of my motors at full load mid rpm, but it feels like it has somehow become more silent after 250km (or I got used to it)
- shaft is too short for 15mm pulleys and Im not sure if 10mm is necessary
- only 14AWG wires used


especially for the price, its a very nice motor and Ill probably use no2 for my spud freebord! torque is less than my sk6374, but about the same as the 6355 rspec. near impossible to quantify without acceleration tests!
```

---
