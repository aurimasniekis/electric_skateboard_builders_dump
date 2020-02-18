# Maytech Dual Hub ESC (setup help) MTDU30A

### Replies: 21 Views: 1212

## \#1 Posted by: kvboards Posted at: 2018-02-18T04:48:15.470Z Reads: 206

```
I have a question for anyone working with the maytech MTDU30A. The problem is when connected with 2 motors they wont spin and just sound like an electrical twitch. Has anyone seen this before and how to fix? Does this dual ESC require hall sensor wires connected or will these sensorless motors work without hall. Any input would be helpful. Thanks!
```

---
## \#2 Posted by: e.board_solutions Posted at: 2018-02-18T10:22:29.925Z Reads: 188

```
Hey, wich motors do you use? There are 2 versions of their dual ESC's, 1 for hubs & one for outrunner motors :slight_smile:
```

---
## \#3 Posted by: Riako Posted at: 2018-02-18T11:25:11.629Z Reads: 182

```
Maytech said it's developped to work better in sensored foc mode on their hub motor ...
Don't really know if it works with other motor I haven't test ... But if you could yes try with all connected maybe it help ... Did you mail your reseller ?
```

---
## \#4 Posted by: SPIRITRON Posted at: 2018-11-26T22:01:02.502Z Reads: 130

```
I have this exact same problem! It may be that the sensor wires MUST be connected. I am trying to run mine sensorless because I don't have the right jst connection atm (waiting for delivery)😬 i have also tried them with vesc's (sensored) and they work perfectly! 
Did you find any solution?
![15432697961115639538556395405461|375x500](upload://vxrxUbjTWqBxuynqpT8TsLHk09m.jpeg)
```

---
## \#5 Posted by: rollinsoul Posted at: 2018-12-02T10:36:22.106Z Reads: 111

```
Hi,
Noob here. Just got the same esc and I'm trying to hook up to the same hubs.  Did you get it to work was it necessary to hook up the sensors? What's the performance like? Can I use my  remote from my meepo board or do you have to use maytechs? How do you pair the remote? Lastly what is the red, brown and yellow cable for?
Regards
```

---
## \#6 Posted by: pat.speed Posted at: 2018-12-02T11:22:59.814Z Reads: 106

```
The cable is for a receiver
```

---
## \#7 Posted by: SPIRITRON Posted at: 2018-12-02T11:23:38.174Z Reads: 108

```
The red yellow and brown cable is what connect to the receiver and you pair it with your remote. I'm not sure about meepo remotes, does it come with a receiver or is it built into the meepo ESC?

I'm still waiting for the sensor cables so I have not tried it yet, will let you know in a week or so..
```

---
## \#8 Posted by: rollinsoul Posted at: 2018-12-02T12:48:53.155Z Reads: 107

```
Thanks for the quick reply.  So it looks like I need to buy the maytech remote then. Drag!
```

---
## \#9 Posted by: rollinsoul Posted at: 2018-12-02T12:55:21.310Z Reads: 102

```
Thanks for the quick reply.  Sorry but what leads do I need to get as my hall sensors connectors on my hubs are too big for the maytech esc. Will I have to crimp or solder the wires to the connectors?
```

---
## \#10 Posted by: SPIRITRON Posted at: 2018-12-02T13:03:13.081Z Reads: 98

```
You need to swap the connectors to female zh 1.5mm and they will fit. If they come with wires you can just solder them, if just connectors you have to crimp. Contact @rey8801 maybe he can send you some, or order them on eBay
```

---
## \#11 Posted by: pat.speed Posted at: 2018-12-02T19:54:01.475Z Reads: 84

```
You can probably buy sensor wire adapters
```

---
## \#12 Posted by: rollinsoul Posted at: 2018-12-02T20:09:41.767Z Reads: 85

```
Oh great. That's a better option as my soldering skills aren't there yet. Crimping looks hit and miss with thin wires. Where can I get them and are they safe? Thanks.
```

---
## \#13 Posted by: pat.speed Posted at: 2018-12-02T20:12:41.756Z Reads: 85

```
I’m not sure exactly but I’d try eBay, apparently they are ZH 1.5mm so you need to find connectors with that to go into the esc and then the right size for the motor wires. Although I’m not actually sure the size of the sensors for those motors
```

---
## \#14 Posted by: rollinsoul Posted at: 2018-12-02T20:35:22.603Z Reads: 82

```
Thanks for the invaluable info. I'm on it.
```

---
## \#15 Posted by: rollinsoul Posted at: 2018-12-03T21:57:55.894Z Reads: 79

```
Thanks. I order some on eBay. I'll get crimping tool. As well. Cheers!
```

---
## \#16 Posted by: rollinsoul Posted at: 2018-12-18T22:53:19.632Z Reads: 71

```
Finally got the maytech dual esc hooked up to skullboard hubs. Outcome not good. After attaching hall sensors (monumental pain) soldering new 4mm plugs and finding the right combination, all I get are cut outs. Doesn't look like they're compatible. Will try to hook up my verreal hubs to see if that works.
Any suggestions would be welcomed.
```

---
## \#17 Posted by: rollinsoul Posted at: 2018-12-26T08:04:12.656Z Reads: 63

```
Just to say I got the maytech esc working with my verreal hubs. Much increased torque than meepo/wowgo esc, which is what I was looking for. My only issue is the v2 remote which i can't get on with. Hopefully I can pair the maytech esc with my wowgo remote.
Thanks for your support and patience. Happy holiday.
```

---
## \#18 Posted by: rollinsoul Posted at: 2019-01-18T21:53:29.582Z Reads: 53

```
Hi. Got the maytech running well. However I want to  stop using their v2 remote, as its sticking in when I brake and in full throttle. Not safe. Tried pairing with my old wowgo and meepo remotes but no success. Do you know any other remotes that will work? Are you using the v2 remote and are you having the same issues
```

---
## \#19 Posted by: SPIRITRON Posted at: 2019-01-18T22:15:26.900Z Reads: 55

```
Damn that's not safe at all, maybe open it up and see what's making it get stuck? Yeah I have the same remote, it's not very sensitive and really jerks on throttle and brake. I did try to test it with my aps remote but didn't work not sure why but I didn't really look into it too much (could have been something else). I think I'm going to get rid of them both soon as its just not doing it for me...
```

---
## \#20 Posted by: rollinsoul Posted at: 2019-01-20T22:07:32.028Z Reads: 53

```
Tell me about it! Someone posted the same problem on YouTube. Hate to give up on the esc as it's exactly what I was looking for with my hubs. Torque. Though it took a week to get use to the sensitivity of the remote. Finally got to grips then fail. Spent so many hours on it. My first build! Do you know a way to use a different remote?
```

---
## \#21 Posted by: bartroosen12 Posted at: 2019-02-19T14:01:33.680Z Reads: 42

```
I was looking for a slightly more powerfull esc.
Now I'm using the ownboard esc which does 2x 10A with their hub motors.

I saw this maytech esc 2x30A which is pretty cheap so that would be perfect if it works well?

You can just buy another remote (like the enertion nano remote) or am I wrong?
```

---
