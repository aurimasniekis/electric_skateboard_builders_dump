# Connecting a charge only BMS

### Replies: 8 Views: 2679

## \#1 Posted by: ShakeNBake7000 Posted at: 2018-06-07T09:25:19.407Z Reads: 314

```
So I've read some threads about connecting a BMS, but none of them specified if the BMS is discharge + charge or charge only. I want to connect the BMS to charge only, and I'm not sure where everything would go.
https://www.electric-skateboard.builders/t/connecting-a-bms-quick-guide-how-to/6122 
For example in this thread is connected to both charge and discharge, right? how would I change it to charge only?
I'm using this BMS:
https://www.ebay.com/itm/322460026383
With two 8000mAh 3s batteries in series.
Thanks
```

---
## \#2 Posted by: longhairedboy Posted at: 2018-06-07T13:40:22.253Z Reads: 282

```
most BMSs interrupt the negative path to control charging and balancing. This one doesn't seem to be any different. 

Connect your negative charge port lead to the "charge/discharge-" and then jump the negative side of the cell pack to "battery -" on the BMS using the same guage wire as your charging leads. 

Then just run a main discharge wire  to the main output connector (your XT-90 or bullets or whatever) directly from the cell pack's negative. 

viola. BMS is in loop for charging but bypassed for discharging.
```

---
## \#3 Posted by: ShakeNBake7000 Posted at: 2018-06-07T14:34:26.559Z Reads: 267

```
Thanks for the response, I'm not sure I completely understood what you meant.
What do you mean by "charge/discharge-"? if it's not too much to ask, is it possible you make a sketch to show it? just some basic drawing in paint or something to visualize it, I'm kinda new to this so It's hard for me to understand some stuff that is basic to others.
When you said main discharge wire what did you mean, where is it connected from the other side? one side the output to the VESC and the other one where on the BMS?
I did buy some wire of the same gauge of my battery cables.
Thank you
```

---
## \#4 Posted by: longhairedboy Posted at: 2018-06-07T17:46:15.906Z Reads: 250

```
![image|384x500](upload://xDOD5MD18TTpxFjBg8eOibDPfD0.jpg)

based entirely on the image of the BMS you posted.
```

---
## \#5 Posted by: ShakeNBake7000 Posted at: 2018-06-07T18:03:15.981Z Reads: 237

```
Wow, thank you for such a detailed picture.
The part with the balance cable, just connect both batteries to something like this adaptor?
https://hobbyking.com/en_us/6s-battery-pack-balance-charge-adapter-lead.html
And just connect the other side to the BMS?
Another thing I didn't understand is this part:
![2018-06-07_21h01_54|141x118](upload://58bB2CmuQKVnEJzjOE7MEFOY0fy.jpg)
Am I supposed to remove one of the balance cables and connect it to the main positive wire that goes to the vesc and charger?
Thank you for the help
```

---
## \#6 Posted by: longhairedboy Posted at: 2018-06-07T19:31:47.930Z Reads: 213

```
well if you follow this diagram, you have three wires coming off of the positive side of the cell pack. One for the charger, one for the positive balance lead, and one is a main discharge lead.
```

---
## \#7 Posted by: ShakeNBake7000 Posted at: 2018-06-07T19:37:41.481Z Reads: 213

```
So:
Positive charger wire - from Charger to vesc.
Positive balance lead - connected from the battery to the bms with this?
https://hobbyking.com/en_us/6s-battery-pack-balance-charge-adapter-lead.html
Not sure which is the main discharge lead though, is it the battery positive (not balance) wire connecting to the positive charger wire?
Edit:
So I made this sketch, I know its terrible but its how I'm understanding it. Is this the same as your sketch? or am I doing something wrong? 
![2018-06-07_23h48_18|690x405](upload://aVpRfVLtHm1qqrfEh00hqUHdkaW.png)
@longhairedboy What do you say?
```

---
## \#8 Posted by: MrPhantom Posted at: 2019-03-12T14:05:31.312Z Reads: 103

```
Its actually very simple just hook up the balance wires like you normally would and then connect the rest like this:  ![Capture|690x429](upload://prkQgYrbNDgl5G0AXpXeC4aGTy2.png)

This add a few benefits and risks tho:

Benefits:
- No limitation on your discharge capabilities caused by your BMS (some BMS's have a low discharge)

Risk:
- No discharge protection (You can kill your battery's if not paying attention to their  %)
```

---
