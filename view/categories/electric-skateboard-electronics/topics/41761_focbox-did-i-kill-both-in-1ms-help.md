# Focbox: Did I kill both in 1ms? HELP

### Replies: 64 Views: 2733

## \#1 Posted by: rene Posted at: 2017-12-23T12:38:15.639Z Reads: 319

```
Hey guys,

I am in a kind of shock since yesterday night.
Was finalizing the beta of my build - getting the electronics to fit into a plastic box.

It was all working - I did not like those bullet motor cables - so I put some shrink tube on them to be save. Fitted the Focboxes inside and came to that idea that I could use those two Vedder Anti-Spark switches just in front of each box.

But it looks like one of those Anti-Spark Switches got its power-switch attached wrong - so it was ON instead of beeing off.

It was late - and it looks like I did connected  all stuff from the battery side - as doing it normaly from the electronics and do attach the battery at last.

There was a little spark inside of the XT60 connector from the Anti-Spark to the Focbox.

But than only the red light of the 2.4gHz receiver started to light up. Not one of the Focboxes LEDs came up anymore.

Here you see the step of applying the shrink tube.

<img src="/uploads/db1493/original/3X/3/0/3006c6124d942f4c87392775ba8056cb6d342a1a.JPG" width="690" height="318">

Here you see it with the finished shrink tube.

https://photos.google.com/share/AF1QipMBiuIM1sS8sfmdVPdKvgzhHQiEwF8T9MIlIfRL1iBDYcAGsDRhO5jFizrP7N55qg?key=ZlNUNHRVX2g2TVJoNjdva3NIVFpOSG1iampmbWJn


Here you see only the 2.4gHz receiver beeing powered - focbox shows no lights.
I disconnected everything not needed to extract possible failures.

https://photos.google.com/share/AF1QipMkiylstTUHGAqx8fHyTzDigBm8tLuRiNLb2joBQU4aKF-PWDc5_Teub7TGgQFdxQ?key=QmduX3lhQzBaMzRUOXAyMHhQRnA5cUpEY29STlhn

So I opened one focbox - here are the pictures - But I dont see anythink blown up - nor does it smell burned.

<img src="/uploads/db1493/original/3X/a/7/a7309e73cf70feec9db549d0df395c0a7f6fa248.jpg" width="666" height="500">

Backside - only that white on the chip in the middle of the caps on the right - seems strange.
<img src="/uploads/db1493/original/3X/7/e/7e69610e710a9c0a6e17f3c2a6d88788df525d7b.jpg" width="666" height="500">

Does some of the VESC gods do know whats going on?
Can I fix the focboxes somehow?
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2017-12-23T12:40:57.825Z Reads: 298

```
@scepterr 
This might seem like a situation that I've been through before
```

---
## \#4 Posted by: ARetardedPillow Posted at: 2017-12-23T12:46:39.579Z Reads: 294

```
Im not expert by any means but that chip kinda looks fried
http://prntscr.com/hrde8h
```

---
## \#5 Posted by: rene Posted at: 2017-12-23T13:50:49.494Z Reads: 284

```
Just opened the second focbox

<img src="/uploads/db1493/original/3X/4/2/424fd360a39f3211c65ec1576c981d616eae4630.jpeg" width="667" height="500">
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2017-12-23T13:55:01.688Z Reads: 278

```
Yea they kinda look a bit burnt to me
```

---
## \#7 Posted by: rene Posted at: 2017-12-23T13:56:22.120Z Reads: 276

```
It looks like a white powder from colombia spread all over that chip.

What is that chip? Name? Numbers?
```

---
## \#8 Posted by: Kug3lis Posted at: 2017-12-23T14:06:27.085Z Reads: 274

```
It's diode I think, and I think you reversed polarity...
```

---
## \#9 Posted by: Kug3lis Posted at: 2017-12-23T14:07:34.227Z Reads: 273

```
I guess the diode protected your whole board, so you just need to replace it ;)
```

---
## \#10 Posted by: rene Posted at: 2017-12-23T14:10:07.857Z Reads: 272

```
I just un-installed on box.

GFZ 74A 

is written on it.

seems to be a z-diode?

Great - but where to get this "thing" in Hamburg in the next 3 hours, 
and find an SMD soldering pro.
```

