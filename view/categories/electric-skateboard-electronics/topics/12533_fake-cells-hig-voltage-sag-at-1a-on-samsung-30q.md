# Fake cells ? (Hig voltage sag at 1A on Samsung 30Q)

### Replies: 9 Views: 1551

## \#1 Posted by: JullianS Posted at: 2016-11-05T15:19:13.902Z Reads: 155

```
Hi guys, I am building my battery pack out of samsung 18650 30Q cells that I got from my chinese boss for free, I proceeded to test them and found out that they sag pretty hard at 1A load.

The tested capacity from 4.05V down to 3.1V (resting voltage)was 2542mAh at 1A load, which seems reasonable.
They do not get hot at all though, even after 2 hours of discharge.

The first test I run was a Li-ion discharge program at 1A... and it couldn't even start correctly as the cell voltage would fall from 4.05V (at rest) down to 2.5V (in load), which would trigger the low voltage cutoff and stop the discharge.

Then, after a little bit of research, I used the 1A discharge function in NiMH mode and set a very low cutoff voltage of 1.3V. I found out that they can sag down to 1.3V and go back up to 3.1V at rest (that's when I got a cell capacity of 2542 mAh).

When I see you guys talk about a voltage sag of 20-30% at 5C I kind of understand, and my cells getting a 40% to 60% sag at 0.4C... that worries me a bit since I plan on using my battery at 15A per cell

I mean, they seem like they have the right capacity but the discharge tolerance is clearly not there. Are they fake cells ? Or am I doing something wrong ?
```

---
## \#2 Posted by: mattdig Posted at: 2016-11-05T15:40:54.353Z Reads: 144

```
Were the batteries used before you got them?
```

---
## \#3 Posted by: smurf Posted at: 2016-11-05T16:59:34.266Z Reads: 129

```
Maybe it's the tester . Does a volt meter get the same results? Can they light up a flash light?
```

---
## \#4 Posted by: Ackmaniac Posted at: 2016-11-05T17:15:39.328Z Reads: 123

```
When you switched to NiMH discharge then you try to discharge a already completely discharged cell. I guess you have real 30Q cells. Charge them to 4,2 V and discharge them to only 2.5V, not lower than that. I for examlpe discharge my cells only to 3V. When the discharger shuts off the voltage goes back to 3,6V but when i put some load on them then they sag down to 3V again very quick. That is the nature of a Li-ion cell. And when you discharge them lower than 2.5v at load you will destroy them. It it is also not safe anymore because the cell can get serious damage by that and maybe explode. So don't do that.
```

---
## \#5 Posted by: JullianS Posted at: 2016-11-06T03:15:21.299Z Reads: 98

```
Thank you guys for your answers !

@mattdig I don't think they were used before as they were very clean and I didn't notice any no soldering/Wielding marks  

@smurf I thought about that and "tested the tester" on a 3S 2000mAh lipo battery, and it worked without any significant voltage sag. The volt meter gave me the same results when in load, but if the tester is screwed up, it would still give me the screwed up voltage from the tester as the battery is wired to it when in load. The voltages at rest were mesured with the voltmeter, charger disconnected from the battery.

@Ackmaniac Ah, do you think a cell resting at 4.05V is discharged because when I tried to charge it it went to 4.2V in seconds... so I figured it was charged. That might indicate a charger malfunction again. But yeah, I won't try to discharge the battery at such low voltages, promess :smile: .

Anyway, thanks for the advice guys, i'll try: 
- discharging with another charger
- charging with another charger
- with a flashlight

I'll keep you updated !
```

---
## \#6 Posted by: Ackmaniac Posted at: 2016-11-06T03:20:00.681Z Reads: 82

```
The charger is fine. When you charge it you charge it with a higher voltage. And 4.2 V is the max voltage of a li-ion cell. And under load the voltage should not go lower than 2.5 v. And at 4.05 they had roupfly around 80% till 90 % capacity. 
But when you discharged them to 2.5 volts and the charger stopped discharging because the cell would drop under load below 2.5 the cell was empty. But then you continued in NiMH mode which you should not do.

And if you still think that they are broken then please send them to my. I can throw them away for you :joy:
```

---
## \#7 Posted by: JullianS Posted at: 2016-11-06T03:32:40.328Z Reads: 78

```
Okay but the problem is : 

When they are at 4.05V, and I put the charger in dischrge mode at 1A, they sag down to 2.5V (I mean the voltage goes down to 2,5V in 3 seconds) and then the charger stops because of the low voltage cut off

If only I was not in china i'd send some to you, no problem :slight_smile:
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-11-06T03:34:02.031Z Reads: 75

```
Ok that voltage sag is too much. then maybe the charger is really broken.
```

---
## \#9 Posted by: JullianS Posted at: 2016-11-06T03:35:15.410Z Reads: 73

```
Okay I'll check that as soon as I can, thanks man !
```

---
