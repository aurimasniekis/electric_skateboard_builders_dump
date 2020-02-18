# Ollin (Chaka) Vesc V1.1 On E-bike question

### Replies: 21 Views: 1393

## \#1 Posted by: rocka Posted at: 2017-11-29T23:40:39.217Z Reads: 203

```
I haven't seemed to get any response to my messages through the ollin website and i've seen chaka is pretty active on the forum. Hopefully I can get some community help and it's just some small problem or he sees this. I'm using the ollin Vesc V1.1 (the best one they sell) on a custom electric bike where I use it to power the back wheel. I was riding the bike a few days ago  and out of nowhere the back wheel locked up and stopped. After skidding to a stop I tried using the throttle and it wouldn't go anymore. When I tried to walk it with the battery disconnected the motor felt like it was in break and offered noticeable resistance when I spun it quickly but almost none when I spun it very slowly. I disconnected the the bullet connectors to the vesc and the motor spins fine. I checked for faults on the vesc but it is showing none.<img src="/uploads/db1493/original/3X/1/1/11dec96a75e9c4b7c369d663e0541a87366677d4.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/5/2/52ad12b3fcda6effd6f5e017523acc0e692395b0.jpg" width="666" height="500">
```

---
## \#2 Posted by: Cobber Posted at: 2017-11-29T23:43:56.710Z Reads: 187

```
@treenutter @longhairedboy
```

---
## \#4 Posted by: chinzw Posted at: 2017-11-29T23:59:23.483Z Reads: 180

```
Sounds like a shorted vesc, the fact that the resistance on the motor disappears when disconnected from the vesc indicates a short on the fets.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-11-30T00:00:24.156Z Reads: 180

```
Look like a blown mosfet
```

---
## \#6 Posted by: rocka Posted at: 2017-11-30T00:24:53.438Z Reads: 178

```
Would I be able to remove the aluminum heat sink that's covering them without causing any damage so I can check this? I took the screws out but the thermal glue seems to be holding the heat sink in place. I haven't applied too much pressure though so I wouldn't know if it's just thermal paste.
```

---
## \#7 Posted by: chinzw Posted at: 2017-11-30T00:26:00.326Z Reads: 174

```
wait for @chaka to reply, but im guessing its just thermal paste, which can generate a bit of a vacuum when the two mating surfaces are very flat.
```

---
## \#8 Posted by: chaka Posted at: 2017-11-30T01:23:12.922Z Reads: 168

```
Do you have any other info? You can start by giving a brief description of you specs, voltage, motor, mode of operation, ect.

Edit: I came off sounding like a d$@k! That's what I get for checking in while eating dinner. @JohnnyMeduse is right, sounds like a blown MOSFET. From what I know of ebikes your were probably running high voltage?... Either way let me know what you want to do, if you have skills and want to fix it yourself we can help you with parts but you will want to send it in if you have not done any reflow work in the past. Makes repairs much harder if the pcb is damaged/pulled traces.
```

---
## \#9 Posted by: rocka Posted at: 2017-11-30T02:21:47.018Z Reads: 158

```
[quote="chaka, post:8, topic:39710"]
Do you have any other info? You can start by giving a brief description of you specs, voltage, motor, mode of operation, ect.
[/quote]

6s 16000ah 10c battery 
Sk3 6364 168kv (1700watts)
Running bldc current limiting 
Using ppm from an arduino for throttle
```

---
## \#10 Posted by: rocka Posted at: 2017-11-30T02:27:13.561Z Reads: 144

```
[quote="chaka, post:8, topic:39710"]
@JohnnyMeduse is right, sounds like a blown MOSFET. From what I know of ebikes your were probably running high voltage?... Either way let me know what you want to do, if you have skills and want to fix it yourself we can help you with parts but you will want to send it in if you have not done any reflow work in the past. Makes repairs much harder if the pcb is damaged/pulled traces.
[/quote]

I don't have any reflow experience so sending it in would be best. How long do you think it would take?
```

---
## \#11 Posted by: chaka Posted at: 2017-11-30T14:31:39.298Z Reads: 127

```
We are getting a fresh shipment of components sometime this week so a repair will not take too long. We were in the weeds for a little while due to component shortage but we are almost clear of back-orders and repairs as of now.

Here is our contact info & address:

Ollin Board Company
PO Box 1340
Elephant Butte, NM
87935

9 a.m. to 5 p.m. "mountain standard time" you can reach me @ 650 761-1801
Give me a call if you want to talk more about your build and what might have gone wrong so it doesn't happen again.
```

---
## \#12 Posted by: rocka Posted at: 2017-12-07T16:11:55.884Z Reads: 109

```
i sent the vesc out and shipping says you've received it. any news on what went wrong?
```

---
## \#13 Posted by: saul Posted at: 2017-12-07T16:23:36.675Z Reads: 108

```
[quote="chaka, post:11, topic:39710"]
Elephant Butte, NM
[/quote]

Really? lol :joy:
```

---
## \#14 Posted by: chaka Posted at: 2017-12-07T18:09:23.581Z Reads: 106

```
You shorted your ppm cables. Its a quick repair so we are going to cover it. You will receive a tracking number when we send it out.

@saul You like that... Never been to or heard of the southwest United States? A butte is similar to a mesa, a flat top hill, only smaller, the names go from butte<mesa<plateau. The butte out here is actually the remains of a dormant volcano ironically...:grin:
```

---
## \#15 Posted by: saul Posted at: 2017-12-07T19:00:34.929Z Reads: 106

```
I guess its pronounced byoot not butt. but still. lol
I'm in the far southwest, but I haven't made it further east than vegas/hoover dam.
```

---
## \#16 Posted by: rocka Posted at: 2017-12-07T20:04:31.679Z Reads: 106

```
[quote="chaka, post:14, topic:39710"]
You shorted your ppm cables. Its a quick repair so we are going to cover it. You will receive a tracking number when we send it out.
[/quote]

@chaka oh wow, any idea how that could have happened? what pins shorted? all of the cables i have going to the vesc from the arduino are heat shrinked and isolated. ill double check all that wiring though. if the arduino is powered from a different 5v source do i need to run the 5v from the vesc, or can i just run signal and ground. or even then, should i power the arduino from the vesc 5v instead?
```

---
## \#17 Posted by: chaka Posted at: 2017-12-07T22:08:58.247Z Reads: 99

```
Looks like you pinched the ppm cable on something.
```

---
## \#18 Posted by: rocka Posted at: 2017-12-08T23:10:42.545Z Reads: 89

```
could it be pinched between the vesc heatsink and the caps?
```

---
## \#19 Posted by: chaka Posted at: 2017-12-08T23:47:40.081Z Reads: 88

```
It looked like it was pinched on the other end of the caps.  You also have added a lot of battery cable  length. It should be fine as long as you don't have a really long mating cable that is attached to your power source. Not a bad idea to add more capacitance if you have really long battery cables.
```

---
## \#20 Posted by: rocka Posted at: 2017-12-24T05:10:40.499Z Reads: 75

```
haven't heard from you for 2 weeks now. any news on when i'll have my part back? @chaka
```

---
## \#21 Posted by: rocka Posted at: 2018-01-08T20:31:44.440Z Reads: 59

```
its been over a month now. why haven't i received the vesc yet??
```

---
## \#22 Posted by: scrapheap Posted at: 2018-01-08T20:38:44.379Z Reads: 53

```
He is no longer on the forums, last I checked. Best bet is to just call him...
```

---
