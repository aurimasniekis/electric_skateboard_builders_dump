# How should I go about programming double vesc

### Replies: 37 Views: 3320

## \#1 Posted by: moe_lester Posted at: 2017-03-26T19:13:49.358Z Reads: 277

```
Hello I'm about to start programming a double vesc setup. 

How should I go about doing it??

Program one vesc and make it master then just connect canbus and make other vesc slave and that it, or do I have to program to slave vesc aswell?
```

---
## \#2 Posted by: rpn314 Posted at: 2017-03-27T18:48:44.511Z Reads: 261

```
Setup each VESC independently and then enable the can-bus
```

---
## \#3 Posted by: moe_lester Posted at: 2017-03-27T18:57:40.998Z Reads: 252

```
great thanks, 

Im having another problem, sometimes my transmitter doesn't connect when I programming the Vesc. Well it connects to the receiver as the red light comes on, its just doesn't process the signal through the vesc. Sometimes it works after I replug it a few times, then I can see my signal on the pulsewidth. 

Anyone know what the problem could be why its so inconsistent????
```

---
## \#4 Posted by: chsknight Posted at: 2017-03-27T22:00:08.542Z Reads: 234

```
What kind of receiver are you using?
```

---
## \#5 Posted by: moe_lester Posted at: 2017-03-27T22:16:31.489Z Reads: 244

```
This one, im based in the uk. Standard 2.4ghz. So weird, sometimes the signal works and other times it doesn't come on Pulsewidth bar. 

http://alienpowersystem.com/shop/radio-transmitters/alien-power-system-2-4ghz-electric-skateboard-remote-control/
```

---
## \#6 Posted by: chsknight Posted at: 2017-03-28T22:11:08.701Z Reads: 252

```
Might be a low battery in the remote.  Does it always work when you have the remote right next to the receiver?
```

---
## \#7 Posted by: thisguyhere Posted at: 2017-03-28T22:39:42.614Z Reads: 246

```
i've been advised to skip the CAN and just split your bluetooth receiver so each vesc acts as a primary, as opposed to a primary+slave via the CAN.

in a primary+slave configuration, if the primary vesc goes out, your slave will stop working as well.

you're building redundancy if you split your bluetooth controller into primary+primary.

so...take the 3 pin servo coming off your bluetooth receiver, split it into two 3 pin servo cables, then each of those get connected into each vesc.

just make sure the 5v wire is CUT for one of the two servo cable going into one of the vesc.  otherwise you'll be sending 10v to your bluetooth receiver, which is probably a bad thing.

i learned this from @psychotiller, btw. 

<img src="/uploads/db1493/original/3X/0/0/004669811aeccd13168b25bc4b996762f1a20488.jpg" width="690" height="244">
```

---
## \#8 Posted by: moe_lester Posted at: 2017-03-28T23:37:08.370Z Reads: 238

```
Oh very interesting, but i do not have a Bluetooth receiver but im guessing it doesn't matter itll probably still work with my reciever. 

So the can the canbus be a bad thing or are people having problems with it, or is it just a measure incase your primary vesc fucks up and stops the slave from working as well.
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-03-29T00:01:28.466Z Reads: 230

```
[quote="moe_lester, post:8, topic:19731"]
i do not have a Bluetooth receiver
[/quote]

what?  isn't this the bluetooth receiver for your remote?

<img src="/uploads/db1493/original/3X/4/0/4079fe83d24ada8ba14a22dc2f496a46bb33609d.jpg" width="350" height="345">

[quote="moe_lester, post:8, topic:19731"]
So the can the canbus be a bad thing or are people having problems with it, or is it just a measure incase your primary vesc fucks up and stops the slave from working as well.
[/quote]

not sure if canbus is inherently bad.  nor do i know if people are having problems with it.

