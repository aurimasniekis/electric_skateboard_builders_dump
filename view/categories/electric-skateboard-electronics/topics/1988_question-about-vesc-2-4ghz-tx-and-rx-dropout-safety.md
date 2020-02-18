# Question about VESC + 2.4ghz TX and RX dropout safety

### Replies: 32 Views: 3074

## \#1 Posted by: lilracerboi Posted at: 2016-03-25T21:35:42.313Z Reads: 117

```
I ordered a VESC last month and am waiting for it to ship with the next batch and I am planning on getting a new controller after a nasty crash recently with my Wiiceiver + Kama malfunctioning.

My question is, what is the result of a 2.4 ghz TXRX, like the GT2B, when the connection, either from the remote or physically, drops from the VESC?

For example, the HobbyWing EZ Run ESC will initiate the brakes for just a moment when the receiver is disconnected. That was the cause of me falling off my board at full speed (thankfully my board isn't 20+mph fast). I plan on getting the Torqueboards 2.4 Ghz remote.

Any advice on making my board safer? I haven't ridden is for fun in a while, just to get to class on campus.
```

---
## \#2 Posted by: torqueboards Posted at: 2016-03-25T21:43:17.676Z Reads: 117

```
I think is is more so due to the Nyko kama bluetooth + receiver. When it drops the last input it takes it keeps or something along those lines.

So IMO I prefer 100% reliability and no issues at all of the connection dropping.

We are working on a new version of the Wiiceiver. Not sure when it will be released but it will be a finished product and no more kit form.

TorqueBoards 2.4ghz Mini Remote works well. 100% reliability, no drops. Just no cruise control. Small form factor.

It's similar to the GT2B as far as reliability goes.
```

---
## \#3 Posted by: trbt555 Posted at: 2016-03-25T21:47:46.382Z Reads: 110

```
I think you can configure the vesc to time out and apply a pre defined brake current -or not- in case no signal is received from the rx
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-03-25T21:53:41.549Z Reads: 102

```
I'll need to get a few to swap out .... Don't like throttling by thumb .... Feel I have less control...the trigger finger gives me better control .... Guess cause I'm use to RC cars
```

---
## \#5 Posted by: torqueboards Posted at: 2016-03-25T21:54:21.103Z Reads: 101

```
me too. trigger is more precise.
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-03-25T21:54:43.507Z Reads: 99

```
You don't do a buy three get one free do you ??? Lol
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-03-25T21:56:09.770Z Reads: 97

```
Yeah man....it just feels way more natural....I don't know how to explain it....especially if you gun it....It's like YEAH BABY....Gimme the Juice!⚡️⚡️⚡️⚡️⚡️⚡️
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-03-25T21:57:22.838Z Reads: 96

```
Or I can be Ghetto and just swap on receiver between boards lol
```

---
## \#9 Posted by: RunPlayBack Posted at: 2016-03-25T22:39:08.145Z Reads: 93

```
I own two @torqueboards mini remotes - one paired with a single VESC and another on dual VESCs. No dropouts and best value for the price. I also like that its small enough to fit in my pocket.
```

---
## \#10 Posted by: Michaelinvegas Posted at: 2016-03-25T23:00:53.689Z Reads: 91

```
Is that a @torqueboards 2.4ghz remote in your pocket? Or are you just happy to see me? Lol
```

---
## \#11 Posted by: lilracerboi Posted at: 2016-03-25T23:11:35.792Z Reads: 92

```
@torqueboards I know about the Kamas thing with keeping the last input when the connection between the chuck and it's own receiver drops, but when the Wiiceiver looses any kind of connection with the ESC, it'll initiate the brakes like a stutter, then it'll go into a neutral state.
```

---
## \#12 Posted by: lowGuido Posted at: 2016-03-25T23:37:37.492Z Reads: 96

```
I feel like I repeat myself alot here. because I do.
But i kinda feel for the people who buy a wiiceiver that comes with a socket built in and rightly assume you should be able to plug the dongle in and have it work safely.
IT WILL NOT.
You must open up the dongle and solder it or else you will experience droppouts with unexpected results.  Almost guaranteed to SYF!
https://www.instagram.com/p/BAs03vxCSeq/
https://www.instagram.com/p/BAs1Uq_iSfd/
```

---
## \#13 Posted by: torqueboards Posted at: 2016-03-26T00:41:48.000Z Reads: 86

```
@lowGuido - Great vids :smile: Now only if there were an abundance of stock on Nyko Kamas!
```

---
## \#14 Posted by: treenutter Posted at: 2016-03-26T03:02:42.234Z Reads: 86

```
@lilracerboi I also have one of @torqueboards mini remotes and I've never had a signal drop when using it.
```

---
## \#15 Posted by: lilracerboi Posted at: 2016-03-26T03:24:59.019Z Reads: 85

```
That's really good to know. After my recent crash, I've been to scared to ride my board. Hell, even before I've been weary about the Wiiceiver since this is the SECOND time it happened. 

Does the VESC do anything when the connection to the receiver is broken?
```

---
## \#16 Posted by: treenutter Posted at: 2016-03-26T03:32:06.342Z Reads: 85

```
@lilracerboi I can't honestly say I know how it behaves. Since I switched controllers I haven't had a single drop out. I think that @trbt555 is right that you can configure this to some degree.

As far as your faith in your controller. I had some similar experiences with the nunchuck. In the end I ditched it for the RC remote and I'm much happier now.
```

