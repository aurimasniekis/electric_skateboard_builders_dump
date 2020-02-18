# Nobody told me it would be like this

### Replies: 24 Views: 1340

## \#1 Posted by: falesias Posted at: 2018-03-31T10:22:44.903Z Reads: 312

```
![image|666x500](upload://wYW8GB2vQJWUTztDIpxf6hGQqxV.jpeg)

After 4 months waiting, it’s finally here:
My Enertion foc boxes 
Well, gess what...?
It does not fit the motors! (Or the motors don’t  fit the foc boxes)
Any you guys had this problem ever? 
How do you get around this?
I would appreciate any help you guys can give me
Thanks
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2018-03-31T10:25:44.251Z Reads: 307

```
Yep, this was a huge pain in the ass.
So much so that I just went unsensored. I know @psychotiller sells adaptors though
```

---
## \#3 Posted by: falesias Posted at: 2018-03-31T10:27:23.533Z Reads: 309

```
Ok 
thanks man 
I’m going to try to reach him...
```

---
## \#4 Posted by: Sebike Posted at: 2018-03-31T10:27:56.354Z Reads: 301

```
For the sensor wires you usually need an adapter unless you're soldering directly onto the focbox connection.. There are a few people on here selling those adapters I believe. 

Focbox comes with 3.5mm bullets on phase wires, while some motors have 5.5mm plugs. Either you switch bullets on vesc side (and possibly void warranty) or you switch on motor side or use adapters. 

Only the sensor wire that doesn't fit on your setup? 

Good luck
```

---
## \#5 Posted by: ARetardedPillow Posted at: 2018-03-31T10:29:47.805Z Reads: 291

```
Here's the link btw!
https://psychotiller.com/product/sensor-wire-adaptor
```

---
## \#6 Posted by: falesias Posted at: 2018-03-31T10:41:11.187Z Reads: 283

```
Thanks Sebike,
Yes that it’s true, the bullets are also different 
But I gues that’ an easier fix, right?
The sensor cable with so many wires is more complicated.
I already sent a message to the adapter seller...
Regarding the bullets...
Now that I am looking at it, how do you know witch is witch, if all the 3 fase wires are black?
```

---
## \#7 Posted by: bigben Posted at: 2018-03-31T10:44:50.682Z Reads: 275

```
I f you are eu based, this is the place or Streetwing in the UK.
http://www.faradaymotion.com/cables-connectors/49-vesc-motor-hall-sensor-cable-20-cm.html
```

---
## \#8 Posted by: falesias Posted at: 2018-03-31T10:45:37.094Z Reads: 259

```
Ok, thaks
will place an order 
Hope it doesn’t take long to get here, I’m in Portugal 🇵🇹
```

---
## \#9 Posted by: e.board_solutions Posted at: 2018-03-31T10:50:47.779Z Reads: 258

```
Hey, I'm from belgium, I have them to :slight_smile:
```

---
## \#10 Posted by: falesias Posted at: 2018-03-31T10:59:55.876Z Reads: 249

```
Hi 
Thanks 
Even better! 
From Europe and cheaper 
I just ordered 

Thanks again
```

---
## \#11 Posted by: e.board_solutions Posted at: 2018-03-31T11:15:40.187Z Reads: 232

```
You ordered from psychotiller you mean?
```

---
## \#12 Posted by: Blitz Posted at: 2018-03-31T11:19:55.215Z Reads: 222

```
Nah I think he ordered from the link @bigben Shared
```

---
## \#13 Posted by: Lobap Posted at: 2018-03-31T11:24:14.388Z Reads: 220

```
Which member owns that website? Might be interested in few things, need to PM.

Thanks
```

---
## \#14 Posted by: falesias Posted at: 2018-03-31T11:28:05.592Z Reads: 212

```
Hi
Thanks for your answer but I had just ordered from bigben link...
```

---
## \#15 Posted by: Acklavidian Posted at: 2018-03-31T11:31:49.933Z Reads: 215

```
[quote="falesias, post:6, topic:50764"]
Now that I am looking at it, how do you know witch is witch, if all the 3 fase wires are black?
[/quote]

I'm also wondering this
```

---
## \#16 Posted by: falesias Posted at: 2018-03-31T11:34:22.283Z Reads: 211

```
![image|666x500](upload://4qXe7u4vPZ4YZ2nLVKUzbZVPUF9.jpeg)
One more question:
The motor has 3 phase wires
1 red 1 blue 1 yellow 
The focbox has all 3 black wires
How do you know witch is witch?
Or this means you can conect randomly?
Once again, I would really appreciate your comments 
Thanks
```

---
## \#17 Posted by: DavidBanner Posted at: 2018-03-31T11:40:48.746Z Reads: 209

```
The FOCBOX (and VESCs) will automatically detect which phase lead is connected to which phase and take care of all of that for you...

Just plug them in and do the motor detection and you are good to go
```

---
## \#18 Posted by: deucesdown Posted at: 2018-03-31T13:34:34.732Z Reads: 188

```
The deal is, connect them randomly and if the motor spins in the wrong direction, switch any 2 of the wires around. That will change the direction of spin.

Sometimes if sensor detection fails, especially in BLDC mode, rearranging the motor connections may help.
```

---
## \#19 Posted by: falesias Posted at: 2018-03-31T13:40:34.040Z Reads: 187

```
Thaks for your help 
I really appreciate it
Will do so
```

---
## \#20 Posted by: falesias Posted at: 2018-03-31T13:58:35.411Z Reads: 184

```
Thanks for your help

Now that you mention it,
In a dual motor setup, if motors are mounted each one facing opposite sides, then you will have to set them up to turn in opposite directions, so when you mount them, the wheels will turn in the same direction, I guess.
```

---
## \#21 Posted by: Apolo Posted at: 2018-04-01T05:56:22.661Z Reads: 137

```
That's correct
```

---
## \#22 Posted by: falesias Posted at: 2018-04-10T16:27:02.167Z Reads: 117

```
Got it!
Cables from Faraday Motion are here.
Thanks![image|375x500](upload://937wMuyRxkQhXhrPooDO8MbfgDp.jpeg)
```

---
## \#23 Posted by: Toughook Posted at: 2018-04-10T19:25:39.768Z Reads: 84

```
This thread about the phase wires has saved me asking the same question 😂 The wire diagram doesn't say which wire goes where and I was guessing it didn't matter, but always nice to see it 'in print' 👍
```

---
## \#24 Posted by: longboardshort Posted at: 2018-04-12T20:20:47.644Z Reads: 62

```
DOES void warranty... pissed me off when I found that out.  Would rather be pissed on than off and re-doing bullet connectors. :rofl:
```

---
