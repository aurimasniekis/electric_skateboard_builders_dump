# Smoke a Torque Boards VESC?

### Replies: 27 Views: 1155

## \#1 Posted by: yelnats8j Posted at: 2018-05-21T01:09:16.188Z Reads: 229

```
I have a torque boards VESC and when I turned on my longboard it sparked and smoked up. ![15268648922687388534905976168566|666x500](upload://oKSIaiP1Jgh7tUl4zmpmYBW2kyS.jpg)

What might of cause this and  is there anyway to fix it?
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-05-21T01:18:18.841Z Reads: 220

```
cool story bro
```

---
## \#3 Posted by: yelnats8j Posted at: 2018-05-21T01:24:13.631Z Reads: 215

```
So pissed forgot to add the question.😂😂
```

---
## \#4 Posted by: mmaner Posted at: 2018-05-21T01:50:25.467Z Reads: 207

```
Post your settings and a pic of the connections, maybe we will be able to deduct from that what caused it.
```

---
## \#5 Posted by: yelnats8j Posted at: 2018-05-21T02:02:31.816Z Reads: 205

```
Allright I'll do it in the morning.
```

---
## \#6 Posted by: district9prawn Posted at: 2018-05-21T06:10:23.451Z Reads: 193

```
That capacitor looks ready to blow.
```

---
## \#7 Posted by: Zac13 Posted at: 2018-05-21T06:26:20.181Z Reads: 186

```
same.  

best way to fix it is to not cross wires, buy another one, and don't fuckup this time
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2018-05-21T09:59:32.671Z Reads: 166

```
Can you remove the heat shrink on the Cap Board and take some picture. Also if can post picture of each side of the vesc it could be helpful.
```

---
## \#10 Posted by: yelnats8j Posted at: 2018-05-21T10:43:29.834Z Reads: 165

```
![15268992407801542484707491944842|374x500](upload://4N5QDtKqHbXExAhNMPKa2ysfi9Q.jpg)
![15268993473694294278485150120145|666x500](upload://7yATJogf6ab5HegXwFYhoGP0oM.jpg)
![15268993693713183458646393830052|666x500](upload://oO3h3itS1n0ZNKvLT3p0CdWkney.jpg)
![15268993945772971778546624367876|375x500](upload://7mFPGJzMmWSJapL7OuAhZGwxEBU.jpg)
```

---
## \#11 Posted by: Martinsp Posted at: 2018-05-21T10:45:51.662Z Reads: 161

```
2 of the 3 capacitors vented/are cracked, that most probably was the smoke you saw.
The one on the left side is good, the 2 on the right are visibly cracked.
![builders|690x348](upload://cfSMHO2SVHHRrpEIzHWJNNo3G7l.jpg)

BTW what is this? looks like a burn mark can you confirm that it is/isnt a burn mark?
![builders|568x500](upload://oZmZfGuXz4NdD5JrESMduJmFkz6.png)
```

---
## \#12 Posted by: mixedcreation Posted at: 2018-05-21T10:49:12.549Z Reads: 159

```
What are the settings?
```

---
## \#13 Posted by: yelnats8j Posted at: 2018-05-21T10:50:40.336Z Reads: 159

```
What might have cause the capacitor to blow?
```

---
## \#14 Posted by: Martinsp Posted at: 2018-05-21T10:54:12.568Z Reads: 159

```
In most cases it is reverse polarity. But it can also be aging which sometimes leads to internal short circuit which creates a lot of heat so when the insides expand it blows the vent on top of the capacitor.

But since they are just cracked and dont really show any signs of violent blow out this could be caused by mechanical stress like squeezing them with an enclosure etc
```

---
## \#15 Posted by: yelnats8j Posted at: 2018-05-21T10:58:41.916Z Reads: 157

```
![15269002606274442540753183141004|666x500](upload://fp28AJavtF2VVsP7K1eEkbZZPxZ.jpg)![15269002879966527422084680783866|666x500](upload://cZE3mk7aVBJSdnXLE1W3WbYnOr5.jpg)
```

