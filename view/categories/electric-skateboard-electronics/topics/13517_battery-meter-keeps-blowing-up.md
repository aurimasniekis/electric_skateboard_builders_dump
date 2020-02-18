# Battery meter keeps blowing up

### Replies: 20 Views: 1390

## \#1 Posted by: Jinra Posted at: 2016-11-23T04:44:53.977Z Reads: 180

```
So I'm getting my third battery meter ([this one](http://www.ebay.com/itm/172143986261?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT)) soon and to avoid blowing it up a third time I'd like to run it by others to see if they can spot where I did something wrong, or if it just happens to be two defective meters.

A couple months ago @longhairedboy recommended the aforementioned meter. I'm pretty sure he used it in his builds as well. I hooked up the meter with positive going direct to battery+ and negative going to to the negative after my DIYES antispark switch. I did this so the meter doesn't turn on when the board is off. To be more accurate, the negative of the meter goes to the XT60 negative of my parallel connector that goes to my two VESCs.

The two blown meters both blew up while riding up a hill causing my board to become unresponsive for 5~ seconds and then act normally again. I'm guessing the meter drew huge current and cause my VESCs to lose power for a second and reboot. It certainly sounds like the meter is blowing up from the higher current draw from going up hill, but I'm unsure why this is since the meter is hooked up in parallel and not in series with my VESCs.
```

---
## \#2 Posted by: TheImmortalJew Posted at: 2016-11-23T05:04:27.705Z Reads: 171

```
I have a very similar meter and did basically the same thing as you. Red to positive, black to negative. Have not had any problems yet. I soldered the meter wires right to the VESC terminals since I cut off the XT90 in place of bullet connectors.

Also, how do you define blowing up? Like smoke and stuff or just dead?  If you have smoke then I think it's definitely your wiring...I had smoke when I put 48V through a 0-30V meter because I wired it incorrectly.
```

---
## \#3 Posted by: Jinra Posted at: 2016-11-23T05:39:53.333Z Reads: 159

```
the larger chip in the back has a burn mark on it and it smelled like burning silicone when I opened up my board. They both have the burn in the same spot. One turns on but doesn't display anything, the other doesn't turn on what-so-ever. I'm assuming there's a bit of smoke when it goes up, but my wiring, in terms of terminals, are correct.

It's worth noting the meter works perfectly fine otherwise, it just hates hills...
```

---
## \#4 Posted by: FredSaberhagen Posted at: 2016-11-23T05:47:33.051Z Reads: 152

```
 could your two separate wires be coupling inductively- Meaning when hill climbing your di/dt get very large and ... what does your main wiring look like, short close wires or long ones with any space between them?  Trace the current path and avoid big loops if possible.

If your voltmeter wires are in close promixity to the power wires, when you hill climb, Induce high di/dt creating a magnetic field, that'll show up as current induced on your meter wires -going into high impedance meter that could create a real high voltage spike (same principle as a wireless charger)

You could put a zener/mov protection device on the wires right by the meter, or route power and meter wires separately , physical isolation is always effective :slight_smile:
```

---
## \#5 Posted by: lox897 Posted at: 2016-11-23T05:55:07.860Z Reads: 144

```
Why don't the wires both go after the antispark switch? That's what most people do I believe
```

---
## \#6 Posted by: Jinra Posted at: 2016-11-23T05:57:11.300Z Reads: 141

```
@lox897 Because I already heat shrinked my XT60's and only wanted to cut into one of the terminals to expose some metal. I wonder if that's somehow causing it to blow.. Maybe the regen current, but how would that be different if i wired it both to the xt60.

@FredSaberhagen here's a very crappy diagram of how it's setup. The orange arrow points to where the negative is plugged into. All fairly short cables, and not **that** close to the battery.

<img src="/uploads/db1493/original/3X/f/a/fa990e4136a9a875c4deff2e076c2ff37fa7cd64.png" width="660" height="243">
```

---
## \#7 Posted by: TheImmortalJew Posted at: 2016-11-23T06:09:28.941Z Reads: 137

