# First Board, Just want to Confirm Wiring Schematic and Amperages Across The System

### Replies: 14 Views: 1860

## \#1 Posted by: JuniorPotato93 Posted at: 2016-07-20T23:53:25.886Z Reads: 137

```
Alright, so I abused the hell out of the search function on this place and I'm fairly certain I got it right (hopefully.. powerpoint was being a little prick about everything) but I'd be silly to assume that without confirming with my more experienced peers. Am I good to go once all my stuff comes in or do I need to fix something that has gotten past me? One thing I'm not certain about is if this wiring works with regenerative breaking, I found [this](http://www.electric-skateboard.builders/t/vesc-regen-breaking-with-a-bms/504/2) post about it where this was stated by @lowGuido 

> "the BMS should have: 
> +ve terminal that connects to the most positive of the cells.
> -ve terminal that connects to the most negative of the cells.
> "managed -ve" which is the negative terminal that you connect to your load (VESC) and also the negative terminal for your charger.
> then it will have a lead for the +ve terminal of every individual cell in the battery."

From what I can make out, the [BMS](http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html) I'm planning on using doesnt have two -ve terminals where one is the managed one, unless that is what N is though I have yet to see any posts where people utilize it. 
I feel like the answer is yes this circuit is okay because a back current from the VESCs would be equivalent to current coming in from the charging port, but if someone would confirm that I would appreciate it.

<img src="/uploads/db1493/original/2X/a/a542d7722833198d40a4c80380038b735a0336d4.jpg" width="690" height="388">

Updated Schematic Below
<img src="/uploads/db1493/original/2X/b/b84b7ab0b82c32f0134db0d6ac98d0cc642051c9.jpg" width="690" height="388">
```

---
## \#2 Posted by: lowGuido Posted at: 2016-07-21T00:01:31.417Z Reads: 127

```
[quote="JuniorPotato93, post:1, topic:6395"]
From what I can make out, the BMS I'm planning on using doesnt have two -ve terminals where one is
[/quote]

not every BMS features the main negative and the managed negative, a lot of the more common ones are just using the same managed -ve for the main.
```

---
## \#3 Posted by: Jinra Posted at: 2016-07-21T00:01:53.352Z Reads: 123

```
Why do you have an anti spark XT90 and an anti-spark switch? Seems redundant. I'm not sure you're running the voltmeter correctly; I'd imagine you'd want the red lead going to the red wire after the anti spark switch and have another positive wire from the battery to the switch.
```

---
## \#4 Posted by: JuniorPotato93 Posted at: 2016-07-21T00:29:45.563Z Reads: 114

```
I already have them from an attempt at a key loop but really it's there should I have left the toggle switch in on or if it got switched accidentally while the battery pack was out of the board. Although now that i'm writing this I see your point. Even IF it got switched into the On position accidentally, connecting the battery pack to the live circuit would be equivalent to turning the Anti-Spark switch On. Okay I'll remove it since I'd have to make an adapter for it anyways.
```

---
## \#5 Posted by: JuniorPotato93 Posted at: 2016-07-21T00:31:18.583Z Reads: 107

```
Perfect, just for my knowledge, what would be the benefit of having both? I'm getting the BMS I linked anyways but for future reference.
```

---
## \#6 Posted by: JuniorPotato93 Posted at: 2016-07-21T00:38:18.605Z Reads: 104

```
I see what you meant with regards to the Voltmeter. Right now it's on its own circuit, bypassing the VESCs but I should be running it in parallel to the main circuit instead. Though I probably should have googled this before but Volts is constant in a parallel circuit, so the red wire leading tot he voltmeter will remain the same and the black wire coming off of it will link back to the wire going towards the P on the BMS.
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-21T00:43:42.616Z Reads: 99

```
If you do that, the voltmeter would be constantly on. You probably want it after the switch.
```

---
## \#8 Posted by: JuniorPotato93 Posted at: 2016-07-21T00:56:30.343Z Reads: 87

```
Ah, yes. Good point. Will put it to the positive leads after the switch.  With regards to the amperages, am I okay with not blowing any fuses? I'm not really interested in crazy accelerations and there's not a lot of hills around, I'm interested in cruising, 20 amps per motor seems likes it's still a very decent amount.
```

---
## \#9 Posted by: Jinra Posted at: 2016-07-21T01:12:15.878Z Reads: 86

```
Personally, Id give the motors a little more headroom and do 40A per motor. You could install a fuse in the circuit as well.
```

---
## \#10 Posted by: lowGuido Posted at: 2016-07-21T01:25:05.622Z Reads: 83

```
it is always best to follow the directions provided with your own particular BMS because models can be Subtley different.
```

---
## \#11 Posted by: JuniorPotato93 Posted at: 2016-07-21T01:59:37.838Z Reads: 82

```
Original I wanted to do 40 amps per motor but I did not find a 8S bms that was rated for 80amps continuous. Unless you're saying I'll probably peak at 40 per motor/80amps across the system in which case would a 60amp BMW work?
```

---
## \#12 Posted by: Jinra Posted at: 2016-07-21T02:06:56.202Z Reads: 81

```
You should check with the BMS's documentation or manufacturer as @lowGuido mentioned. You probably won't draw 80A continuous on the powers, but having a higher limit gives it some headroom for burst.
```

---
## \#13 Posted by: JuniorPotato93 Posted at: 2016-07-21T02:13:54.604Z Reads: 80

```
Okay so set the limit on the motors to 40( if the manufacturers recommendations allow for it) and put a 80 amp inline fuse before the BMS should it want to go over 80
```

---
## \#14 Posted by: JuniorPotato93 Posted at: 2016-07-21T02:31:50.070Z Reads: 78

```
So I found link in the forums for bestech, hadn't seen that yet, and it looks like they do carry 8S 80amp bms's so I'm going to use that instead to be safe.  Thanks for the help.
```

---
