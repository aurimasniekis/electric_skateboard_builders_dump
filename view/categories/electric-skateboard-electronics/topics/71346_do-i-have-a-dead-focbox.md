# Do I have a dead FOCBOX?

### Replies: 25 Views: 398

## \#1 Posted by: RHill051 Posted at: 2018-10-16T00:29:17.349Z Reads: 103

```
Hey guys, so I've got a focbox that is flashing the fault light in sets of 3 repeatedly. I initially understood this as a sign the DRV chip was bad. So I desoldered it and replaced it. The ESC powers on but is still flashing the fault light. I can connect to it just fine but when I try to do a motor detection it said "Bad Detection Result Received". I should mention that I was given this FOCBOX by a friend who tried to desolder the motor leads and solder the bullet connectors right to the board. He told me his soldering iron wasn't getting hot enough and he had to leave the iron on the board for quite awhile to get the solder to melt. I'm guessing he fried something but I'm not sure what. If anyone had any advice I would greatly appreciate it. I already tried asking both @CarlCollins and @JohnnyMeduse but I'm guessing they are either busy or not sure as I haven't heard back from them.
![image|500x499](upload://5Cmx7LzpqGdjIjyOB7clSjL21GJ.jpeg)![image|498x499](upload://gTFQ8vifft6DBZ154nTWBeoUbbC.jpeg)
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-10-16T00:31:22.544Z Reads: 96

```
does it appear when you connect it to your pc and open the bldc tool?
```

---
## \#3 Posted by: dareno Posted at: 2018-10-16T00:55:48.435Z Reads: 90

```
Try upping the duty cycle and trying again
```

---
## \#4 Posted by: RHill051 Posted at: 2018-10-16T01:10:21.708Z Reads: 89

```
[quote="mynamesmatt, post:2, topic:71346, full:true"]
does it appear when you connect it to your pc and open the bldc tool?
[/quote]
yup, it shows up in BLDC and Ackmaniacs tool. (its currently running FW 3.102)