---
## \#16 Posted by: mixedcreation Posted at: 2018-05-21T13:32:08.105Z Reads: 138

```
What exactly is your build?  All the info the better in this matter?  Any pics of the electronics on the board?
```

---
## \#17 Posted by: yelnats8j Posted at: 2018-05-21T18:53:02.544Z Reads: 120

```
I noticed that, it looks like a burn make but I cant tell.

Correction It is burned right there.
```

---
## \#18 Posted by: Martinsp Posted at: 2018-05-22T07:23:29.105Z Reads: 100

```
That is a pretty significant damage, do you have any idea what caused it? It is easily repairable but we should first find what the cause is because if you bridge it and plug it in it is going to happen again if not worse.

Is there any chance you plugged it in reverse polarity? Probably not since connectors usually only work one way but just to make sure.
Was the VESC under some physical stress?
Is your motor OK? because it looks like the battery shorted through the PCB and the part I marked in red acted as a fuse, check the rest of your board to make sure.

I would suggest to take the clear heatshrink off and inspect/post pictures of the VESC.
```

---
## \#19 Posted by: pat.speed Posted at: 2018-05-22T07:52:20.963Z Reads: 92

```
Pretty sure that burn spot is on the opposite side to where the positive batt wire is connected
```

---
## \#20 Posted by: Martinsp Posted at: 2018-05-22T07:54:02.141Z Reads: 90

```
Yes that is correct, that is the path to the mosfet tabs on high side.
```

---
## \#21 Posted by: yelnats8j Posted at: 2018-05-22T14:45:36.112Z Reads: 78

```
I'm not completely sure what caused it because I have been connecting the battery to the VESC the same way since I've gotten it with no problems. 
The VESC was under no physical stress nothing on top of it or putting any pressure on it.
I wont know if the motor is ok until I get a new VESC going to get a FOC Box this time.
I will post better photos when I get home.
```

---
## \#22 Posted by: Martinsp Posted at: 2018-05-22T15:01:58.216Z Reads: 70

```
Good choice, be sure to check the motor, battery, BMS etc for some obvious damage just in case... You dont want to break your focbox in case the reason for the DIY VESC to blow was the rest of the system.
```

---
## \#23 Posted by: yelnats8j Posted at: 2018-05-22T20:18:37.591Z Reads: 58

```
Ok I checked the wiring didn't find any connections or bad soldering points that could of caused it just gonna let it go and move on I guess.

RIP DIY VESC
```

---
## \#24 Posted by: Martinsp Posted at: 2018-05-22T22:40:46.433Z Reads: 50

```
IMO you should try to get it to work... it may be easier than you think.

If you want to you can check if the 5V, 3.3V are not shorted to ground. And check if the + and - on input are shorted (after bridging the burned trace) and check if the power wires are not shorted to either + or - on input.
```

---
## \#25 Posted by: yelnats8j Posted at: 2018-05-22T22:50:27.719Z Reads: 48

```
Where would I find the stuff to fix it?
```

---
## \#26 Posted by: Martinsp Posted at: 2018-05-22T23:25:14.140Z Reads: 45

```
Well from what we know right now you will need 3 electrolytic capacitors. Depending on where you are from you can find them on mouser of farnell. Or maybe even locally.

But it would be better to check what is wrong with it, since for some of the parts like DRV you would need a hot air soldering station/iron to remove and install a new one.
```

---
## \#27 Posted by: yelnats8j Posted at: 2018-05-22T23:48:22.002Z Reads: 41

```
I'll probably save fixing the vesc for later, the FOCBOX is the easiest option for me as I dont have much room for hot air soldering station.
```

---
## \#28 Posted by: Martinsp Posted at: 2018-05-23T00:06:28.441Z Reads: 36

```
Sure, it is up to you. Good luck! :)
```

---