---
## \#11 Posted by: rene Posted at: 2017-12-23T14:17:01.973Z Reads: 264

```
Do got an idea - what kind of spec's of this diode I should look for?
```

---
## \#12 Posted by: Kug3lis Posted at: 2017-12-23T14:34:06.830Z Reads: 262

```
Hmm, I can see the number in schematics

<img src="/uploads/db1493/original/3X/c/b/cb4b9276a1ada313589a7e41325aa210300063b6.png" width="690" height="400">

But its zener diode... Hmm, It should be transient voltage zener diode...
```

---
## \#13 Posted by: Kug3lis Posted at: 2017-12-23T14:36:50.492Z Reads: 254

```
[quote="rene, post:10, topic:41761"]
GFZ 74A
[/quote]

Maybe this, don't know because can't find correct marking on datasheets

http://www.littelfuse.com/products/tvs-diodes/surface-mount/smcj/smcj51.aspx
```

---
## \#14 Posted by: Kug3lis Posted at: 2017-12-23T14:38:25.119Z Reads: 247

```
I think technically it shouldn't make the focbox to not work... Maybe you can try to remove it. 

https://en.wikipedia.org/wiki/Transient-voltage-suppression_diode

I am not pro at this field so I cant help much with TVS
```

---
## \#15 Posted by: rene Posted at: 2017-12-23T14:39:49.195Z Reads: 239

```
you mean remove it and short the connection?
```

---
## \#16 Posted by: Kug3lis Posted at: 2017-12-23T14:40:10.205Z Reads: 244

```
Just remove do not shorten
```

---
## \#17 Posted by: rene Posted at: 2017-12-23T14:41:45.291Z Reads: 243

```
and leave those two solder points open after removing?
```

---
## \#18 Posted by: Kug3lis Posted at: 2017-12-23T14:42:55.809Z Reads: 241

```
Yeah, but I can't guarantee it will make a change, because from logic it shouldn't make a change.... Maybe something else is also burned... But not visible
```

---
## \#19 Posted by: Quezacotl Posted at: 2017-12-23T14:45:33.628Z Reads: 243

```
Have you even measured any voltages? To see in what point it stops..
```

---
## \#20 Posted by: rene Posted at: 2017-12-23T14:48:14.618Z Reads: 239

```
Great Question!

I am a software guy - have no f**cing clue - where to put the multi-meter to find out.
At least that 2.4gHz receiver and the bluetooth module got power.
```

---
## \#21 Posted by: Quezacotl Posted at: 2017-12-23T16:56:44.982Z Reads: 216

```
Measure if there is battery voltage on both side of the diode in question.
Measure if there is about 3,3V and 5V between any three legs on the GH12E(on backside of board)
Measure also all other same looking diodes if they got about 0,2V - 0,7V.
```

---
## \#22 Posted by: Kug3lis Posted at: 2017-12-23T17:08:04.811Z Reads: 203

```
It's not diode it's TVS
```

---
## \#23 Posted by: rene Posted at: 2017-12-23T17:08:49.118Z Reads: 206

```
[quote="Quezacotl, post:21, topic:41761"]
Measure if there is about 3,3V and 5V between any three legs on the GH12E(on backside of board)
[/quote]

there is 5.1v on that GH12E
there is no voltage on the big black GFZ 74A diode.

now I check the rest.
```

---
## \#24 Posted by: rene Posted at: 2017-12-23T17:16:24.062Z Reads: 198

```
there is some small black chip near the can bus connector. 
it has 6.7v
```

---
## \#25 Posted by: mmaner Posted at: 2017-12-23T17:29:43.482Z Reads: 196

```
I didn't read the entire thread, but if noone has said yet...when using can bus you should start the VESCs up at the same time or you risk killing can bus.
```

---
## \#26 Posted by: Kug3lis Posted at: 2017-12-23T17:31:50.553Z Reads: 190

```
and you do not need to connect 5V
```

---
## \#27 Posted by: rene Posted at: 2017-12-23T17:33:55.542Z Reads: 192

```
My CAN bus cable only has the data cables
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2017-12-23T17:50:36.135Z Reads: 193

```
[quote="rene, post:27, topic:41761"]
My CAN bus cable only has the data cable
[/quote]


