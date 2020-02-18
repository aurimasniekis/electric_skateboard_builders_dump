# Throttle cut after battery level drops under acceleration

### Replies: 16 Views: 265

## \#1 Posted by: drangboards Posted at: 2019-07-16T22:20:35.181Z Reads: 88

```
I have a stock raptor set up on my board.  New Unity, new BMS, new connections shrink wrapped on the motor wires.  I also changed to the mini remote, and all seems well until this happens. 

With the app open and the phone in my hand, watching, as I accelerate, the battery meter goes down over the course of 5 or so seconds to basically zero, and then throttle cuts out for a second.  It also seems that bumps in the road cause this to happen almost any time (if the bump gives enough jolt to the board or battery).  Is my battery dead?  How can I test this?  Could it be a problem with the BMS or settings in unity?  Keep in mind this is a new unity with the new firmware. ..  

Could the problem be one of the motors?  One of the motors reads about 10 celsuis higher than the other motor before riding. 

The battery has been taking longer and longer to charge from 90-100 percent.
```

---
## \#2 Posted by: Vero Posted at: 2019-07-16T23:36:59.524Z Reads: 81

```
sounds like a loose nickel connection in the battery
```

---
## \#3 Posted by: drangboards Posted at: 2019-07-16T23:55:38.134Z Reads: 82

```
That's all I needed to hear, (others have agreed) so I'll be stripping off the battery casing, and looking at them all, and probably fixing whichever one is wrong.  Would it be ok to immediately ride the board after that, or should I charge again first?
```

---
## \#4 Posted by: goldrabe Posted at: 2019-07-17T00:06:09.791Z Reads: 80

```
Sounds like your battery. Either broken Nickel as mentioned loose battery leads and / or bad P group and cells. First check your Voltages at the BMS balance plug here is a video of how to do this.

https://www.youtube.com/watch?v=6i8i6h1LkBw
Don´t charge or discharge your battery, doing so with dead cells can lead to fire.\
I am not familiar with the space cell BMS or pack design, @barajabali is one of the most knowledgeable persons to ask here.
```

---
## \#5 Posted by: drangboards Posted at: 2019-07-17T01:09:50.065Z Reads: 73

```
Well ok then sheesh, I thought this was going to be easy lol...  So watching the video until I understand more, and if @barajabali wantsta chime in, that would be nice.  I still owe him my two bad BMS units...
```

---
## \#6 Posted by: robthebuilder Posted at: 2019-07-17T05:32:06.468Z Reads: 55

```
It's quite simple :) You just messure each pin on the connector that plugs the batteryleads into the BMS. The first pin should read something between 3.7 - 4.2 V. The next pin should be the same value added on top of the first one.

An example:
If the first pin shows 4V, then the next pin should read 8V and the next 12V and so on. If they differ in like 0.1V it's not a problem but if the difference is big there might be something wrong with the cell or the connection.

Hope that helps :)
```

---
## \#7 Posted by: drangboards Posted at: 2019-07-17T13:58:24.880Z Reads: 41

```
That very much does help.  I have a dude coming over today to help, I think he's going to do the heavy work while I do my job.
```

---
## \#8 Posted by: drangboards Posted at: 2019-07-17T19:08:37.795Z Reads: 39

```
So this means I don't have to rip into my battery wrapping yet eh
```

---
## \#9 Posted by: robthebuilder Posted at: 2019-07-18T08:42:07.419Z Reads: 36

```
Well, not if everything is all good :) But something must be wrong somewhere with the issues you're having. Might also be a bad solder on the big leads that can't hold up during heavy amp loads.
```

---
## \#10 Posted by: robthebuilder Posted at: 2019-07-18T08:46:45.589Z Reads: 38

```
But I guess the easiest thing would be to check all the strips on the pack. Is it soldered or welded?
```

---
## \#11 Posted by: drangboards Posted at: 2019-07-18T19:06:22.669Z Reads: 25

```
I'm not sure, it's just a stock raptor 2.1 battery, latest model as far as I can tell.
```

---
## \#12 Posted by: robthebuilder Posted at: 2019-07-19T10:36:25.123Z Reads: 21

```
Oh, ok! Thought it was a DIY battery. I guess I didn't read your post as well as one would've hoped :P 

Then it's welded for sure. I don't know much about their batteries but i guess they use 18650 cells in a 10SxP config. Someone else with experience with these batteries might be able to help you better!
```

---
## \#13 Posted by: drangboards Posted at: 2019-07-19T15:02:20.060Z Reads: 18

```
Yeah 10s4p.  @barajabali do you have the inputs I'd need, or has everything been covered?
```

---
## \#14 Posted by: barajabali Posted at: 2019-07-19T15:03:25.940Z Reads: 17

```
Inputs for the tool?
```

---
## \#15 Posted by: drangboards Posted at: 2019-07-19T15:04:18.428Z Reads: 16

```
Input for the diagnosis, or opinions on potential issues, based on your experience.
```

---
## \#16 Posted by: drangboards Posted at: 2020-01-18T23:29:07.838Z Reads: 7

```
Found the problem. 15 of the 40 batteries have a negative terminal disconnected at the weld. I'll go ahead and say that this isn't enertion fault as the deck is custom and it probably has a bit more deflection than the stock raptor. ![15793897758359180038462611330999|666x500](upload://1Nbx35gEmXTJzNxl1uD9XdkhkAF.jpeg) 

Being saved by my buddy Stephen. I'll be ripping again soon. Glad I have this board and I dont care what's going on with enertion. I hope they make it out of their mess and look into new deck designs and want me to design them.
```

---
