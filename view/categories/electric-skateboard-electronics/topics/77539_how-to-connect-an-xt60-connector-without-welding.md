# How to connect an XT60 connector without welding&hellip;?

### Replies: 30 Views: 1177

## \#1 Posted by: kchxaz Posted at: 2018-12-09T20:04:40.599Z Reads: 201

```
Hi all,

Wondering if there is a way to connect my battery (xt60 connector) without throwing a giant welding spark as I try to connect the two? As I close the two ends together right about the point of contact it throws a giant spark, burns away one of the connector pins and chars the plastic part. I switch out the extra battery I have for my Haloboard all the time and it just throws a small non-eventful spark without damaging anything. They are both 10s3p batteries.

Any hints or tips on how to connect the the two connectors without welding my face to it, please?
```

---
## \#2 Posted by: brenternet Posted at: 2018-12-09T20:06:32.114Z Reads: 199

```
You need an xt90 my friend, built in antispark.
```

---
## \#3 Posted by: xclr8r Posted at: 2018-12-09T20:34:32.290Z Reads: 187

```
Search the forum for xt90 loop key and look at the wiring diagrams and pics people have posted. Super helpful ideas on how to wire it up so you don’t get a spark.
```

---
## \#4 Posted by: VECTOR.xyz Posted at: 2018-12-09T20:35:38.800Z Reads: 184

```
https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

Take a look at this post, really helpful.
```

---
## \#5 Posted by: pat.speed Posted at: 2018-12-09T21:23:17.595Z Reads: 166

```
@brenternet
@xclr8r

Guys be careful to new peeps that is not quite right. What he needs is a XT90s, the little ‘s’ means antispark. This fella wouldn’t have known that and might have bought normal XT90 connectors
```

---
## \#6 Posted by: brenternet Posted at: 2018-12-09T21:27:39.074Z Reads: 153

```
Fair enough. You're right.
```

---
## \#7 Posted by: kchxaz Posted at: 2018-12-09T21:34:33.199Z Reads: 141

```
I, see, ok good. A quick googling of that turns up plenty of options. Looks like one w/ a pre-soldered, green "L" is the way to go.

So how do the ppl who assemble the boards get it out together without sparking it? 

OH, and do I hook up the main battery to VESC connector first or the recharge connector first? Does it matter? 

Thx
```

---
## \#8 Posted by: brenternet Posted at: 2018-12-09T21:37:41.973Z Reads: 131

```
It really does sound like you've got some serious reading to do.

Generally you'd have a break before your battery gets to your esc. That would be a loop key or antispark switch of some sort. A lot of people do just plug the battery directly into the esc with a xt90s (split enclosure vanguard style) and that acts as both an antispark and engagement. 

Read some threads and look at some wiring diagrams, you really shouldn't be handling a battery without this information.
```

---
## \#9 Posted by: kchxaz Posted at: 2018-12-09T21:40:09.300Z Reads: 125

```
I've actually picked up the xt60 connector, regular I am assuming, and I have them all soldered on there nicely, heat shrinked, and touched up w liquid insulation compound - both to insulate and help keep it together. Now I want to connect them but am afraid it will spark like hell again. How do they connect them at the shop when they are building them?
```

---
## \#10 Posted by: pat.speed Posted at: 2018-12-09T21:46:28.140Z Reads: 117

```
Pre built boards use antispark switches. It is just as switch wired in before the esc. So that you can turn it on and off. It is not a normal switch, you can purchase from forum members
```

---
## \#11 Posted by: kchxaz Posted at: 2018-12-09T21:56:12.563Z Reads: 113

```
I'm sorry, I don't understand. Why take something that is already an anti-spark connector and have to do that to it? Why?
```

---
## \#12 Posted by: Blitz Posted at: 2018-12-09T21:59:14.595Z Reads: 104

```
@kchxaz Tell us what you know about anti-spark xt90s and we'll try fill in the gaps bro.
```

---
## \#13 Posted by: kchxaz Posted at: 2018-12-09T22:03:34.960Z Reads: 102

```
Very little. Didn't even know there were anti-spark xt 30/60/90 connectors available. The old one I'm replacing is actually an xt30 connector (non-anti spark), it's for my Acton Qu4tro. I bought the wrong ones (xt60) by mistake.
```

---
## \#14 Posted by: pat.speed Posted at: 2018-12-09T22:04:44.971Z Reads: 100

```
I’m don’t think there are xt60 and xt30 antispark. Well I’ve never seen them

If you don’t want a loop key you can just change the connectors so that you plug the battery into the esc to turn it on
```

---
## \#15 Posted by: kchxaz Posted at: 2018-12-09T22:05:25.714Z Reads: 97

```
Not trying to arguer - maybe I'm not seeing something - but there is nothing at all in line between the connector and the solder points on the ESC board.
```

