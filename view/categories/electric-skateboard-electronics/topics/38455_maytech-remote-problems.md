# Maytech Remote Problems

### Replies: 34 Views: 1977

## \#1 Posted by: Bensaida Posted at: 2017-11-15T23:02:39.724Z Reads: 252

```
So, I am currently using the Maytech remote with the Pulse Echo board. I am having this problems, where sometimes when i am throttling, it suddenly ramps down speed/brakes, then returns to normal speed. Does anyone have any clue on whats going on?


Here is a pic of the inside of the enclosure. This is after i moved the receiver to the separate compartment.
<img src="/uploads/db1493/original/3X/d/7/d731b2b1a3ecb32359f02a324df2fc5e37daf835.jpeg" width="374" height="500">
```

---
## \#2 Posted by: Bensaida Posted at: 2017-11-15T23:08:51.834Z Reads: 234

```
Any clue or idea works. Even if you dont know what youre saying and its just a potshot, any suggestion works. Also dont mind the wire management haha


I JUST NEED TO FIX IT haha
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-11-16T01:37:25.586Z Reads: 214

```

1. remote need rebinding, chage battery, or receiver is failing.
2. vesc is slowly dying, I experienced it.
3. vesc has fail safe option. u can turn off or increase time limit.
4.battery is low
5. u r exceeding erpm
```

---
## \#4 Posted by: michaelcpg Posted at: 2017-11-16T02:17:08.584Z Reads: 201

```
Could the connection dropping out briefly
```

---
## \#5 Posted by: mmaner Posted at: 2017-11-16T02:20:14.175Z Reads: 196

```
Could be u related to the remote.  That could be a BMS issue or VESC issue.
```

---
## \#6 Posted by: Bensaida Posted at: 2017-11-16T02:26:20.100Z Reads: 190

```
before I moved the receiver, there were certain deadzones where the remote would take 1-2 seconds to accelerate or brake after pushing the throttle.So pretty sure its the receiver
```

---
## \#7 Posted by: Bensaida Posted at: 2017-11-16T02:26:36.451Z Reads: 178

```
yea, but why dropping out?
```

---
## \#8 Posted by: michaelcpg Posted at: 2017-11-16T03:07:38.635Z Reads: 178

```
They're not particularly reliable remotes tbh
```

---
## \#9 Posted by: mmaner Posted at: 2017-11-16T03:10:31.213Z Reads: 171

```
Mine has been ultra reliable.  I've been using for about 3 months now.  

It took me a little while to get used to the form factor, I was used to the benchwheel grip. Now that I'm used to it it feels more natural than the gun grip style of the benchwheel. 

I actually bought 2 more for a couple of other builds because it's been so reliable.
```

---
## \#10 Posted by: michaelcpg Posted at: 2017-11-16T03:16:26.755Z Reads: 164

```
The one I've been testing drops out consistently in several areas on my commute to work. My friend's had the same issue with several other areas around town
```

---
## \#11 Posted by: Bensaida Posted at: 2017-11-16T03:18:17.019Z Reads: 154

```
yep. That's the issue
```

---
## \#12 Posted by: michaelcpg Posted at: 2017-11-16T03:20:05.379Z Reads: 141

```
Get a GT2B and one of the various custom enclosures available for it. I've been using mine for over a year, never had a single dropout
```

---
## \#13 Posted by: dAeM0N1K3 Posted at: 2017-11-16T03:26:18.059Z Reads: 142

```
I've had a similar experience with remote disconnect. I am still not certain what the cause is. Initially I thought it was the crappy Maytech VESCs my Raptor1 came with, but I have since installed 2 brand new FOCBOXs. All was going well until I rode downtown Chicago for a while, then I experienced some drop outs when accelerating. I didn't have this problem in the suburbs where I live. So I'm beginning to think there is some radio interference when riding downtown.

I've also read some stories about the first gen Raptor1s having problems with the carbon fiber lid causing interference. However, I do think I have a later generation lid, but I'm not 100% certain since I bought the board used used on this forum.
```

---
## \#14 Posted by: michaelcpg Posted at: 2017-11-16T03:30:02.640Z Reads: 137

```
Based on consistency of where my dropouts occur, I'm guessing its prone to interference from specific frequencies
```

---
## \#15 Posted by: Bensaida Posted at: 2017-11-16T04:05:43.489Z Reads: 142

```
that's what I thought
```

---
## \#16 Posted by: mmaner Posted at: 2017-11-16T04:09:26.195Z Reads: 143

```
@psychotiller have you had dropouts with the steez v2?
```

---
## \#17 Posted by: PredatorBoards Posted at: 2017-11-16T05:17:05.944Z Reads: 142

```
The interesting tidbit is that you had an RF shielded VESC (FOCbox). I was originally thinking it could have been a crosstalk interference issue, but I guess that's not the case. Has anybody attempted extending the antenna? Perhaps it's a weak signal.