Yeah, but it is doing a ground loop that can kill both Focbox... remove U401 and use split ppm or replace it. 

If you want to be sure just check if c25 is shorted.
https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse

[quote="Kug3lis, post:22, topic:41761, full:true"]
It's not diode it's TVS
[/quote]

I don't what you're talking about, but yes it is a TVS
```

---
## \#29 Posted by: rene Posted at: 2017-12-23T18:12:09.878Z Reads: 184

```
I measured C25 like you described in the other thread.
I took the multi-meter and it does "beeeeepp"  - is this the meaning of shorted?

C23 on the top side does not beep - it shows 5.1v
```

---
## \#30 Posted by: JohnnyMeduse Posted at: 2017-12-23T18:12:46.698Z Reads: 183

```
[quote="rene, post:29, topic:41761"]
is this the meaning of shorted?
[/quote]

yes exactly.

Edit: so basically U401 is Blown
```

---
## \#31 Posted by: rene Posted at: 2017-12-23T18:16:59.366Z Reads: 180

```
[quote="JohnnyMeduse, post:30, topic:41761"]
Edit: so basically U401 is Blown
[/quote]

And I am still unsure - what U401 is.
```

---
## \#32 Posted by: JohnnyMeduse Posted at: 2017-12-23T18:17:55.536Z Reads: 182

```
<img src="/uploads/db1493/original/3X/b/1/b15f2e47ee4cfbda4476bd9c1640a55988efa50e.png" width="666" height="500">
```

---
## \#33 Posted by: rene Posted at: 2017-12-23T18:19:42.495Z Reads: 180

```
Johonny - thanks for you help!

So I need this U401 and also the TSV? 
The one that has this white powder on it in my pictures?
```

---
## \#34 Posted by: JohnnyMeduse Posted at: 2017-12-23T18:22:23.970Z Reads: 180

```
[quote="rene, post:33, topic:41761"]
and also the TSV?
[/quote]

No TVS is fine.
```

---
## \#35 Posted by: rene Posted at: 2017-12-23T18:23:38.830Z Reads: 180

```
 what is the exact name of U401 - so I can search for it.
```

---
## \#36 Posted by: JohnnyMeduse Posted at: 2017-12-23T18:26:01.308Z Reads: 181

```
SN65HVD232

<img src="/uploads/db1493/original/3X/5/0/50e2e88a889c379f692adb63280e9c622ce11e41.png" width="662" height="500">
```

---
## \#37 Posted by: rene Posted at: 2017-12-23T18:26:16.463Z Reads: 172

```
is it this one?

