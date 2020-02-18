# Help with 30Q battery lay out

### Replies: 10 Views: 975

## \#1 Posted by: red Posted at: 2017-11-26T16:38:53.683Z Reads: 136

```
hello this is my first post so apology in advance.
I have 28 Samsung INR18650-30Q 3000mAh - 15A and need some help i dont really know what way to configure them i understand series and parallel connection. i just dont understand the best way to but them together. Im using the vruzend diy kit reason being i want to be able to take the battery apart when going on a plane so that i will be under the 99wh limit. basicly what is the best volts to amp lay out. im going to have duel hubs not sure what size yet as diy e.s is sold out of hubs.i weight 85kg and wont be going up any steep hills any help on this matter would b greatly appreciated. i hope this post was not to obscure. i have some pics.if there is a post explaining what im talking about please point me in the right direction<img src="/uploads/db1493/original/3X/b/b/bbb95c7036473af01856aa62eb0258c6eeeb5307.jpg" width="669" height="500"><img src="/uploads/db1493/original/3X/c/a/ca3261ba82fc90d890e1e2049efd83bf9185028b.jpg" width="669" height="500">.
```

---
## \#2 Posted by: BoostedBuilder Posted at: 2017-11-26T16:58:21.338Z Reads: 127

```
What hubs are you using?
I would say 9s3p. You will leave 1 cell behind but that gives you 99.89wh x 3.

EDIT: Just re-read what you wrote. Most hub motors are around 80Kv so if you want speed, 9s3p, if you want torque, 7s4p.
```

---
## \#3 Posted by: jmasta Posted at: 2017-11-26T17:37:12.812Z Reads: 124

```
Those VRUZEND battery builders are cool. But can they handle the currents we need?  Maybe you could use two or three strips on top?

> _How much current can the terminal caps support?_

> _So far the caps have been tested and confirmed to **withstand up to 3.5 A of current each**. However, we are quite confident that they can carry higher levels of current and will testing this further soon!_

http://vruzend.com/faq/#how-much-current
```

---
## \#4 Posted by: Jammeslu Posted at: 2017-11-26T17:52:40.062Z Reads: 114

```
thats the old style with steel bars. the new one is suposed to have nikeltinned copper
```

---
## \#5 Posted by: red Posted at: 2017-11-26T18:56:28.257Z Reads: 109

```
ok thanks a lot bro  its starting to become a bit clearer to me now thanks. its the way to lay that out thats tripping me up so ill be doing  9s3p when i connect the 3p+ to the next 3p - { which is upside down} which add up the volt of each set of 3p does that add the mah also.as in each set of 3 will be 3.6volts and 45A  or 9ooomah so this set up will give me a 32.4volt and 81000mah or 405A battery? like this pic sorry i know its bad. thanks for the help <img src="/uploads/db1493/original/3X/4/7/47c5ea8b9366f63ea61badb2718144669210bfa4.jpg" width="669" height="500">
```

---
## \#6 Posted by: red Posted at: 2017-11-26T18:57:22.869Z Reads: 104

```
ya think ill have to solder them. thanks pal
```

---
## \#7 Posted by: thisguyhere Posted at: 2017-11-26T19:11:57.102Z Reads: 100

```
[quote="red, post:5, topic:39341"]
32.4volt and 81000mah or 405A battery
[/quote]

no.

parallel group will multiple capacity and continuous discharge.  serial count will multiply voltage.

your 30q cells have 3000mah capacity, are safe up to 20amp continuous discharge, and are 3.7v nominal.

in 9s3p, voltage will be 9s*3.7v, so pack voltage will be 33.3v nominal.

the 3p will set your capacity to 9000mah (3000mah per cell * 3p), and continuous discharge to 60a (20a per cell * 3p).

watt hours is voltage * amp hour, so 9s3p pack will be 300Wh. ((33.3 * 9000) / 1000)

like @jmasta mentioned, you will severely limit current flow with vruzend.  either you'll have to limit batt max in the vesc to 15a, in which case it's pointless to use 30q cells.  or risk overheating the caps, which causes a whole host of issues.

check here, there is no shortage of how to wire up a pack:
https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179
```

---
## \#8 Posted by: longhairedboy Posted at: 2017-11-26T19:43:21.303Z Reads: 88

```
i drew that off the top of my head as a doodle in a meeting. 

That's how elegantly simple esk8s are. You can do that.
```

---
## \#9 Posted by: red Posted at: 2017-11-26T20:58:20.385Z Reads: 74

```
Thanks thisguyhere you just blow my mind makes a lot of sense now.thanks for the link its got a lot of useful stuff.
```

---
## \#10 Posted by: red Posted at: 2017-11-27T22:51:05.972Z Reads: 54

```
when connecting the parallel could i connect each cell of 3  using 12 AWG so i could just break the solder or find some sort of connector for easy disassembling  for traveling on planes. also do i need just one contact between each set of 3 as they are now 1 cell not 3? this is what im thinking of doing  (see pic) or would i have to connect each +/- of each 3.7 cell?<img src="/uploads/db1493/original/3X/0/5/05d87025f7c64cafddc9bdd51ab594019495cdb5.jpg" width="281" height="500">
```

---
