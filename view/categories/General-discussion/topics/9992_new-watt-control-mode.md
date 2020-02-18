# New watt control mode

### Replies: 6 Views: 742

## \#1 Posted by: Ackmaniac Posted at: 2016-09-22T18:32:26.441Z Reads: 181

```
I was wondering why my board does full power at higher speeds. This means it does full power already at 40% throttle. I calculated a bit and looked at the sourcecode of current control and found out that the faster you go the more throttle control you loose. That means depending on your settings you might only have half the throttle to control  the board at higher speeds. 
Because of that I created a new mode which I call Watt mode. So you have control about the watts at higher speeds. 90% throttle means only 90% of the available watts. This way it is easier to carve at higher speeds because the throttle is not so aggressive. 
I also needed to mix it with current control so that it ramps up by the current until it reached the wanted watts. 
The first time the board feels less powerfull because you need to pull the trigger more at higher speeds. But after a while you get used to it. And it is easy to reduce the power for other riders because you can simply choose the watts you want. 

My question is if the community is interested in a bldc tool and firmware mod from a third person where the watt control can be choosen and adjusted. Because if nobody wants it I don't need to invest in the time to build it.
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-09-22T18:45:58.027Z Reads: 168

```
What TX do you use?
```

---
## \#3 Posted by: Hummie Posted at: 2016-09-22T19:10:57.107Z Reads: 156

```
sounds nice but current control has been great to me so far.
```

---
## \#4 Posted by: elkick Posted at: 2016-09-22T19:33:05.107Z Reads: 147

```
It would be easier if you'd implement this on FW 3.1 though I guess.
```

---
## \#5 Posted by: Ackmaniac Posted at: 2016-09-22T19:42:06.910Z Reads: 141

```
That's true. Maybe I should wait until Benjamin brings out the vesc-tool (new version of bldc-tool).
```

---
## \#6 Posted by: Namasaki Posted at: 2016-09-24T06:18:20.908Z Reads: 87

```
It's open source to encourage very intelligent people like you to help it evolve. So why wouldn't everyone be interested in your idea. Wether it's better or not doesn't matter. It's a new idea. Share it.
P.S. it wasn't that long ago when current control was a new idea.
```

---
