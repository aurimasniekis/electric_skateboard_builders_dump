# LCD battery capacity meter issues

### Replies: 9 Views: 293

## \#1 Posted by: Songsta Posted at: 2019-02-10T05:08:35.702Z Reads: 89

```
I’m trying to figure out 2 things about this meter:

1. What are the high and low voltages it uses to measure percentage, i.e. high is probably 4,2v but low is ???
2. How the heck do I get it to permanently stay on the mode where it shows voltage rather than percentage? I can change the modes, but when I remove my loopkey and then connect it again, it defaults back to percentage. 

I initially thought that the percentage would be based on what I had set as the minimum voltage on the VESC, but I’ve realised it doesn’t work like that. There is a high and low voltage setting programmed into the Meter, based in the battery type and the size. 

I’m going to try work out the answer to the first question by noting the percentage as it decreases and check this against  what the VESC Mobile app is giving for battery capacity at the time. 

The other question I have: are there better alternatives to this meter?

http://www.trampaboards.com/lcd-12v-lithium-battery-capacity-indicator--blue-screen-p-25093.html
```

---
## \#2 Posted by: dareno Posted at: 2019-02-10T07:31:25.470Z Reads: 72

```
Looks just like the generic meter everyone uses but in a different case.  You do have to tell it what series count you are using.  As for the percentage come voltage there is no way to lock in the voltage but if you depress the set button at the back after the initial set up for some reason or witchcraft it toggles between the 2.  Don't ask me why but thats what happens on one of my set ups where everything is squeezed in there tight as.  Alternatively you could use a remote voltage meter ala @mmaner which I believe he will be chucking on thingimajig
```

---
## \#3 Posted by: Andy87 Posted at: 2019-02-10T07:36:25.132Z Reads: 68

```
That’s a nice option too
https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509?u=andy87
```

---
## \#4 Posted by: ShutterShock Posted at: 2019-02-10T08:59:40.011Z Reads: 56

```
This is the one I have used on all of my builds and I think the full should be 4.2 as long as you set it to the "P" version of the things it can measure.

I believe that its low is the rating for a low on a liion cell, so probably 3.0, but I cut my boards off at 3.4 for my lipos, so it usually is dead at around 15%
```

---
## \#5 Posted by: pat.speed Posted at: 2019-02-10T11:15:18.141Z Reads: 42

```
The P stands for lead acid no? As in Pb. I thought lithium was L or maybe it was S
```

---
## \#6 Posted by: J0ker3366 Posted at: 2019-02-10T13:38:00.614Z Reads: 36

```
@pat.speed is correct. P stands for lead acid and L stands for li ion. Each number under L should be your series packs. 1s, 2s, 3s and so on.
```

---
## \#7 Posted by: Songsta Posted at: 2019-02-10T14:10:42.362Z Reads: 35

```
Yeah, I know it toggles between the 2 but I want it to stay on Volts. 

[quote="Songsta, post:1, topic:83774"]
I can change the modes, but when I remove my loopkey and then connect it again, it defaults back to percentage.
[/quote]
```

---
## \#8 Posted by: ShutterShock Posted at: 2019-02-10T19:07:49.671Z Reads: 27

```
Oh right I was rememebering it wrong.  The lead acid goes up to 4p and then it switches to 1s to 12s I think
```

---
## \#9 Posted by: J0ker3366 Posted at: 2019-02-10T19:11:04.783Z Reads: 25

```
[quote="Songsta, post:7, topic:83774"]
back to percentage
[/quote]

I believe thats just programming. Ive had ones that wont change and ive had some that will change. Its nothing but a push of a button but i understand how that becomes redundant
```

---