---
## \#17 Posted by: pat.speed Posted at: 2018-12-09T22:07:24.612Z Reads: 94

```
That is because the esc probably has its own switch for turning on and off then.

If you want to stop the sparks you need to swap the connectors to XT90s connectors. They have a little resistor that stops the initial spark from the capacitors

Edit: I meant spark you silly sausage @wafflejock
```

---
## \#18 Posted by: wafflejock Posted at: 2018-12-09T22:08:42.876Z Reads: 90

```
Speak -> peak (high current, "inrush" to capacitors from battery to esc)

Haha okay was guessing thanks for clarifying
```

---
## \#19 Posted by: pat.speed Posted at: 2018-12-09T22:08:55.888Z Reads: 91

```
You do have the correct polarity yeah? It shouldnt be that bad a spark just from connecting the battery
```

---
## \#20 Posted by: b264 Posted at: 2018-12-09T22:08:57.679Z Reads: 92

```
[quote="brenternet, post:2, topic:77539, full:true"]
You need an xt90 my friend, built in antispark.
[/quote]

That would be an XT90S - the XT90 do not have resistor
```

---
## \#21 Posted by: Blitz Posted at: 2018-12-09T22:09:29.536Z Reads: 88

```
LoL I'm too late to help the new guy this place is swarming with helpers.
```

---
## \#22 Posted by: kchxaz Posted at: 2018-12-09T22:28:50.924Z Reads: 85

```
I definite have the polarity correct. I have more than a little experience soldering but that doesn't necessarily exempt me from making mistakes from time to time either.
```

---
## \#23 Posted by: kchxaz Posted at: 2018-12-09T22:29:48.387Z Reads: 86

```
Not too late. Still watching this string for now. Trying to figure out exactly what to order before the window closes in about an hour.
```

---
## \#24 Posted by: brenternet Posted at: 2018-12-09T22:44:37.988Z Reads: 86

```
Thanks penis :smiley: I've already been corrected by the unwashed masses.
```

---
## \#25 Posted by: Richcan Posted at: 2019-07-21T03:31:18.946Z Reads: 45

```
What is this anti spark thing I’ve been hearing?
```

---
## \#26 Posted by: Flasher Posted at: 2019-07-21T03:38:38.763Z Reads: 49

```
@Richcan basically a connector with a resistor inside it. It limits the electricity coming in long enough for you to plug it in fully without creating a spark
```

---
## \#27 Posted by: Flasher Posted at: 2019-07-21T03:42:23.723Z Reads: 49

```
@Richcan
This:
![Screenshot_20190720-233954_Google|622x500](upload://1oCMxPbxwkWOAcLYZ9JKQ7iWyuT.jpeg) 
From there if you want a better idea go see @b264 post about loopkeys
  https://forum./t/how-to-make-an-xt90s-loopkey/2325
Or come chat with us on the other side
```

---
## \#28 Posted by: Richcan Posted at: 2019-07-21T12:50:25.560Z Reads: 44

```
Ok Thanks! Ya was thinking a good tight connector. Didn’t know had resistor? Good to know when I do my build! Been reading some units overheating or starting fire! I ordered those XT90 I’ll check if has resistor? I’m guessing there is inline resistors also? When building basically between battery and focbox? Is that the only location for these because of the high current. I heard Focbox might have this built in the boxes? If so would you still install extra one? Thanks
```

---
## \#29 Posted by: Flasher Posted at: 2019-07-21T18:51:11.083Z Reads: 33

```
If it doesn't have the green line on it, it doesn't have a resistor in it. I would recommend using one no matter what. Repeatedly connecting and disconnecting the battery pack without any resistance at the point of connection will eventually start melting the connectors from the heat created by the sparks. I dont believe you could put an inline resistor as this would continuisly limit current rush and would in turn fry the resistor. In an xt90S, the resistor is at the tip of the connector and is no longer in use once the connector is completely seated inside the Male xt90.
```

---
## \#30 Posted by: Richcan Posted at: 2019-07-21T19:04:52.408Z Reads: 30

```
Thanks! Makes sense! I’ll check out what I purchased. I’d rather play it safe!
```

---
## \#31 Posted by: deucesdown Posted at: 2019-07-22T07:26:52.341Z Reads: 21

```
[quote="kchxaz, post:1, topic:77539"]
throws a giant spark, burns away one of the connector pins and chars the plastic part
[/quote]

This is not typical. Usually you connect a pack, it throws a spark big enough to scare you and might leave a small char on the connector. Nothing to worry about, but the connectors may wear out and need to be replaced after a few dozen cycles.

To actually melt the connector and burn the housing, this does not happen from just connecting a pack to the escs.

I believe you direct shorted the pack somehow. No XT90s or other technology will save you from melted stuff here.
```

---