```
I would try putting the meter wires on the same side of the switch. So move the positive between the switch and VESC where your negative is. You don't have to cut terminals, just strip off a piece of insulation mid-wire, solder it, and electrical tape.
```

---
## \#8 Posted by: Jinra Posted at: 2016-11-23T06:19:25.430Z Reads: 133

```
I guess I'll try that when I get the replacement, just not sure how it's much different than how it is now.
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-11-23T16:08:52.324Z Reads: 121

```
typically i wire them directly to the ESC side of the e-switch in parallel to the VESCs. Occasioanlly id there is an issue I'll tap them into the wires by slicing a section of insulation off of the wire and soldering it in that way then heat-shrinking the joint, but not usually. 

this is the first I've heard of one popping like that. I wonder what was defective int he unit to make it do that.
```

---
## \#10 Posted by: Jinra Posted at: 2016-11-23T16:21:56.032Z Reads: 117

```
The more I think about it the more it makes sense that maybe the way i had it wired caused it to blow.

Since the positive was direct on battery and negative was on eswitch, when current draw got too high and my main power leads got saturated, perhaps the current overflowed to my meter wire and caused enough current to both the chip on the meter. I'll definitely rewire the replacement.

Thanks all
```

---
## \#11 Posted by: longhairedboy Posted at: 2016-11-23T17:37:18.350Z Reads: 108

```
that's exactly what happened, i'm sure of it. It took me a minute to realize what you were saying about how you had it wired.
```

---
## \#12 Posted by: jmasta Posted at: 2016-11-24T01:03:21.693Z Reads: 90

```
With that particular model, do you know if you can switch the display from percentage to voltage?
```

---
## \#13 Posted by: Jinra Posted at: 2016-11-24T01:30:04.492Z Reads: 86

```
I don't think so, only percentage I believe.
```

---
## \#14 Posted by: FredSaberhagen Posted at: 2016-11-25T07:04:11.063Z Reads: 71

```
That makes no sense to say when current got high you overflowed current into the meter... meters impedance don't change based on the voltage across the two nodes...
```

---
## \#15 Posted by: Jinra Posted at: 2016-11-25T07:08:43.279Z Reads: 72

```
Do you have a better suggestion? That's the best idea I have at the moment to solve this.
```

---
## \#16 Posted by: FredSaberhagen Posted at: 2016-11-25T07:22:04.198Z Reads: 69

```
Your ideas  probably still worth trying !  I just wanted to point out that's not how current works... your GND might be bouncing by picking the wire up further from the battery (high current will  show up as a raised voltage there) .  Can you post a real pic?
```

---
## \#17 Posted by: Jinra Posted at: 2016-11-25T07:28:10.275Z Reads: 70

```
Here you go. That small JST connector is what plugs into the meter. GND goes to the XT60 and red direct to battery+.

<img src="/uploads/db1493/original/3X/9/1/91debedab8a1242f44a767ff263b604fdf1b17b3.jpg" width="375" height="500">
```

---
## \#18 Posted by: FredSaberhagen Posted at: 2016-11-25T07:41:47.757Z Reads: 69

```
Cool it does look tight in there but depending how it's ran when installed I think inductive coupling could still be the culprit.
You could fix it by moving the GND wire over to the pack but still want to keep those meter wires physically separated from the high current power wires .
```

---
## \#19 Posted by: Jinra Posted at: 2016-11-25T07:44:18.848Z Reads: 66

```
The reason the GND is where it is is because I don't want the meter to be on while my board is off. The only way to do this is to have at least one of the meter cables after the switch. I'll move the positive over to the switch as well and see if that helps.

It's going to have to be attached to the high current main power line because of this as well.
```

---
## \#20 Posted by: rtasca Posted at: 2016-11-25T09:01:47.081Z Reads: 66

```
you can try twisting the wires to the meter where possible and /or giving it some turns around a toroid and/or soldering a cap next to the meter.
```

---
