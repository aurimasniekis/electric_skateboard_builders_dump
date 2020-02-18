# So I fried a VESC

### Replies: 16 Views: 859

## \#1 Posted by: mervmonster Posted at: 2017-10-15T18:20:07.995Z Reads: 161

```
Greetings, these forums have been super helpful with programming my ESCs and stuff. I was hoping you could help me out again. I built a dual motor board using two VESCs. I was running sensor-less and at 12s. One of my ESCs does works fine and the other one blinks red 3 times whenever I give it a command. I rode my board down a bike-path and then put it in my trunk for 3 days. When I pulled it out, it was one wheel drive. I am not sure if the VESC fried on the ride or in the car. What im wondering is, how can I not smoke the second one (they are expensive) and is there any chance of revival for this ESC?
```

---
## \#2 Posted by: scepterr Posted at: 2017-10-15T18:21:33.854Z Reads: 161

```
First, plug it in to pc, check for faults and start from there
```

---
## \#3 Posted by: mervmonster Posted at: 2017-10-15T18:28:07.688Z Reads: 155

```
How would I go about that? Under motor configuration I hit 'detect parameters' and it just tells me that it had a bad detection result.
```

---
## \#4 Posted by: scepterr Posted at: 2017-10-15T18:29:58.234Z Reads: 143

```
Go to terminal, type "faults" without " "
```

---
## \#5 Posted by: mervmonster Posted at: 2017-10-15T18:33:54.728Z Reads: 136

```
"Fault            : FAULT_CODE_DRV8302" So is that the DRV chip? I don't want to smoke the second one.
```

---
## \#6 Posted by: mervmonster Posted at: 2017-10-15T18:34:22.683Z Reads: 134

```
Also what is a DRV chip? I just learned that from search ing the forums.
```

---
## \#7 Posted by: MysticalDork Posted at: 2017-10-15T18:35:50.516Z Reads: 130

```
The DRV chip is a combined mosfet driver, current shunt amplifier and voltage regulator.

There are several people here on the esk8 forum that will do the replacement for you, since it's a pretty much impossible to solder unless you have a full hot-air rework setup.
```

---
## \#8 Posted by: mervmonster Posted at: 2017-10-15T18:37:38.884Z Reads: 128

```
Awesome thank you! Any idea on cost? I pulled off the second motor and am now running a one wheel drive board :frowning:
```

---
## \#9 Posted by: MysticalDork Posted at: 2017-10-15T18:39:16.643Z Reads: 126

```
IIRC they charge about $10-15. Cheaper than buying a whole new vesc.
```

---
## \#10 Posted by: scepterr Posted at: 2017-10-15T18:40:05.327Z Reads: 127

```
You can send it to @JohnnyMeduse 
If youre around NYC I can take a look at it at my shop if you like. I do local service only
```

---
## \#11 Posted by: mervmonster Posted at: 2017-10-15T18:41:50.847Z Reads: 121

```
Thank you but im all the way in Colorado. Ill message him. Thanks a lot all.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-10-15T20:54:56.959Z Reads: 105

```
Are you running canbus?
Are you running FOC?
You should check the motor that was on the blown vesc. See if it has any short between the phase wires.
```

---
## \#13 Posted by: wafflejock Posted at: 2017-10-15T21:40:50.530Z Reads: 97

```
Keep in mind the component is about $10-15 think for doing the replacement it costs around $50 or so but haven't had it done myself (did blow a drv chip but just sent the blown board to someone to see if they can salvage it for themselves).  If you have a hot air rework station or are interested in learning you can try but VESC isn't a particularly simple board to learn on (easy to burn connectors pretty crowded board and dealing with the DRV chip is a lot of pins to have flow right or check/fix).

---

DRV8302 is the actual chip too http://www.ti.com/lit/ds/symlink/drv8302.pdf

http://www.mouser.com/search/refine.aspx?Ntk=P_MarCom&Ntt=113734323
```

---
## \#14 Posted by: mervmonster Posted at: 2017-10-15T21:55:36.020Z Reads: 90

```
I am running FOC and I originally thought it was the motor but I checked it and its fine. Makes me want to make some kind of universal pod because I have 2 motors and 1 working VESC. Are there any cheaper VESC substitutes?
```

---
## \#15 Posted by: Clonkex Posted at: 2017-10-15T22:22:03.047Z Reads: 80

```
The only real alternative to the VESCs are RC car ESCs like the HobbyKing X-Car Beast, but I guarantee you'll be disappointed if you go to those. Compared to the VESCs they're rubbish. The VESCs really are the only ESCs specifically designed for esk8.

Really the best option is the VESC6, which is significantly tougher then the VESC4 and won't blow DRVs. They're more expensive though, and there's less sellers for them, but they're absolutely the best option.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-10-15T23:39:26.240Z Reads: 67

```
Some Vescs can't handle FOC. 
I think BLDC is more reliable
```

---