[quote="dareno, post:3, topic:71346, full:true"]
Try upping the duty cycle and trying again
[/quote]
that doesn't seem to do anything, I bumped it up from .05 to .1 and then to .15 (not sure how far up to go using Ackmaniacs tool for the configuration.
```

---
## \#5 Posted by: dareno Posted at: 2018-10-16T01:12:19.944Z Reads: 80

```
One of my motors only detects on .2 and the other on .15 so maybe take it up another increment.  Check the fault window.
```

---
## \#6 Posted by: RHill051 Posted at: 2018-10-16T01:14:24.376Z Reads: 74

```
Nope, still a no go... here is the debug console:
![image|690x80](upload://3mOoPUH9q8DjcsknoqAZMm5EOGd.png) 
Also, the fault light on the FOCBOX is still flashing in sets of 3 even while I successfully update other values on the ESC such as voltage setting and what not.
```

---
## \#7 Posted by: jojamcha Posted at: 2018-10-16T01:14:31.868Z Reads: 73

```
Hello everyone. I am very new to this website and am very sorry to intrude on your conversation, but I just have one question to ask myself. Do you know how to start a thread? I have a few problems I need solving. :sweat_smile:
```

---
## \#8 Posted by: RHill051 Posted at: 2018-10-16T01:26:47.186Z Reads: 71

```
I sent "threads" and "mem" to the terminal in the Ackmaniac tool and here were the results. I don't know if any of this is helpful in determining the issue but I don't know what else I can pull out of the ESC other than this. 
![image|690x384](upload://9Kl1fWdlhYKOtPlrvm5WxbfcMbS.png)
```

---
## \#9 Posted by: mynamesmatt Posted at: 2018-10-16T02:05:40.491Z Reads: 67

```
@jojamcha you go to the "new tab" and on the top right select "new topic"
```

---
## \#10 Posted by: mynamesmatt Posted at: 2018-10-16T02:06:21.600Z Reads: 68

```
go onto bldc tool and go to terminal. type "faults" and press enter. what comes up?
```

---
## \#11 Posted by: RHill051 Posted at: 2018-10-16T02:25:30.545Z Reads: 65

```
[quote="mynamesmatt, post:10, topic:71346, full:true"]
go onto bldc tool and go to terminal. type “faults” and press enter. what comes up?
[/quote]

No faults show up when I send the "fault" or "faults" command in the terminal :frowning: BUT, I was looking more closely at the board and realized that my a one or more of the cap resistors next to the DRV chip had been moved... so I took a few min to clean them up. (added flux and carefully tried to get them back to original position) there was also a stray wire (single strand) from the receiver wire that was touching one of the cap resistors that I got out of there. After that (and a good cleaning with isopropal alcohol the flashing fault light has now gone away!!! I tried to run the motor detect again with the duty cycle set at .05, .1, .15 and .2 but I'm still getting the same message "2018-10-15 21:19:00: Status: Bad Detection Result Received". I definitely feel like I'm moving in the right direction though :slight_smile: any other tricks to get the motor to detect?
```

---
## \#12 Posted by: RHill051 Posted at: 2018-10-16T02:31:53.296Z Reads: 64

```
When I do run a motor detect I can see the signal light on the FOCBOX gets brighter twice but the motor never spins. What are the chances the fets got overheated and one or more of them are bad? Does anyone know if its possible to test them to see? They look physically fine but my buddy said when he was trying to desolder the phase wires he burned himself on the heat sink because it was soaking up all the heat from his soldering iron that was passing through the fets...
```

---
## \#13 Posted by: RHill051 Posted at: 2018-10-16T18:24:11.639Z Reads: 57

```
[quote="Martinsp, post:34, topic:46309, full:true"]
You can test continuity between positive input and each phase wire, do the same with negative input.
[/quote]

I saw this message by @Martinsp but I'm not really sure what he is suggesting. I just to see if the mosfets are damaged from overheating. They look fine but the motor won't detect, and like I said I've tried changing the duty cycle from .05 up to .2 with no success. (how high is safe to go up on the duty cycle?)
```

---
## \#14 Posted by: Trdolan03 Posted at: 2018-10-16T19:01:24.429Z Reads: 48

```
Try testing in FOC. Had issues with my FOC box detecting in BLdC
```

---
## \#15 Posted by: RHill051 Posted at: 2018-10-16T19:38:33.688Z Reads: 47

```
[quote="Trdolan03, post:14, topic:71346, full:true"]
Try testing in FOC. Had issues with my FOC box detecting in BLdC
[/quote]

So I've never tried to and though maybe it would work. I hooked up the sensors too for good measure. When I click the box circled below I got this message. (this motor works fine with my other FOCBOX) Does this mean something to someone else? I'm not sure yet what it would mean.
![image|690x487](upload://cd3jECZ5MrrgCDkSnFnHTH15V9n.png)
```

---
## \#16 Posted by: Trdolan03 Posted at: 2018-10-16T20:46:55.101Z Reads: 37

```
Never seen that error before
```

---
## \#17 Posted by: RHill051 Posted at: 2018-10-16T20:48:09.912Z Reads: 37

```
I've only seen it referenced once before by @Eboosted but he never mentioned if he got it fixed or not... I sent him a message awhile ago to see if he did or not. Fingers crossed he's got a better idea whats going on :slight_smile:
```

---
## \#18 Posted by: Eboosted Posted at: 2018-10-17T00:26:25.191Z Reads: 35

```
If your have a flashing red light on the Focbox, you need to repair it or replace it, unfortunately there's nothing you can do. I suggest you get 2 Focboxes one for inmediate replacement and one as spare. Having a board under service waitiong for parts it's the worst thing an esk8r can experiment, that's why I have have 5 now only 2 working and 3 under service :smirk:
```

---
## \#19 Posted by: RHill051 Posted at: 2018-10-17T00:31:16.362Z Reads: 36

```
bummer :( so did the FOCBOX throwing the "L is 0" error get repaired or just replaced? I was talking to CarlCollins and he said after talking to his RA the issue has to do with a short on the DRV which kinda sucks cuz I just replaced the DRV. If I can't get this one fixed I gues it will just be a parts ESC lol but it would be nice to get it fixed and have a spare as you said. I do have another FOCBOX so I'm not dead in the water (just went for a nice 5 mile ride.. love this thing!!) but I'd also not like to see the money wasted.
```

---
## \#20 Posted by: Eboosted Posted at: 2018-10-17T00:32:50.880Z Reads: 34

```
Replace the Focbox and enjoy, forget about everything else :sunglasses:
```

---
## \#21 Posted by: Trdolan03 Posted at: 2018-10-17T00:48:37.235Z Reads: 33

```
Check all the pins on the drv chip and make sure non of them are shorted.
```

---
## \#22 Posted by: RHill051 Posted at: 2018-10-17T02:16:42.177Z Reads: 35

```
well I did check with my multimeter to make sure there were no shorts but I'm not sure if maybe there is an issue in this area... the protective coating on the board looks like it wore of and the soldier might be causing a short.. not sure though.. I don't know how to test it to be positive. My next idea is to possible just desolder all those little cap resistors and apply some solder past to just the pads and then try to reflow it so that I am more confident the solder is only where its supposed to be. What do you guys think? I'm all for having a good ESC but I don't want to just throw away $150 on this one.
![image|431x500](upload://9WS4C9qtgK3e6Ise6gYr0QNgsEr.jpeg)
```

---
## \#23 Posted by: briman05 Posted at: 2018-10-17T03:40:44.355Z Reads: 34

```
There was a shit load of heat put into this board. To me it looks like he burnt the components next to the one phase wire and next to the drv. Looks like your friend sold you a turd. Send it in and buy a new one
```

---
## \#24 Posted by: Trdolan03 Posted at: 2018-10-17T04:07:59.181Z Reads: 34

```
[quote="briman05, post:23, topic:71346"]
he burnt the components
[/quote]

I second this but I would try to fix the top left of the drv chip. There are 2 spots which look like they are shorted
```

---
## \#25 Posted by: RHill051 Posted at: 2018-10-17T04:51:51.261Z Reads: 29

```
I thought the same thing but if you look a the schematic you an see that there are a few pins that aren't used as well as those 4 pins that are bridged on purpose. I think I'll try to spend some more time looking at this schematic tomorrow and maybe try to ensure that the connections are all isolated from eachother with my multimeter and maybe there is a bridge somewhere in there that shouldn't exist. 
![image|690x488](upload://w2AO2jX9YTib30wde7sZCWNWOMY.png)
```

---