---
## \#17 Posted by: psychotiller Posted at: 2016-03-26T03:38:13.763Z Reads: 88

```
Your Ez run should have went to coast at a dropped signal...very odd to hear that happened to you
```

---
## \#18 Posted by: Kaly Posted at: 2016-03-26T03:40:12.725Z Reads: 88

```
@lowGuido that's a good connection there, but I had some serious issues with the wiiceiver and the cell towers here in NYC.  

Sometimes it just dropped the signal and I had no input on the ESC. The other times was more scarier, the tower will interfere with the wiiceiver and the thing will accelerate at full throttle ( no good to be speeding up full throttle in the Bronx ) that's when I call it quits with the wiiceiver. 

I know a lot of people like it, personally I use to love it , but if you live in a big city with a lot of cell towers , wifi, interference, etc. save your self a trip to the hospital and get a 2.4 ghz remote. 

In the other hand if in your area you do not have this type of interference just solder your wires and use the wiiceiver. IMO the software is the best controller for eBoard in the world.
```

---
## \#19 Posted by: lowGuido Posted at: 2016-03-26T04:05:21.599Z Reads: 87

```
I gotta admit I have never skated NYC so I can't really compare. But where I live in Australia I have had no such cell tower interference in over a year of skating.
```

---
## \#20 Posted by: torqueboards Posted at: 2016-03-26T04:21:14.773Z Reads: 88

```
Yeah, SF downtown is pretty much just as bad.. Specific corners it will just drop 100% every time. Although, I did not give the soldering option a try.
```

---
## \#21 Posted by: Michaelinvegas Posted at: 2016-03-26T05:05:06.851Z Reads: 83

```
It's like what WE ALL do ain't dangerous enough and we throw in a dodgy reciver and transmitter....

How hard is it to get the same features via the 2.4ghz remotes? It's it the lack of buttons? Simpler still a thumb control for those who choose it.
```

---
## \#22 Posted by: torqueboards Posted at: 2016-03-26T05:21:11.608Z Reads: 81

```
We're working on a new one similar to how Ben did his and replaced the internal PCB. Guess, we'll see once we test it.
```

---
## \#23 Posted by: lilracerboi Posted at: 2016-03-26T05:58:10.869Z Reads: 80

```
Just made a video of what my ESC does when the receiver is disconnected. I may just solder the wires to the pins again.
Also, I'm using my wired nunchuck that I extended, because my Kama is out of battery.

https://youtu.be/TdCGdphiey0

I know my board is really messy, but I plan on redoing pretty much everything soon.
```

---
## \#24 Posted by: trbt555 Posted at: 2016-03-26T07:17:01.931Z Reads: 80

```
Doesn't look problematic to me.
Or am I missing something ?
```

---
## \#25 Posted by: lowGuido Posted at: 2016-03-26T09:57:39.892Z Reads: 78

```
Or you could convert to push assist. And have no remote at all. 😉
```

---
## \#26 Posted by: Michaelinvegas Posted at: 2016-03-26T13:01:50.812Z Reads: 76

```
I need a VESC ... 😒 I shall wait my friend .... But I shall do your mod... Loved it bro👊🏻
```

---
## \#27 Posted by: lilracerboi Posted at: 2016-03-26T17:31:44.077Z Reads: 78

```
@trbt555 The problem is when I'm moving fast, this could happen at any moment and if I'm not prepared, such as when turning, it'll throw me off balance.

Once the disconnection happens, it throws out the brakes pretty hard.
```

---
## \#28 Posted by: trbt555 Posted at: 2016-03-26T17:58:36.447Z Reads: 77

```
I see.
For an RC vehicle this is a desirable behavior, if you lose connection, you don't want yout vehicle to run a way on you and stop.
Not so for an eskate! That's why you need a vesc.
```

---
## \#29 Posted by: lilracerboi Posted at: 2016-03-26T20:27:36.254Z Reads: 75

```
Yeah, it's happened twice now.
I have a VESC on order and am waiting for the next shipment.
```

---
## \#30 Posted by: treenutter Posted at: 2016-03-27T23:35:16.208Z Reads: 72

```
@lilracerboi I've had a few controller dropouts when using VESC and a nunchuck. As far as I can tell, the VESC just cuts throttle to the motor and allows the board to stop naturally. The problem is that with a reduction ratio and brushless motors that already have some resistance when neutral, that can mean a brake-like force is applied, especially if you are accelerating when you lose your connection, and ever more so if you have high reduction ratio like I do (14:60). So my suggestion is to use the most reliable controller you can possibly find.
```

---
## \#31 Posted by: Squatcher30 Posted at: 2018-01-10T03:22:44.917Z Reads: 29

```
Question. I have two MayTech VESCs on my board, with a 2.4ghz remote. When the battery dies at 29 volts, the board seems to do a sudden brake jolt before losing power. It is extremely annoying and makes me nervous to ride up hills because it tends to throw you off the board. Any ideas? Is it a BLDC programming parameter issue that can be fixed?
```

---
## \#32 Posted by: Blasto Posted at: 2018-01-10T03:45:33.300Z Reads: 26

```
[quote="Michaelinvegas, post:26, topic:1988"]
need a VESC ... 😒 I shall wait my friend .... But I shall do your mod... Loved it bro👊🏻
[/quote]

I got you covered bro

@Squatcher30 thanks for the thread revival. @Michaelinvegas has been waiting 2 years for his vesc
```

---
