# Dual hub sine wave esc issue&hellip;..maybe battery wtf

### Replies: 18 Views: 459

## \#1 Posted by: Chase Posted at: 2018-10-08T21:52:24.037Z Reads: 143

```
For my lou board I use a 10S1P battery that I made with the charge only bestech HCX-D239. Out of nowhere today my motors stopped responding. At first I thought the battery was out of power so I went home and tried to charge..... it won’t charge. Each time I plug it in, the charge light goes red for just a second, then gos back to green. Checked the voltage with a meter and it looks like the battery is about half charged. Plugged my motors back in and they work all the sudden. The battery however will not charge. Checked all the connections and their all still solid. Do you think the bms somehow just went bad? It was just weird how the motors stopped responding for a little when the battery was still half full. If it was just a problem with the bms charging then you wouldn’t have expected the motors to be effected. This board doesn’t have a vesc, I am using the V1 sine wave esc from diyeboard. 

And yes I have changed chargers and check the charge port itself

![image|375x500](upload://cXnVS5qxyozPVKhkFYzmgVl331d.jpeg)
```

---
## \#2 Posted by: Lionpuncher Posted at: 2018-10-08T23:27:20.349Z Reads: 118

```
Do you have access to a dc volt meter (multimeter)?
```

---
## \#3 Posted by: Lionpuncher Posted at: 2018-10-09T00:10:48.801Z Reads: 112

```
I think you had a ‘fault’ with your esc. Likely battery sagged too much and went below voltage cutoff. I’d bet once you sort this charging issue, the board will work fine.
```

---
## \#4 Posted by: Chase Posted at: 2018-10-09T01:24:25.789Z Reads: 107

```
Thanks. Yeah I think the board will work fine, just weird that it suddenly won’t charge. I do have a meter.
```

---
## \#5 Posted by: ElectricCoast Posted at: 2018-10-09T03:28:50.240Z Reads: 100

```
Yeah you'll need a multi-meter to troubleshoot this issue.
```

---
## \#6 Posted by: Chase Posted at: 2018-10-09T04:19:24.213Z Reads: 91

```
I mean I’ve checked the voltage on everything I can think of. The battery is at 40.7V. The voltage at P- and B- both read 40.7. The cells are all connected to the balance wires and are all balanced.
```

---
## \#7 Posted by: Chase Posted at: 2018-10-09T04:22:51.125Z Reads: 88

```
And it just suddenly started working (charging) again when I plugged in the charger. What the hell.
```

---
## \#8 Posted by: Lionpuncher Posted at: 2018-10-09T04:32:23.437Z Reads: 88

```
That’s interesting. Maybe a cold solder joint on the bms.
Poking around usually solves the issue.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-10-09T05:06:26.327Z Reads: 80

```
Bypass the bms and look if your charger than charge the pack up to 42v. If yes replace the bms
```

---
## \#10 Posted by: Chase Posted at: 2018-10-09T05:21:51.488Z Reads: 80

```
When it randomly started charging again it charged to full. I just changed out all the solder joints on the bms. The weird thing is just that the bms is bypassed for discharge and the motors stopped working for a little while when this issue first started. The battery wasn’t empty so I don’t know why there would have been a huge voltage sag to shut down like that.
```

---
## \#11 Posted by: Chase Posted at: 2018-10-09T05:58:42.022Z Reads: 82

```
And now the motors won’t work again. The speed controller turns on but the wheels won’t respond. It’s not the controller, it’s paired fine. The battery charged all the way full and the voltage is correct at the connection to the speed controller.

I’m thinking this is a problem with the speed controller.
```

---
## \#12 Posted by: Chase Posted at: 2018-10-11T06:59:00.152Z Reads: 63

```
So the company that makes the esc has watched a video of the issue and is saying I broke the esc because I put silicone glue on it, causing it to overheat.....

![image|375x500](upload://aiS7RLbPinpeYjK3j21PHCwK0ck.jpeg) 

The esc only has silicone glue around the edges and where the power wires solder on (because on a previous one the wires came unsoldered here). I’m certainly no engineer, but I don’t see why such a small amount of silicone glue would suddenly cause it to overheat after it has been on it for months. When I questioned this, they just replied by saying try repairing the remote and disconnecting/reconnecting the motor wires. It kind of seems like they are fishing here. If it breaks this easily then fuck.....this is one of my only options due to size restrictions.
```

---
## \#13 Posted by: visnu777 Posted at: 2018-10-11T07:20:15.159Z Reads: 61

```
What are your space restrictions?
I also used one of these which mysteriously half died on me and they didn't give a damn about it.
```

---
## \#14 Posted by: linsus Posted at: 2018-10-11T16:00:04.615Z Reads: 57

```
...does it have a resettable fuse?..
```

---
## \#15 Posted by: Chase Posted at: 2018-10-11T18:08:25.931Z Reads: 54

```
Hello. I’m not sure if it has a resettable fuse. @visnu777 my space restrictions are basically exactly the dimensions of this thing 104 x 80 x 17 mm. I might be able to fit just s slight bit longer, but not even a mm taller. I really need something with a push to start option like this one has because I can’t fit a switch of any sort. If you know of any decent options I’d be happy to hear about it.

![image|375x500](upload://wtLc7OYpxMPjx5BujhinQGKQOK9.jpeg)
```

---
## \#16 Posted by: Chase Posted at: 2018-10-12T04:52:09.498Z Reads: 51

```
I don’t know anymore. Diyeboard says that the esc is broken, but I took the esc off and the battery suddenly won’t charge again. The other day it suddenly started working and charged up to full voltage somewhere around 41.5V. Then I check it today even though it hasn’t been used and it’s dropped to 36.9V. And once again it won’t charge. On one of my chargers the green light blinks instead of going to red and on the other it just stays green. They are trying to convince me to buy another esc but I sure as hell don’t want to spend the money if it’s really the bms.
```

---
## \#17 Posted by: Chase Posted at: 2018-10-19T04:32:56.875Z Reads: 38

```
Whatever the situation be, I bought a new bms because the battery still won’t charge. It’s at 36.9V disconnected from the esc. I checked all the solder connections and they’re solid.

The question that I’m hoping someone can shed some light on:

Why did the esc start fucking up at the same time as the battery? It’s a charge only bms so if the battery isn’t charging, that shouldn’t effect the esc. The battery isn’t empty and the cells are bypassing the bms during discharge.
```

---
## \#18 Posted by: yuweng Posted at: 2018-10-20T03:05:12.143Z Reads: 26

```
If you have another battery pack or BMS or ESC then swap them & you'll know which one is causing the failure. if you don't have any then check each cell with load, one of them should be lower voltage, thats the one causing problem. Eg. While spinning the wheels, check the voltage
```

---
