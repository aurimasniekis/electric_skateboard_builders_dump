# Broken Collarbone from DIY ESK8

### Replies: 22 Views: 1086

## \#1 Posted by: lasplaner Posted at: 2017-11-11T12:44:02.195Z Reads: 212

```
It has always been my dream to build an electric skateboard. And so I did, in September 2017, and it has been really, really great. Until today.

I decided to allow my sister to have a turn on the esk8, and so I rode her bike. She has had a lot of experience with it in the past, and the small decline of the hill did not make me think twice. So there we are, 500 meters from home, and whizzing on a bike lane at a modest 18-20km/h. Life is Great.

I tell her to watch out, as the bike lane splits into a pedestrian lane and a bike lane, and I tell her to merge into the pedestrain lane. The it hits me. The faster I accelerate, the faster she is going; faster than any speed she had dared to gone before. I knew something was wrong. Then speed wobbles, left, right, left, right. And in a split-second, she is on the floor with multiple scrapes, and most of all, a broken collarbone. To put into context, she had never broken a bone before. What happened?

By the time I got home, and she was sent to hospital, I recalled that she told me the remote was not responding to her command to brake. I carefully open up the remote (Enertion NANO-X). Just 5 minutes ago I was telling her how nice the range is on the remote, with no "dark spots" whatsoever, reception wise. And there it is. It had failed me. The tiny LiPo battery was disconnected from the PCB. Furthermore, parts of the plastic had broken off. Now this is by no means criticism of Enertion, but this disconnection had led to all of those problems.

Why didn't the VESC (Torque Boards 4.12) activate the brakes when the remote disconnected? Because I updated the firmware to Ackmaniac's 2.54 Extended BLDC, and it removed/reset the setting.

So things to take away are; ALWAYS wear a helmet, and to turn on the setting in the VESC because it could save you from injury or even death. Which brings me to one last thing. Why did the joint disconnect? It was soldered properly, and was intact for months. What if I wasn't so close to my destination, and the remote broke? Would I be stranded? I think this is an occasion that we should all reflect on, and I guess part of being an esk8ter is accepting these risks, especially in DIY. But she never signed up, and now I feel extremely sorry.

P.S. she is fine
```

---
## \#2 Posted by: cryo Posted at: 2017-11-11T12:49:19.476Z Reads: 206

```
This is why I think everyone who rides an esk8 needs to know basic longboard techniques for slowing down.
```

---
## \#3 Posted by: SirDiff Posted at: 2017-11-11T12:52:34.974Z Reads: 199

```
You can't slowdown if your motor is accelerating at 20+ mph, unless you can slide (which is pretty difficult with soft and big wheels). 
You didn't have a failsafe set, right?
```

---
## \#4 Posted by: lasplaner Posted at: 2017-11-11T12:53:33.057Z Reads: 196

```
Yes I agree. I could probably slow myself down in that situation, but unforunately, she could not.

Ironically, I was joking to her about this 20 minutes before the accident. I said that sometimes the brake wouldn't work, and that you'd need to slow down manually.

Only god knew that it was going to happen today!
```

---
## \#5 Posted by: lasplaner Posted at: 2017-11-11T12:55:21.652Z Reads: 188

```
It was only 18-20km/h or around 12 mph. I would not let her go 20+ mph!

From personal experience it can brake at around 12 mph, but the remote control's battery wires were disconnected.

I used to have a failsafe, until i updated the firmware, and I forgot to configure it.
```

---
## \#6 Posted by: psychotiller Posted at: 2017-11-11T14:02:11.096Z Reads: 169

```
Not to be a conspiracy theorist, But could that wire have disconnected in the fall? Sounds like she hit the ground pretty hard so the remote probably did as well.
```

---
## \#7 Posted by: Skitzor Posted at: 2017-11-11T14:08:11.755Z Reads: 167

```
I second this, broken plastic and dc battery are most probably from the fall. Since your instincts will tell u in a split second to put your hands to protect your head, the remote probably got her full weight while crashing. Nonetheless I think you should look for the issue at the receiver side. Maybe a bump dc'd the receiver wires in the board, maybe something external prevented the signal for some seconds, I don't know. I just wanted to share the cause is probably elsewhere and it is not logical to blame this on the disconnected battery (after such hard impact)

Safety first and well recovery !
```

---
## \#8 Posted by: Fiori Posted at: 2017-11-11T14:39:00.312Z Reads: 151

```
> Why didn't the VESC (Torque Boards 4.12) activate the brakes when the remote disconnected? Because I updated the firmware to Ackmaniac's 2.54 Extended BLDC, and it removed/reset the setting.

When you build a custom DIY, YOU ARE THE MANUFACTURE. You need to double check these kinds of things, especially when allowing someone else to ride such a powerful machine. 

This is why I always set my board to the slowest possible settings when other people ride my board. It's just not worth having something like this happen. Nobody has the same experience on your custom DIY as you(the builder).

I'm so sorry that she fell. I hope she is ok and recovers fast, a broken collarbone is no fun at all.
```

---
## \#9 Posted by: Deckoz Posted at: 2017-11-11T15:14:50.293Z Reads: 142

```
When my wife tries to steal my esk8, I make her wear all my gear.  I've been teaching her to skate slowly. Before I even let her on I made he practice going down on her knees(no pun intended) in the grass. She still says "seriously?" When I say "don't you dare walk out that door without them hip pads on Missy". I get it, wearing a full face helmet, knee, elbows, hips, gloves is a little much for her 11mph(so far). But I'd rather take the time to teach her to skate safe, and learn to foot brake then throwing her on without skills and no gear.

I've taken some falls at 30+ since she started skating and I've walked away with tiny road rash, thanks to the gear, she doesn't argue now. But now I've gotta tell her that skating with hillbilly hip pads outside of your yoga pants is not a fashion statement, ya gotta wear some sweatpants on the outside.

Hope your sister heals soon, but remember, basic skate skills should be passed on before letting someone dear try an esk8..
```