Ben, see if you can ride around the dead zones, but hold the remote really close to the board... maybe even crouch more.

Edit @dAeM0N1K3 do you have pictures of how you wires the Bluetooth module to your FOCbox?
```

---
## \#18 Posted by: Bensaida Posted at: 2017-11-16T05:19:27.811Z Reads: 139

```
did that. Placed the remote literally on the board. No help
```

---
## \#19 Posted by: psychotiller Posted at: 2017-11-16T06:03:26.388Z Reads: 139

```
I had a customer send one back to me not too long ago because he said it had a weak signal. It tested out alright though..
```

---
## \#20 Posted by: Gunnisilli Posted at: 2017-11-16T12:01:07.587Z Reads: 130

```
I had the same problem with the same remote. My problems were caused by induction noise.

I made sure the signal lead (cable from receiver) and the receiver itself are nowhere close to the 3 phase wires that go from the Vesc to the motor. Cleared the problem right up.

Looking at your picture, I see that the signal wires are actually right next to the cables carrying AC current.... In two places.

I suggest you try to run the receiver leads as far away from the motor leads as possible and try again. Or you can try to shield them somehow.
```

---
## \#21 Posted by: longhairedboy Posted at: 2017-11-16T12:46:42.133Z Reads: 109

```
i can't get past the wire gauge on those phase leads. What are the power levels on that board?
```

---
## \#22 Posted by: Bensaida Posted at: 2017-11-16T15:01:48.955Z Reads: 107

```
Thanks dude!!! Hope it works
```

---
## \#23 Posted by: ATLesk8 Posted at: 2017-11-16T15:05:25.516Z Reads: 109

```
Yeah it's a vesc, but how much power can it safely be putting down...
```

---
## \#24 Posted by: Bensaida Posted at: 2017-11-16T15:05:52.087Z Reads: 107

```
No idea to be honest. Right now, trying ti diagnose my issue
```

---
## \#25 Posted by: Bensaida Posted at: 2017-11-16T15:09:26.784Z Reads: 115

```
Hey, so initially, the enclosure looked like this: <img src="/uploads/db1493/original/3X/4/2/421a68b7fc30b44eaf33d1696bf21aa97cc98f30.jpeg" width="374" height="500">




I was having “deadzone” issues where the remote would suddenly lag in high-traffic areas, but moving the receiver away from the capacitors helped the issue a bit. However, now, i am also experiencing the acceleration blips. Should i just get a new controlled?
```

---
## \#26 Posted by: longhairedboy Posted at: 2017-11-16T18:04:42.660Z Reads: 105

```
try moving the receiver to an outer edge. Move the BT module over and put it next to that. 

You never want the receiver anywhere near your phase leads or caps. That's just asking for cutouts.
```

---
## \#27 Posted by: Bensaida Posted at: 2017-11-16T18:24:11.545Z Reads: 103

```
In that picture, the recuever was under the VESC, and still experiencing issues
```

---
## \#28 Posted by: longhairedboy Posted at: 2017-11-16T18:26:15.703Z Reads: 107

```
probably too close to the PCB. You can't mix receivers with high frequency switching devices. 

Try moving it into one of those corner compartments off to the side ot the phase leads and make sure the antennae traces on the receiver are facing outward away from the innards of the box.
```

---
## \#29 Posted by: Bensaida Posted at: 2017-11-16T20:04:14.218Z Reads: 105

```
Receiver is too large
```

---
## \#30 Posted by: Berlad180 Posted at: 2018-03-08T11:31:23.369Z Reads: 90

```
Hi could you please share the model or a picture ? THanks!
```

---
## \#31 Posted by: mmaner Posted at: 2018-03-08T13:05:28.803Z Reads: 85

```
Of what?

(10 chars)
```

---
## \#32 Posted by: Berlad180 Posted at: 2018-04-22T10:53:45.765Z Reads: 77

```
Sorry i lost track, 
I meant a picture of the remote+receiver, that you found reliable.
Thanks
```

---
## \#33 Posted by: Danny414 Posted at: 2018-05-11T04:06:02.352Z Reads: 68

```
Did you figure it out?
```

---
## \#35 Posted by: Nedtrampz Posted at: 2019-01-15T01:09:31.050Z Reads: 30

```
To add to this. I have my maytech remote playing up in only certain areas. So bad down at the shorefront next to some portable wireless tower thing.. that i actually had nothing within 30m of it. 

I have moved my reciever to the outside of my box to try but its only made everything worse because now it seems to connect to everything i ride past. 

Back in the box for a ride today. If i remember ill be back with more later. I reckon its gonna be better..
```

---
