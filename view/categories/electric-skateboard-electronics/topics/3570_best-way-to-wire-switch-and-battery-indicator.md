# Best way to wire switch and battery indicator

### Replies: 4 Views: 2446

## \#1 Posted by: Johan Posted at: 2016-05-20T21:58:47.330Z Reads: 299

```
Hi does anyone know the best/safest way to wire a switch and battery indicator?
<img src="/uploads/db1493/original/2X/4/407b35b9b9a4eddb8c36a394074d5b9e6ff23d8e.png" width="166" height="125">
<img src="/uploads/db1493/original/2X/8/8567567c8355ea4e2f9dae6ebf168e1777198754.png" width="150" height="150">

What I was thinking is to wire the custom switch instead of the two existing switches on my two esc's.(not VESC)

And the battery indicator, should it just be connected on to the existing battery wire in parallel? I'm not very skilled in electronics but it seems to be a bad idea to have the current flow through the battery indicator.

Thanks for the help.
```

---
## \#2 Posted by: evoheyax Posted at: 2016-05-21T05:42:43.167Z Reads: 274

```
Switches, you'll need a mechinism for storing a state, or physically cutting the power, and those little guys are usally rated at 12v. You can using solid state switches, like DIYs switch does. That allows you to plug in a switch like that to the small solid state brick, which physically breaks the connection. These are the best option I've come across.

On the topic of battery indicator, It seems like it should break, but I've been told they have basically infinite resistance, so they don't break. I use it in line, between batteries and esc (+ from lcd to + inline, - from lcd to - inline). But you need to get one for the right voltage and battery type. So read the fine print when buying one.
```

---
## \#3 Posted by: seanpain4 Posted at: 2016-05-21T05:59:19.474Z Reads: 268

```
So you mean have the ability to turn both ESCs and your volt meter on with one switch? 

If so, you will need a Triple Pole Single Throw switch. 

<img src="/uploads/db1493/original/2X/6/675602d78e15f0c5039130c65616364a210e6340.jpg" width="96" height="114">

You would wire it up by connecting once ESC to one set of terminals, the other ESC to the next set of terminals, and the volt meter to the last pair of terminals. Then you can turn them all on with one switch and they won't interfere with each other.
```

---
## \#4 Posted by: lowGuido Posted at: 2016-05-21T10:33:33.277Z Reads: 253

```
I have wired all my esc and lipo alarm to one breaker. Diagram is here.
http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/4
```

---