---
## \#10 Posted by: lasplaner Posted at: 2017-11-11T23:59:40.563Z Reads: 112

```
I don't know. When I checked the remote after the fall it was disconnected, but it was working seconds ago. What do you supect was the problem then?
```

---
## \#11 Posted by: lasplaner Posted at: 2017-11-12T00:01:13.869Z Reads: 110

```
A bump may well have, but the correllation between not being able to brake and a disconnected wire in the remote is too strong for me to ignore...
```

---
## \#12 Posted by: lasplaner Posted at: 2017-11-12T00:05:54.655Z Reads: 105

```
@Deckoz @Fiori I agree. 

The thing is, I wouldn't have let her gone so fast, and nor would she have; it was not her choice. She is not a "beginner" as you know it; she started riding it basically the same day as i did. 

Will definetly make sure more safety gear is worn in the future. As for now, i think its worth testing the failsafe on the VESC.

Thanks
```

---
## \#13 Posted by: Deckoz Posted at: 2017-11-12T00:18:40.043Z Reads: 97

```
But, foot braking is an essential skill. Dont go faster then you can foot brake.. 

I was going 39mph down a hill and my VESCs died. It breaked for half a second and then no brakes.  Aiir checking and foot brake are some of the first things you should practice. :)
```

---
## \#14 Posted by: Namasaki Posted at: 2017-11-12T00:19:27.416Z Reads: 96

```
As @psychotiller stated, the disconnected battery and broken plastic most likely happened during the crash.
The loss of response could have been a simple drop out caused by interference.
Also, if I'm not mistaken, the NanoX receiver has a small internal antenna unlike the RC Mini receiver which has a long external wire antenna. This could be a factor that makes the Nano and NanoX more susceptible to drop outs especially in areas where there is interference.
I tried using a Nano remote once and noticed it consistently lost connection if I got about 15-20 feet from my board.
I quickly abandoned it and went back to the RC Mini.
```

---
## \#15 Posted by: Jinra Posted at: 2017-11-12T01:46:30.017Z Reads: 80

```
nano and nano v2 are vastly different. I've never lost connection so far on my nano v2 (except when my remote battery was low). And antenna length is irrelevant given how close we are to our receivers at all times. 

Maybe the battery did disconnect while riding and the bits of plastic and other damage was from the fall, hard to say.

@lasplaner If it was the battery that disconnected, the VESC likely wouldn't have braked anyway since it times out when it fails to receive PPM signal above a certain time threshold. You have to manually **set** this threshold on the VESC and specify a current to use to brake if it passes it. However, since it was the remote and not the receiver that died, it likely wouldn't have timed out anyway since the receiver was still sending neutral pulse width.

I can tell you from using the winning v1 remote where the receiver **did** cause a timeout, that sudden brakes when you're not expecting it is not a good thing. You get thrown off balance very easily by unexpected brakes and it might be better to bail on your own terms.
```

---
## \#16 Posted by: lasplaner Posted at: 2017-11-12T02:13:12.898Z Reads: 70

```
[quote="Jinra, post:15, topic:38017"]
If it was the battery that disconnected, the VESC likely wouldn't have braked anyway since it times out when it fails to receive PPM signal above a certain time threshold.
[/quote]

I realised that after checking my VESC settings. So forget about what I said.

The battery was almost on full charge, after I checked with my multimeter, so it wasn't that. Good thing was, a bit of soldering and the remote still works.

Just a question - what is the nano vs nano 2? Is the nano-x v2 or v1? because as of today, the remote i see on enertion's website is the I purchased, so i'm assuming that it is the v2. Please correct me.
```

---
## \#17 Posted by: lasplaner Posted at: 2017-11-12T02:15:02.307Z Reads: 64

```
[quote="Namasaki, post:14, topic:38017"]
I tried using a Nano remote once and noticed it consistently lost connection if I got about 15-20 feet from my board.
I quickly abandoned it and went back to the RC Mini.
[/quote]

I noticed that the Nano-X wouldn't do that. I could be at one side of my house, and my remote control 10 meters (30 feet+) from the board, with walls etc. in between, would still be connected. I have not personally had **any** drop out issues with the NANO-X.
```

---
## \#18 Posted by: Jinra Posted at: 2017-11-12T02:16:00.640Z Reads: 66

```
Enertions nano-x is a reskin of the winning nano v2, same remote, different enclosure.
```

---
## \#19 Posted by: lasplaner Posted at: 2017-11-12T02:19:33.044Z Reads: 67

```
Well, does that rule out the interference issue? Apart from this incident, I had never witnessed the remote disconnect.
```

---
## \#20 Posted by: Jinra Posted at: 2017-11-12T02:20:21.153Z Reads: 66

```
I don't think it was interference no. It is possible the battery was disconnected before the fall, but I'm not sure sorry.
```

---
## \#21 Posted by: lasplaner Posted at: 2017-11-12T02:21:56.154Z Reads: 64

```
I guess we will never know...
```

---
## \#22 Posted by: Namasaki Posted at: 2017-11-12T03:57:52.642Z Reads: 54

```
The Nano I used was indeed version 1
When they first appeared on the scene.
```

---