like i said, just splitting the connection gives you more redundancy.
```

---
## \#10 Posted by: Jebe Posted at: 2017-03-29T03:08:11.655Z Reads: 219

```
Have had lots of trouble with can bus. I think the root cause was dry solder connections inside the R-specs.
I'll be splitting the connection next time. The redundancy it gives you is worth it alone.
[http://www.electric-skateboard.builders/t/need-help-dead-vescx-and-3-dead-vesc/18666](http://www.electric-skateboard.builders/t/need-help-dead-vescx-and-3-dead-vesc/18666)
```

---
## \#11 Posted by: moe_lester Posted at: 2017-03-29T08:16:31.631Z Reads: 208

```
Honestly mate it could be im still new to this community. How do i make the servo split? 

Which wire from the second vesc shall i cut so my reciever isnt getting too many volts?
```

---
## \#12 Posted by: Maxid Posted at: 2017-03-29T08:24:45.429Z Reads: 210

```
[quote="thisguyhere, post:7, topic:19731, full:true"]
just make sure the 5v wire is CUT for one of the two servo cable going into one of the vesc.  otherwise you'll be sending 10v to your bluetooth receiver, which is probably a bad thing.
[/quote]

That is not how that works. The VESCs are connected in parallel - you can not make 10V out of two 5V lines this way.
```

---
## \#13 Posted by: PXSS Posted at: 2017-03-29T11:26:28.258Z Reads: 202

```
It's still necessary to cut one of the wires. Connecting the two 5v rails in parallel will end up killing one. The reason is that you can have small variations in the output of the regulator, and if one is higher than the other then you're sinking power into it which will burn it eventually.

---

@moe_lester
That's a 2.4ghz receiver not Bluetooth
```

---
## \#14 Posted by: Maxid Posted at: 2017-03-29T13:27:00.462Z Reads: 202

```
Not necessarily
http://www.electric-skateboard.builders/t/jittery-dual-car-esc-cause/17299/4

I had to reconnect them to make it work properly.
```

---
## \#15 Posted by: PXSS Posted at: 2017-03-29T14:30:52.947Z Reads: 198

```
It's got nothing to do with jitters or anything like that. 
You're just stressing it. As I said eventually it will fail. Google connecting two 5v rails in parallel. There are plenty of explanations as to why doing this is bad practice
```

---
## \#16 Posted by: Maxid Posted at: 2017-03-29T14:46:35.222Z Reads: 196

```
As you can see in the thread: it only started working once I reconnected them.

Also there is quite some contrary information out there with people saying one or the other.
In the end I have not encountered a single case where NOT removing the voltage line had a negative effect. 
https://www.rcgroups.com/forums/showpost.php?s=e83ddd9f7650bc51c141657d79e53a11&p=14651248&postcount=11
```

---
## \#17 Posted by: PXSS Posted at: 2017-03-29T15:07:43.019Z Reads: 191

```
I'm talking about electrical engineering here. Not RC forums. It's not a good practice. They teach you that in school. 

"In general, a power supply isn't expected to operate in a redundant mode (i.e. with outputs tied together).

In industry parlance, this function is called OR-ing (not O-ring). If a power supply is designed with OR-ing in mind, there will be several additions to the circuitry:

Some means of isolation (diodes or MOSFETs)
Some means of maintaining regulation at absolute zero load (anti-rollback)
Some means of load balancing (forced or droop)
These factors allow you to connect identical voltage rails together to provide load current beyond what a single supply can do, and allow for the rail to stay up (if the load can be delivered by N-1 units) if a single unit goes down. It also gives you some measure of protection if you accidentally connect a higher voltage to a lower voltage."
```

---
## \#18 Posted by: Maxid Posted at: 2017-03-29T15:13:38.215Z Reads: 179

```
I am not sure what you want me to say:
It did not work without the connection - now it does.
In my case I don't care what good practice is - I just want it to work.
```

---
## \#19 Posted by: PXSS Posted at: 2017-03-29T16:16:59.271Z Reads: 191

```
I read your thread and it is obvious you have a failing ESC since it jitters on a single drive setup and has nothing to do with the receiver wires. Some component in it is faulty. What I suspect is going on is that your 5v line is dropping, which is causing the signal line coming from the receiver to jitter. By connecting the second esc in parallel, that esc's 5v rail power gets pegged to the other and is most likely why it works. 

I would not give recommendations based on a faulty setup. Yours works as long as the second esc doesnt start to jitter and as is you are putting an extra load on it. 

The reason you are not meant to connect two 5v rails in parallel is stated above. You can take that however you want.
```

---
## \#20 Posted by: thisguyhere Posted at: 2017-03-29T16:40:32.342Z Reads: 193

```
[quote="PXSS, post:13, topic:19731"]
That's a 2.4ghz receiver not Bluetooth
[/quote]

you're totally right, not sure why i was so hung up on bluetooth.  yes, 2.4ghz remote receiver.

[quote="moe_lester, post:11, topic:19731, full:true"]
Honestly mate it could be im still new to this community. How do i make the servo split? 

Which wire from the second vesc shall i cut so my reciever isnt getting too many volts?
[/quote]

no worries, i should have given you a better explanation earlier.

parts needed: 

TWO 3-pin servo wire, male to male
ONE splitter, 3-pin servo wire, 2 female to 1 male - something like this
<img src="/uploads/db1493/original/3X/d/d/ddbdf2d941bc4d056b23e8387f4040b25ea0bf37.jpg" width="250" height="auto">

so, the MALE end of the splitter goes into your remote receiver, for me it's channel 2 (yours may be different, test it out):

<img src="/uploads/db1493/original/3X/0/d/0dbf6301e78f0fd565c62740872d08e21852af8b.jpg" width="304" height="246">

then the two servo wires are connected to the female ends of your splitter.

then each of the servo wires gets connected to your vesc.

watch torqueboards' instructions on how:

https://www.youtube.com/watch?v=j2fkMCEgzlM
https://www.youtube.com/watch?v=ywUfqtKF8Zg

here's the part where you cut the 5v wire.  but let me just explain why again.

if you look at the [vesc schematic](http://vedder.se/wp-content/uploads/2015/01/Schematic-1.png), the servo connection outputs 5 volts through the center pin.

your remote receiver requires 5 volts to operate.

since we're connecting two vescs, middle wire will now carry 10 volts to the remote receiver.

that's why we cut one of the 5v line.

put together it looks like this, RED is the 5v line.

<img src="/uploads/db1493/original/3X/5/9/59ce619a3e69ec59762b40bbc1930fae5a3e8390.jpg" width="690" height="244">
```

---
## \#21 Posted by: Maxid Posted at: 2017-03-29T16:45:07.638Z Reads: 175

```
[quote="thisguyhere, post:20, topic:19731, full:true"]
since we're connecting two vescs, middle wire will now carry 10 volts to the remote receiver.
[/quote]

No it will not - it will still carry 5V
```

---
## \#22 Posted by: thisguyhere Posted at: 2017-03-29T16:48:37.756Z Reads: 172

```
hm...if this is the case then no need to cut the wire.

i was strictly going off @psychotiller's advice but didn't measure it with a multi-meter.

at this point i'm too lazy to take stuff apart to test, but @moe_lester it may be good to check the voltages.  if after connecting everything the middle wire reads 5 volts then you're good to go, no need to cut anything.
```

---
## \#23 Posted by: PXSS Posted at: 2017-03-29T17:03:07.371Z Reads: 170

```
As @Maxid said, the voltage will still be 5v. 
The reason you cut the wire is what I explained above. It is not done to protect the receiver, it is  done to protect the VESCs from each other.
```

---
## \#24 Posted by: thisguyhere Posted at: 2017-03-29T17:16:29.619Z Reads: 164

```
[quote="PXSS, post:23, topic:19731, full:true"]
As @Maxid said, the voltage will still be 5v. The reason you cut the wire is what I explained above. It is not done to protect the receiver, it is  done to protect the VESCs from each other.
[/quote]

there you go then, makes sense.

i've cut one of the 5v wires, works great.
```

---
## \#25 Posted by: HTownBomber Posted at: 2017-03-29T17:21:51.629Z Reads: 162

```
I've also heard you should disconnect 1 of the red wires in Y-servo config.  Makes sense.

Maybe use the redundant red wire for a lil 5V tail light?  Curious if this would be bad for the vesc, and what kind of amp draw this 5V out would allow for safely.  @PXSS, maybe you could help here?  Sorry, I'm no electrical engineer as you might've guessed.
```

---
## \#26 Posted by: PXSS Posted at: 2017-03-29T17:41:37.429Z Reads: 163

```
I think the VESC can output 1A from the 5V rail. I'm just going by memory though. There are several threads about pulling power from the vesc for led lights. As long as you're not pulling a lot of power, you're not damaging anything
```

---
## \#27 Posted by: mmaner Posted at: 2017-03-29T17:46:02.358Z Reads: 165

```
I might have missed something, but why not can bus?
```

---
## \#28 Posted by: psychotiller Posted at: 2017-03-30T01:53:06.865Z Reads: 159

```
Cut the wire and you'll have no issues or surprises. I I've ran it both ways. Cut wire is better.
```

---
## \#29 Posted by: psychotiller Posted at: 2017-03-30T01:54:20.653Z Reads: 158

```
Canbus is just an unneeded complication and doesn't always work.
```

---
## \#30 Posted by: mmaner Posted at: 2017-03-30T02:09:54.315Z Reads: 158

```
I've heard that, but never had the problem myself. Weird.
```

---
## \#31 Posted by: ROFEN13 Posted at: 2018-01-12T01:28:51.794Z Reads: 109

```
Just curious, if I am splitting ppm, can I still use a Bluetooth module?
```

---
## \#32 Posted by: Mikenopolis Posted at: 2018-01-12T01:37:21.049Z Reads: 106

```
Pretty sure not. I kept running into problems because the apps can only connect to one so the other never connects. Got it to work once but never again
```

---
## \#33 Posted by: ROFEN13 Posted at: 2018-01-12T01:56:33.054Z Reads: 104

```
What about only connecting it to one VESC, or having a module for each. Not the most convenient I kmow, but possible?
```

---
## \#34 Posted by: GrecoMan Posted at: 2018-01-12T02:04:10.634Z Reads: 103

```
i’ll test it once I get my vescs back.  

got 10 modules in stock atm if you wanna pick one or two up 😋
```

---
## \#35 Posted by: ROFEN13 Posted at: 2018-01-12T02:11:55.115Z Reads: 99

```
I did see your other post. :) that is why I was asking these questions!
```

---
## \#36 Posted by: GrecoMan Posted at: 2018-01-12T02:18:25.628Z Reads: 101

```
hahaha cool!  should be getting my vescs back mid next week, will let you know :)
```

---
## \#37 Posted by: thisguyhere Posted at: 2018-01-12T04:22:34.411Z Reads: 98

```
you can most definitely use bt when splitting ppm. 

the vesc that the bt module is attached, make sure ppm+uart is enabled, set baud rate to 9600. 

then the vesc app (Ackmaniac) will multiply values if you set it was multi motor.
```

---