[https://www.distrelec.de/de/schnittstellen-ic-can-so-sn65hvd232-texas-instruments-sn65hvd232dr/p/30022810](https://www.distrelec.de/de/schnittstellen-ic-can-so-sn65hvd232-texas-instruments-sn65hvd232dr/p/30022810)
```

---
## \#38 Posted by: JohnnyMeduse Posted at: 2017-12-23T18:27:08.762Z Reads: 175

```
Yes it is  :slight_smile:(10Char)
```

---
## \#39 Posted by: rene Posted at: 2017-12-23T18:31:46.706Z Reads: 178

```
And those two focboxes got killed - because one was powered on and the other 10sec later?
```

---
## \#40 Posted by: JohnnyMeduse Posted at: 2017-12-23T18:36:58.563Z Reads: 176

```
Yeah, you have to power them simultaneously,  or you occur the risk of creating a ground loop that will kill both can transceiver
```

---
## \#41 Posted by: rene Posted at: 2017-12-23T18:39:56.402Z Reads: 178

```
WTF!

Understood - I just realized it was the first time that the boxes were NOT powered on simultaneously - because I used two Vedder Anti-Spark switches with two power-buttons.
```

---
## \#42 Posted by: Quezacotl Posted at: 2017-12-23T18:42:00.673Z Reads: 178

```
Apparently so. Since you did not get 3V3 out, and CAN chip is bad, desolder the CAN chip and see if the FOCBox wakes up. If it doesn't, measure the C25 and if it still doesn't have the 3,3V, i would suspect the regulator(GH12E).

How powerful board are you going to make? Even one anti-spark circuit with one FET is enough for normal commuting.
```

---
## \#43 Posted by: rene Posted at: 2017-12-23T18:59:43.452Z Reads: 174

```
* 10s4p Sanyo 20700B 
* Street-Wing Motors 6374 / 190KV

I wanted to secure each Focbox with an 40A Fuse and those Anti-Spark Switches got 40A fuses inside - so I installed both.

Now I am a lot "smarter"  - thanks to @JohnnyMeduse and @Quezacotl.

<img src="/uploads/db1493/original/3X/9/d/9d9c8d1b804cd8f866e95c2e73037e608c884dce.jpg" width="374" height="500">
```

---
## \#44 Posted by: b264 Posted at: 2017-12-23T19:05:41.805Z Reads: 168

```
[quote="rene, post:10, topic:41761"]
GFZ 74A
[/quote]

Is the TVS diode [this one](https://www.mouser.com/ProductDetail/Vishay-Semiconductors/SMCG51A-E3-57T/?qs=cuN208rz%2FQ%2F9o%252bWPZPtznw%3D%3D)?

Looks like a SMCG51A
```

---
## \#45 Posted by: rene Posted at: 2017-12-23T20:47:15.144Z Reads: 166

```
Johnny,

I was joking with a friend via WhatsApp and ask him if he got some of those CAN chip around.
He sad no, I only got the newer version and then he gave me 10 of those:

http://www.microchip.com/wwwproducts/en/en010405

Could I use them?
```

---
## \#46 Posted by: Kug3lis Posted at: 2017-12-24T00:19:42.673Z Reads: 158

```
I am just curious how did CAN chip died then it has protections?
```

---
## \#47 Posted by: JohnnyMeduse Posted at: 2017-12-24T00:29:45.032Z Reads: 160

```
[quote="rene, post:45, topic:41761"]
I only got the newer version and then he gave me 10 of those:
[/quote]

you can always try them. 

[quote="Kug3lis, post:46, topic:41761, full:true"]
I am just curious how did CAN chip died then it has protections?
[/quote]

there is no protection, it is a design flaw that is present on every vesc or derivate on the market, except the 6 (since it is a different can chip)
```

---
## \#48 Posted by: Kug3lis Posted at: 2017-12-24T00:31:26.862Z Reads: 155

```
What about this

>Designed for operation in especially harsh environments, these devices feature cross wire protection, loss of
ground and overvoltage protection, overtemperature protection, as well as wide common mode range of
operation.

Oh well maybe just shitty chip... I usually use the ones with isolation...
```

---
## \#49 Posted by: JohnnyMeduse Posted at: 2017-12-24T00:38:13.217Z Reads: 145

```
NOPE, not a shitty chip, Ground loop problem... 

I just don't see what you trying to prove here
```

---
## \#50 Posted by: Kug3lis Posted at: 2017-12-24T00:40:30.207Z Reads: 146

```
I am not trying to prove anything I am just curious... That's all, I have been working, with multiple CAN systems, and never run into the problem with ground loops...

I am just trying to understand how that happened so that I could prevent this kind of cases in the future.
```

---
## \#51 Posted by: JdogAwesome Posted at: 2017-12-24T02:01:04.464Z Reads: 145

```
First off that TVS diode with the white gunk on it is not blown, my brand new FOCBOX's have it as well. Also why where you using two switches instead of just one connected to both FOCBOX's? And I wouldn't try using that different CAN chip unless it states it's a drop in replacement and all the pins are the same.
```

---
## \#52 Posted by: pat.speed Posted at: 2017-12-24T05:15:14.147Z Reads: 149

```
I think he had two switches so he could pull 80a (40a each switch)
```

---
## \#53 Posted by: rich Posted at: 2017-12-24T10:00:55.960Z Reads: 150

```
[quote="rene, post:43, topic:41761"]
I wanted to secure each Focbox with an 40A Fuse and those Anti-Spark Switches got 40A fuses inside - so I installed both.
[/quote]

You could wire the on/off switch in parallel to both antispark-switches like @esk8 did it. I don't know if it's necessary because the 40A fuse can take more than 40A for a short period of time, for example 60A for 10 seconds and even more for bursts. Also I don't know what happens if you use 2 switches and only one fuse blows (or one switch dies), maybe you could harm the second FOCBOX as well.  I had a single switch running on my MTB and the 40A fuse never got blown.

I would use 1 antispark-switch only and if you want a bigger fuse then you can desolder the fuse holder of the antispark and solder a bigger fuse like the one in the picture. 150A is too much but they are available in 80A. too.

<img src="/uploads/db1493/original/3X/d/8/d8bef06c03c5aea51dea5f4afe174435cf6f9fe2.jpg" width="690" height="388">
```

---
## \#54 Posted by: Acido Posted at: 2017-12-24T11:00:40.742Z Reads: 148

```
Why only 40a focboxes can handle much more
```

---
## \#55 Posted by: rene Posted at: 2017-12-24T11:38:28.531Z Reads: 147

```
[quote="rich, post:53, topic:41761"]
Also I don't know what happens if you use 2 switches and only one fuse blows (or one switch dies), maybe you could harm the second FOCBOX as well.
[/quote]

Thanks Rich, I had the same thought last night. What if I take two Anti-Sparks and one blows - it will automatically kill my other v4 "x-VESC".

Now I am heading into the office and try to de-solder that crapy CAN chip.
```

---
## \#56 Posted by: telnoi Posted at: 2017-12-24T12:17:17.648Z Reads: 139

```
There are anti-spark switches being sold that are capable of handling 80a or more/it's not just the fuse that is different. 

Two anti-spark switches and canbus may again lead to trouble in the future. Would opt for two receivers with disconnected canbus.
```

---
## \#57 Posted by: rene Posted at: 2017-12-24T12:41:11.979Z Reads: 139

```
Guys, I just came into my office and had a stupid idea while I saw that heat gun laying on my desk.

I grab a tong that grabbed that CAN chip and lifted the whole PCB 5cm. Pointed the heat gun at it and 5 sec later GRAVITY kicked in!

<img src="/uploads/db1493/original/3X/1/6/1683e98e0b51840337991b36d84a1d6548423a10.jpeg" width="375" height="500">
```

---
## \#58 Posted by: banjaxxed Posted at: 2017-12-24T16:28:50.594Z Reads: 133

```
There goes the warranty :stuck_out_tongue: good work
```

---
## \#59 Posted by: Octavio Posted at: 2017-12-24T23:48:13.257Z Reads: 128

```
JohnnyMeduse Fixed mine. Just send him pics of the inside of your foc box and he will let you know if he can fix them. It’s a bummer I fried mine as well.
```

---
## \#60 Posted by: rene Posted at: 2017-12-25T17:27:40.277Z Reads: 126

```
[quote="JohnnyMeduse, post:47, topic:41761"]
you can always try them.
[/quote]

OK - I tried but they dont talk - I suppose the MCP2551 does need more than 3.3v as the sn65hvd232 does.

Ordered 10 of the SN65HVD232. 

So project does need to wait until 2018...

Thanks for all the help from @JohnnyMeduse @Quezacotl  @Kug3lis
```

---
## \#61 Posted by: Kug3lis Posted at: 2017-12-25T17:58:19.906Z Reads: 124

```
Today, by mistake I connected each esc 5s apart and nothing burned same CAN and etc used...
```

---
## \#62 Posted by: JohnnyMeduse Posted at: 2017-12-25T18:51:46.937Z Reads: 119

```
[quote="Kug3lis, post:61, topic:41761"]
Today, by mistake I connected each esc 5s apart and
[/quote]

where the VESC power simultaneously ?

And was the Can Cable connected?
```

---
## \#63 Posted by: Kug3lis Posted at: 2017-12-25T19:53:00.644Z Reads: 117

```
CAN cable was connected, by accident I got my Y switch disconnected from VESC's because battery fell off so I plugged one by one with like 5s delay and nothing happened ;)
```

---
## \#64 Posted by: JohnnyMeduse Posted at: 2017-12-25T19:56:59.195Z Reads: 117

```
Guess you're lucky... Unlike most people.

I still DO NOT RECOMMEND to plug your vesc not simultaneously if the can cable is connected.
```

---
## \#65 Posted by: Winfly Posted at: 2018-10-13T00:03:56.163Z Reads: 48

```
hmmm if only i knew this. time to buy SN65HVD232
```

---
