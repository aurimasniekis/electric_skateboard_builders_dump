# Struggeling to get good reliability with the mini remote

### Replies: 7 Views: 216

## \#1 Posted by: aMasheep Posted at: 2018-10-14T21:28:35.468Z Reads: 88

```
Hello!
This summer I've been building my eMTB(which I will soon publish in the builds section), but I am struggelig with signal dropout from the remote!

I have been reading and googeling a lot about this, but hasn't found anything that works. I am struggeling with the mini remote, that in 2.4ghz congested areas, I loose connection, and have to hold it right next to the reciever to get signal again. 

Does any one of you have experience in this, and can tell me what to do? Where should I place the reciever for example? Might it be a bad idea to have it next to the ESC? and if so, how far away?

Hope someone have some tips.
Best regards!
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-10-14T21:34:43.943Z Reads: 85

```
from what I've read, if you have a carbon fibre enclosure there are connection issues, as well as if you put the receiver near the phase wires of the esc. that's all I've heard
```

---
## \#3 Posted by: dareno Posted at: 2018-10-14T23:55:49.902Z Reads: 67

```
That just goes to prove my theory that all remotes experience issues in certain environments.  The mini is supposed to be the exception to that rule.  
I always position my receiver mid way down the deck away from everything.  Never had an issue of drop out regardless of where I ride.  I use maytech and nano and benchwheel.  All fine.  
are you talking about this one?
![image|225x225](upload://3fvzrTaNn12aWCFNnZnQoSC0Vgh.jpeg)
```

---
## \#4 Posted by: b264 Posted at: 2018-10-14T23:59:25.287Z Reads: 62

```
Mini remote seems to be rock-solid.  What deck do you have?
```

---
## \#5 Posted by: J0ker3366 Posted at: 2018-10-15T00:01:51.821Z Reads: 61

```
[quote="dareno, post:3, topic:71239"]
Never had an issue
[/quote]

Have the mini as well and it sits side by side the focbox at the rear of the enclosure. So far I've found one place that I get a repeated cutout. Do some searching on switching buad. Its used regularly in rc for comp racing so no two rc vehicles are on the same buad. I'm sure it already been done but if not it shouldnt be that hard to implement to our applications.
```

---
## \#6 Posted by: Badgermilk Posted at: 2018-10-15T02:28:27.031Z Reads: 45

```
I was having issues with my mini dropping signal. I turned on the remote and jiggled the signal, ground, and pos wires at the receiver and noticed that the light would go off.  Poor wire connection at the receiver was the problem I think. It may have been the terminal block was loose. I used a liberal amount of hot glue, and the problem was fixed. I hope you figure it out. Signal drop is super dangerous.
```

---
## \#7 Posted by: aMasheep Posted at: 2018-10-15T05:56:41.406Z Reads: 36

```
Yes, it is that one. I should try to position the reciever otherwise. At the time of speaking, it is right next to my ESC, with the antenna running over the phase wires. I will first try to make a new enclosure and put the antenna just a little bit off. I've tried having it on the outside of the box with no luck, but I haven't tried moving it away from it.

[quote="mynamesmatt, post:2, topic:71239, full:true"]
from what I’ve read, if you have a carbon fibre enclosure there are connection issues, as well as if you put the receiver near the phase wires of the esc. that’s all I’ve heard
[/quote]
Thanks for the tip! I have a PLA enclosure, but it is damn close to the phase wires. I guess I should try moving it away.

[quote="b264, post:4, topic:71239, full:true"]
Mini remote seems to be rock-solid. What deck do you have?
[/quote]
I have the deck from the standard MBS Atom 90, eco MTB. How does the deck affect the signal when the reciever is on top of the deck?

[quote="J0ker3366, post:5, topic:71239"]
Have the mini as well and it sits side by side the focbox at the rear of the enclosure. So far I’ve found one place that I get a repeated cutout. Do some searching on switching buad. Its used regularly in rc for comp racing so no two rc vehicles are on the same buad. I’m sure it already been done but if not it shouldnt be that hard to implement to our applications.
[/quote]
Hello! I have searched a bit on how to change this baud rate, but I can't find anything, would you mind guiding me a little more on where to find it? Best regards.

[quote="Badgermilk, post:6, topic:71239, full:true"]
I was having issues with my mini dropping signal. I turned on the remote and jiggled the signal, ground, and pos wires at the receiver and noticed that the light would go off. Poor wire connection at the receiver was the problem I think. It may have been the terminal block was loose. I used a liberal amount of hot glue, and the problem was fixed. I hope you figure it out. Signal drop is super dangerous.
[/quote]
Yes it's quite dangerous.. At least when riding downhill. The wire connections was a issue before, but this time it is not. I can ride in the woods a long time, and when I get down to the city again, it starts cutting out in the most congested areas. But thanks for the tip! I am considering soldering all connections when I am done with the board.

Thanks a lot everyone for the good replies. I have new hope for my board now! :smile:
Best regards
```

---
