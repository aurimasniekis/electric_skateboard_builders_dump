# 3.3v Dead on 2 FocBoxes

### Replies: 11 Views: 241

## \#1 Posted by: kuphjr Posted at: 2018-08-30T23:07:34.851Z Reads: 77

```
So I just set up my dual motor board w/ 2 Focboxes connected w/ canbus. Everything was working fine but then 1 motor stopped. Opened up the board and 1 vesc had no lights on. I unplugged and replugged it in and it started just fine. Then I made sure the canbus was connected securely and restarted the board. Now both vescs have no lights. I checked for power on the 5v pin and it was just fine, however the 3.3v pin showed now power. It seems somehow the 3.3v power supply shorted on both vescs. Opened up both vescs and nothing is visually wrong. It seems (hopefully) the only problem is the 3.3v circuit is just fried on both circuit boards from a short circuit. My question is, could I provide power to the 3.3v pin externally bypassing the one on each vesc so I can still ride my board? Could anyone who fixes vescs easily fix this issue? Any help or experience is welcomed. Thanks!
```

---
## \#2 Posted by: chuttney1 Posted at: 2018-08-30T23:50:04.542Z Reads: 60

```
It's definitely the LM3671MF-3.3_NOPB chip if its on the FOCBox. Definitely an issue it failed be there is no diode in series to prevent this issue.
```

---
## \#3 Posted by: kuphjr Posted at: 2018-08-30T23:53:12.277Z Reads: 56

```
Ok, so could I provide 3.3v externally using the 3.3v pin on the FocBoxes? I just got a 3.3v voltage regulator on Amazon with 1 day shipping and I can just stick a couple extra 18650s in the board to power it.
```

---
## \#4 Posted by: kuphjr Posted at: 2018-08-30T23:54:02.818Z Reads: 53

```
This would be a temporary fix, but I want to be able to ride this fall without needing to wait another 2+ weeks to have it repaired by @JohnnyMeduse
```

---
## \#5 Posted by: chuttney1 Posted at: 2018-08-30T23:58:58.382Z Reads: 48

```
[quote="kuphjr, post:3, topic:66599, full:true"]
Ok, so could I provide 3.3v externally using the 3.3v pin on the FocBoxes? 
[/quote]

Technically, yes if you wanna take the old school route of just soldering wires to a voltage regulator and soldering those wires to the traces of the 3.3V rail. But you are riding your board and risk having road vibrations damage a simple fix. 

I still don't know how you destroyed your 3.3V regulator...
```

---
## \#6 Posted by: kuphjr Posted at: 2018-08-30T23:59:00.885Z Reads: 45

```
[quote="chuttney1, post:2, topic:66599"]
LM3671MF-3.3_NOPB
[/quote]

I am also pretty good with a soldering iron & I am a 2nd year EE major.  Is this something I could replace on my own?
```

---
## \#7 Posted by: chuttney1 Posted at: 2018-08-31T00:02:04.361Z Reads: 45

```
[quote="kuphjr, post:6, topic:66599"]
I am also pretty good with a soldering iron &amp; I am a 2nd year EE major. Is this something I could replace on my own?
[/quote]

Got access to a hot air gun? Can be fixed with some solder flux and cleaning of area. Just verify it's the correct chip on the FOCbox. I'm do not know what they currently use other than what was posted in the schematics for this open source VESC. The LM3671MF-3.3_NOPB may not be the exact chip for the footprint on the FOCBox.
```

---
## \#8 Posted by: kuphjr Posted at: 2018-08-31T00:06:27.276Z Reads: 41

```
Alright.  Thanks for the info! In fact, I do believe I have access to a hot air gun in the EE lab, but I am not exactly sure how to use it to be honest. I will explore this further this winter.
```

---
## \#9 Posted by: kuphjr Posted at: 2018-08-31T00:09:28.558Z Reads: 40

```
I think I am just going to add a couple extra 18650s so I don't have to do any soldering to the FOCBox itself.  I'd rather not take the risk of damaging the circuit board since I will likely just have Johnny fix it at a later date.  I will just have a connector attached to the ground & 3.3v pins.
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-08-31T00:44:27.852Z Reads: 42

```
if u unplugged focbox while it was CAN connected and other one was running it probably CAN chip which shortens 3.3v vreg is normally OK just you need to replace CAN chip and can resistor.
```

---
## \#11 Posted by: kuphjr Posted at: 2018-08-31T02:41:43.300Z Reads: 32

```
that is exactly what I did so I am sure that is what happened. Seems like a bit of a design flaw, for example what happens if it were to come loose while riding? Anyway I guess Johnny will have to fix it for me because I have no idea where and what parts do purchase to fix
```

---
