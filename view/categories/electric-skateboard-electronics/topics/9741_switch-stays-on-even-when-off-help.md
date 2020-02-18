# Switch stays on&hellip;. even when off. HELP?

### Replies: 20 Views: 1848

## \#1 Posted by: Raf Posted at: 2016-09-17T11:20:31.435Z Reads: 184

```
Hey guys,

Just plugged in my electronics and turned on the antispark switch. everything is working fine but when i press the button to turn of the antispark switch nothing happens. It just stays on. 

can anyone tell me whats wrong?
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-09-17T11:24:09.404Z Reads: 183

```
Prob your switch to turn it on is busted
```

---
## \#3 Posted by: elkick Posted at: 2016-09-17T11:29:02.764Z Reads: 176

```
Put it in off position, disconnect power and reconnect power again.
```

---
## \#4 Posted by: Raf Posted at: 2016-09-17T11:32:38.890Z Reads: 178

```
tried this.

i used it with one 5s lipo i had and it worked perfectly. on/off but then i connected them 2 5s in series and plugged everything iin. turned it on and now it won't turn off. The switch says it can take up to 60v 14s batteries
```

---
## \#5 Posted by: 2-alex-2 Posted at: 2016-09-17T18:06:46.972Z Reads: 156

```
Wonder if the switch has been soldered the wrong way round.
```

---
## \#6 Posted by: Mobutusan Posted at: 2016-09-18T17:24:11.249Z Reads: 142

```
Did you figure out what the issue is? I've got a @torqueboards switch that is doing the same thing.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-09-18T18:07:49.540Z Reads: 142

```
I had 2 of them that did the same thing. 
I just gave up on them and got a BMS with built in switch. It hasn't failed so far.
```

---
## \#8 Posted by: Raf Posted at: 2016-09-21T20:58:02.811Z Reads: 125

```
the one i using is from @torqueboards  it was working fine but now it doesn't switch off. Ive seen other having problems with these switches. i think they're prone to failing quickly
```

---
## \#9 Posted by: Smashapotamus Posted at: 2016-09-21T21:01:07.414Z Reads: 122

```
This is a common failure with these switches.  I went through 2 torqueboards switches which failed the same way.  Torque is a great guy though and did everything in his power to take care of me.  You should contact him.

I found the Vedder/Fechter switch to be much more reliable, especially at higher voltages.  I still have a torqueboards switch that was given to me as a replacement.  I use it on a lower voltage system and it hasn't failed me yet.
```

---
## \#10 Posted by: Raf Posted at: 2016-09-21T21:02:47.056Z Reads: 116

```
yeah i dotnt think they work at high voltages even though it says up to 14s it think its probably 6s max
```

---
## \#11 Posted by: Namasaki Posted at: 2016-09-21T22:39:02.890Z Reads: 107

```
My first switch failed after a long ride. It got really hot. 
My second failed within 5 min after powering it up.
Both times on 12s
```

---
## \#12 Posted by: torqueboards Posted at: 2016-09-22T15:37:10.954Z Reads: 100

```
Odd how you are all having issues with the switches. I use these switches religiously on 10S/12S all day, everyday. I'm working on re-designing another which will hopefully be better.
```

---
## \#13 Posted by: evoheyax Posted at: 2016-09-22T16:15:53.737Z Reads: 98

```
I had one of @torqueboards switches fail after using it for a week. I ordered another one, and it broke 30 seconds I hooked it up. I was extremely careful to not short circuit anything and I did not. I turned it off and on 2 times, it worked, then 10 or 15 seconds later while in the off position, it turned back on and never turned off again, just like the first one... I have stopped using them and now turned to @JdogAwesome's power switch, as I can't keep dumping money into a bad power switch.

Do your manufacturers use counterfit fets?

It really doesn't make sense why they break instantly like this, and having spent $100 on power switches to not have one working when I've done nothing to break them is frustrating...
```

---
## \#14 Posted by: denton Posted at: 2016-11-19T21:00:23.774Z Reads: 82

```
I have this same switch, and it has worked for months, then I go for my first ride and it just stays on. It's not the switch either because I have wired in a new switch and it doesn't change how it works. Is it a problem with the relay?
```

---
## \#15 Posted by: Ackmaniac Posted at: 2016-11-19T21:19:36.961Z Reads: 82

```
One of mine also failed after I connected it to the battery while it was switched off. Somewhere in the forum somebody mentioned that this can be caused by a short power burst when you connect it which can damage the mosfetts. So what I do since then. When I disconnect the battery and connect it again I use a 4,7K Resistor first to  close the circuit and then I connect the real power wires. Could be difficult if you have no access to the batterys +-.  But if you have the space you can add a xt90 anti spark in between the battery and the switch. Or you take the balance leads to connect it with the Resistor.  Since I do that the switch didn't break anymore. But it also only happened once to me so you can't really say that this fixed the issue permanently. Maybe I am also wrong.
```

---
## \#16 Posted by: denton Posted at: 2016-11-19T22:43:00.924Z Reads: 79

```
I tried several things and it doesn't turn off the switch....
But while riding it just shuts off power to the motors, but the light stays on the switch. I disconnected it and reconnected it and the board worked again. But the battery switch never "turned off" meaning it still illuminated the blue light in the power button itself.
```

---
## \#17 Posted by: Ackmaniac Posted at: 2016-11-19T22:55:22.573Z Reads: 80

```
It was the same for my broken one. You can't turn it off anymore.
```

---
## \#18 Posted by: Kostya Posted at: 2016-12-15T07:07:59.172Z Reads: 64

```
Hey guys I have the same problem  with the switch. And seems like these switches are bad Just a small question 
is it okay to just leave it connected  as it is on the  board. I don't mind to disconnect the batteries. Or will the broken switch damage my board ? @evoheyax?
```

---
## \#19 Posted by: Kostya Posted at: 2017-09-14T21:33:38.712Z Reads: 47

```
Anyone there ?'
```

---
## \#20 Posted by: DaveMess Posted at: 2017-09-14T21:59:01.588Z Reads: 42

```
Holy old post, Batman.

Leaving batteries connected to an antispark switch will eventually drain them. It's fine to ride until you're batteries are depleted, just don't leave them hooked up too long or you'll over discharge them. Just make sure to charge your board that evening.
```

---
